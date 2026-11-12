# Ames Housing Price Prediction

## Overview
This project develops a Linear Regression model to predict residential house prices using the Ames Housing dataset.

The main objective is to build a comprehensive regression pipeline that transforms raw housing data into model-ready features and predicts property sale prices.

**Target Variable:** `SalePrice`

## Dataset
The project uses the Kaggle House Prices dataset, which contains residential property characteristics, including:

- Building and property features
- Overall quality and condition
- Location and neighborhood information
- Garage and basement characteristics
- Construction and renovation details

## Methodology

The project covers the following stages:

1. Exploratory Data Analysis and Train-Test Split
2. Identification of Uninformative Features
3. Outlier Detection and Removal
   - Z-score
   - IQR
   - Modified Z-score
   - Isolation Forest
   - Local Outlier Factor (LOF)
   - DBSCAN
4. Missing Value Imputation
   - Median and mode imputation
   - KNN Imputation
5. Feature Engineering
6. Categorical Feature Encoding
   - Ordinal Encoding
   - One-Hot Encoding
   - Target Encoding
7. Sparse Feature Analysis
8. Feature Scaling
   - StandardScaler
   - RobustScaler
   - MinMaxScaler
   - PowerTransformer
9. Feature Selection and Multicollinearity Analysis
10. Linear Regression Model Training
11. Model Evaluation

## Model
**Algorithm:** Linear Regression

The target variable (`SalePrice`) is log-transformed using `log1p()` during training. Predictions are converted back to the original price scale using `expm1()`.

## Evaluation Metrics
- R² Score
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)

Both training and test performance are evaluated.

## Technologies
Python, Pandas, NumPy, Scikit-learn, SciPy, Matplotlib

## Project Structure
- `house-price-prediction.ipynb` — Complete preprocessing, feature engineering, model development and evaluation pipeline.
- `house_price_train.csv` — Training dataset.
