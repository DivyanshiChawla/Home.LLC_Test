# Home Price Prediction Model

This project analyzes the factors influencing home prices over the past 20 years using various machine learning models.

## Overview

The model uses economic indicators and housing market data from 2003 to 2023 to predict and analyze home prices. It employs Linear Regression, XGBoost, and Random Forest algorithms to understand the relationships between different features and home prices.

## Features

The model considers the following features:
- Home Prices (target variable)
- Mortgage Rate
- Unemployment Rate
- Income
- Consumer Price Index (CPI)
- Gross Domestic Product (GDP)
- Real Mortgage Rate
- GDP per Capita
- Affordability Index

## Model Performance

1. Linear Regression:
   - MAE: 4.18
   - R-squared: 0.83
   - Cross-validation MAE: 3.64

2. XGBoost:
   - MAE: 0.50
   - R-squared: 0.99
   - Cross-validation MAE: 0.54

3. Random Forest:
   - MAE: 4.96
   - R-squared: 0.19

XGBoost outperforms the other models with the lowest MAE and highest R-squared value.

## Key Findings

1. Feature Importance:
   - CPI is the most important feature in both XGBoost and Random Forest models.
   - Unemployment Rate is the second most important feature in both models.
   - Other significant features include GDP, Income, and Mortgage Rate.

2. Correlation Analysis:
   - Home Prices show strong positive correlations with Income (0.88), CPI (0.86), and GDP (0.87).
   - There's a strong negative correlation between Home Prices and GDP per Capita (-0.88).
   - Unemployment Rate has a moderate negative correlation (-0.55) with Home Prices.

3. Model Predictions:
   - The XGBoost model shows the best fit between actual and predicted home prices.
   - Linear Regression and Random Forest models show more scattered predictions.

4. Residual Analysis:
   - XGBoost residuals are more tightly clustered around zero, indicating better performance.
   - Linear Regression and Random Forest models show larger residuals, especially for higher home prices.

## Conclusions

The analysis suggests that economic indicators, particularly CPI and unemployment rate, play crucial roles in determining home prices. The strong performance of the XGBoost model indicates that there are complex, non-linear relationships between the features and home prices. Future work could focus on feature engineering and exploring additional economic indicators to improve prediction accuracy.
