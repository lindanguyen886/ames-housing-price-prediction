# Ames Housing: Sale Price Prediction

## Objective
Support pre-listing housing price decisions using historical transaction data from Ames, Iowa.

## Decision Question
Given the characteristics of a house, what is a reasonable market price, and how confident can we be in that estimate?

## Data
Ames Housing dataset (De Cock, 2011), containing 2,930 residential property sales with structural, quality, and location features.

## Approach
- Exploratory data analysis to identify key price drivers
- Multi-model comparison using bootstrap resampling
- Model selection based on RMSE
- Final evaluation on a hold-out test set

## Models Evaluated
- Linear regression  
- Regularized regression (GLMNet)  
- Random forest  

## Key Results
- Best model: Random forest  
- Test RMSE: approximately $42,000  
- Key drivers: living area, neighborhood, condition, garage capacity, and age

## Tools
R, tidyverse, tidymodels, recipes, workflowsets, ranger, Quarto

## Output
- Full analysis: `ames-housing-price-prediction.html`
