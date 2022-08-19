# MMA-Significant-Strikes-Model
## Project Overview
Final Project for STAT 1361 (Statistical Learning and Data Science)
House Pricing Model

For this project, I created models in R to predict housing prices in the Pittsburgh, PA and Richmond, VA housing markets.  

Before model creation, I undertook some exploratory data analysis in order to better understand the data.  Based on this analysis, certain variables and observations were removed for various statistical reasons.

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
