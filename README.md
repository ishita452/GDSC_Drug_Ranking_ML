# GDSC Drug Sensitivity Prediction and Ranking Using Machine Learning

## Overview
This project uses machine learning to predict LN_IC50 values of anticancer drugs using the Genomics of Drug Sensitivity in Cancer (GDSC) dataset obtained from Kaggle. The primary objective is to rank anticancer drugs for individual cancer cell lines based on their predicted LN_IC50 values.
Lower predicted LN_IC50 values indicate greater drug sensitivity and receive higher rankings.

## Methodology

1. Performed Exploratory Data Analysis (EDA) on each dataset to understand its features and data quality.
2. Selected relevant features and merged into a unified dataset.
3. Missing values and duplicate records were handled during preprocessing.
4. Trained four regression models and evaluated:
   - Linear Regression
   - Random Forest
   - Decision Tree
   - Gradient Boosting
5. Model performance was compared using R², Mean Squared Error (MSE), and Mean Absolute Error (MAE).
6. Linear Regression demonstrated the best overall performance and was selected to predict LN_IC50 values.
7. Actual and predicted values, along with prediction errors, were tabulated, and drugs were ranked for each cell line based on predicted LN_IC50 values.
   
## Limitations
- Since random cross-validation was performed at the drug–cell-line observation level, the same drugs and cell lines may appear in both training and validation folds; therefore, the evaluation does not establish generalization to completely unseen drugs or cell lines.
- Drug rankings represent predicted sensitivity in the GDSC cell-line context and cannot be interpreted as clinical treatment recommendations.
## Dataset
Source - https://www.kaggle.com/datasets/samiraalipour/genomics-of-drug-sensitivity-in-cancer-gdsc



