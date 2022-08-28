# MMA Model and Research Paper
## Project Overview

In this study, I attempt to determine whether the amount of significant strikes landed by mixed martial arts fighters influences the likelihood of attaining victory in later rounds of the fight.  I specifically look at those bouts that end in knockout (KO) or technical knockout (TKO) victories.  This analysis investigates the broader idea of "chronic weakening" of an opponent; i.e. does landing more strikes in previous rounds increase likelihood of knocking out opponents later in fights? 

To answer this question, I use UFC fight data from February 2014 through October 2018 to build two multiple binary logistic regressions.  I split the data into fights ending in the second round, and those ending in the third, due to differences in fatigue between these two rounds.  The predictor variables in these regressions are the relative proportions for each type of significant strike.  The response variable is the prediction of the bout's winner.  

After creating the full models, I backwards eliminate them to ultimately end up with two simple binary logistic regressions (done via AIC).  For second round KO/TKOs, head strikes are the sole statistically significant predictor, while for third round KO/TKOs, body strikes are the sole predictor in the model.

For more on the process, please check out the full [**journal article**](journal_article.pdf)!

Data attained from [**ufc-api**](https://github.com/valish/ufc-api)

## File Descriptions
[**mma_strikes_model.Rmd**](mma_strikes_model.Rmd): Code start to finish.  Starts with imports, then data manipulation/exploration, and finally modelling.

[**markdown.pdf**](markdown.pdf): Knitted output of the code.

[**raw_data.csv**](raw_data.csv): Raw data from kaggle, that was initially sourced from the repo [**ufc-api**](https://github.com/valish/ufc-api).  This is the only input file required to run the code. 

[**journal_article.pdf**](journal_article.pdf): Associated article that I wrote, which goes through the context, methodology, and results of the study.  Background on binary logistic regression can be found on page 10. 
