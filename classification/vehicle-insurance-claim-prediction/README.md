# Vehicle Insurance Claim Prediction

## Overview
This project uses Logistic Regression to predict whether a vehicle insurance policyholder will file an insurance claim (`claim_status`).

The objective is to build a binary classification model that identifies potential claims based on customer, vehicle, and policy-related features.

## Dataset
The dataset contains 40,000 records and 39 predictive features, including:
- Customer information
- Vehicle characteristics
- Insurance policy details
- Regional attributes

**Target variable:** `claim_status` (0 = No Claim, 1 = Claim)

## Methodology
The project covers the following steps:

1. Exploratory Data Analysis (EDA)
2. Missing Value Handling and Data Preprocessing
3. Categorical Encoding and Feature Scaling
4. Class Imbalance Handling
5. Feature Selection
6. Logistic Regression Model Training
7. Model Evaluation on Test and Out-of-Time (OOT) datasets
8. Feature Importance Analysis

## Evaluation Metrics
- ROC-AUC
- Precision
- Recall (Sensitivity)
- Specificity
- Confusion Matrix
- Classification Report

## Technologies
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Imbalanced-learn

## Project Structure
- `logistic-regression.ipynb` — Model development and evaluation
- `vehicle-insurance-data.csv` — Dataset
