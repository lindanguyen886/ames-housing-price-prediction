# Ames Housing: Sale Price Prediction

## Objective
This project is a practice-based analysis designed to support pre-listing housing price decisions using historical transaction data from Ames, Iowa.  
The main purpose of the project is to strengthen my understanding of the complete data analysis and modeling workflow through hands-on implementation.

## Decision Question
Given the characteristics of a house, what is a reasonable market price, and how confident can we be in that estimate?

## Data
The analysis uses the Ames Housing dataset (De Cock, 2011), which contains 2,930 residential property sales with detailed structural, quality, and location features.

## Approach
- Exploratory data analysis to understand price distribution and key drivers  
- Feature selection based on data relationships and domain reasoning  
- Multi-model comparison using bootstrap resampling  
- Model selection based on RMSE  
- Final evaluation on a hold-out test set  

## Models Evaluated
- Linear regression  
- Regularized regression (GLMNet)  
- Random forest  

## Key Results
- **Selected model:** Linear regression (baseline model)  
- **Reason for selection:** Lowest RMSE among the evaluated models  
- **Preprocessing steps:**  
  - Centering and scaling numeric variables  
  - Log transformation of sale price  
  - Grouping rare neighborhood categories  
  - Dummy encoding categorical variables  

- **Model performance:**  
  - Test RMSE ≈ 0.18 on the log-transformed sale price  

- **Key price drivers:**  
  - Living area  
  - Neighborhood  
  - Overall condition  
  - Garage capacity  
  - Year built  

## Learning Outcome
This is a typical end-to-end housing price prediction project, but it was very helpful for developing hands-on experience.  
Through this project, I improved my understanding of:
- How to structure a data project around a clear decision question  
- How to compare multiple models using a consistent evaluation framework  
- How preprocessing choices affect model performance  
- How to select a final model based on both accuracy and interpretability  

## Tools
R, tidyverse, tidymodels, recipes, workflowsets, ranger, Quarto

## 📄 Project Report
The full rendered analysis can be viewed here:  
👉 **[View the interactive HTML report](https://github.com/lindanguyen886/ames-housing-price-prediction/blob/2500091b5cb76be54243d588ad3ddfc71fcf7c79/Ams%20housing%20prediction.html)](https://github.com/lindanguyen886/ames-housing-price-prediction/blob/main/Ams-housing-prediction.pdf)**
