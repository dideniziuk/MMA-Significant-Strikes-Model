# MMA Model and Research Paper
## Project Overview

In this study, I attempt to determine whether the amount of significant strikes by a fighter influences the likelihood of that fighter attaining victory in later rounds.  I specifically look at those bouts that end in a knockout (KO) or technical knockout (TKO) victories.  This analysis investigates the broader idea of "chronic weakening" of an opponent; i.e. does landing more strikes in previous rounds increase likelihood of knocking out the opponent?

I use UFC fight data from February 2014 through October 2018 to build a multiple binary logistic regression.  The predictor variables in this regression are the relative proportions of each type of significant strike.  The response variable is the prediction of the bout's winner.  After creating the full model, I backwards eliminated the model to ultimately end up with a simple binary logistic regression of only head strikes (done via AIC).

For more on the full process, please check out the full journal article!

Before building the actual model, I first undertook some exploratory data analysis in order to better understand the data.  Based on this analysis, certain variables and observations were removed for various statistical reasons.

As per my professor's instructions, I built models on a training set which included variables like number of bedrooms, zipcode, and roof type.  The response variable for these predictive models was house price.  The output prices from the best performing (test set) model were submitted to be compared against actual home listing prices.  This, in theory, identified under-priced and over-priced properties.  
I employed various statistical learning and ML techniques to build and fit an optimal predictive model. These include regression, LOOCV, PCR, PLS, lasso regression, ridge regression, boosting, bagging, and random forest. 

Along with attaining predictions, we were also tasked with producing reports for technical and non-technical audiences of our findings and methods.  These reports help to keep interpretability of results in mind.  

Data attained from [**ufc-api**](https://github.com/valish/ufc-api)

## File Descriptions
[**housing_price_model.rmd**](housing_price_model.Rmd): rmarkdown code from start to finish.  Broken into subsections (imports, data exploration/alteration, modeling, final predictions)

[**test.csv**](test.csv): test data

[**train.csv**](train.csv): training data

[**testing_predictions.csv**](testing_predictions.csv): final csv export containing predicted prices

[**non_technical_report.pdf**](non_technical_report.pdf): brief business-oriented report describing the task at hand and the most important results in a non-technical manner

[**technical_report.pdf**](technical_report.pdf):  in-depth technical report walking through the various steps of the project.  follows same workflow as the code (housing_price_model.rmd).  explains reasoning for data alterations as well as takeaways from each individual statistical learning technique as applied to the data.  finally gives conclusions and interprets results
