# Residential House Price Prediction

## Project Overview

House price prediction is an important machine learning problem because accurate price estimates can support property valuation and real estate decision-making.

This project uses the Ames Housing dataset to explore the factors associated with residential house prices and eventually build regression models to predict the final sale price of a house.

The current stage of the project focuses on understanding the dataset and performing Exploratory Data Analysis (EDA).

---

## Dataset

The project uses the **House Prices - Advanced Regression Techniques** dataset from Kaggle.

The dataset contains 1,460 residential house records and 79 explanatory features related to property size, quality, location, construction, garage, basement, and other characteristics.

The dataset is publicly available on Kaggle:

https://www.kaggle.com/c/house-prices-advanced-regression-techniques

The main target variable is:

`SalePrice`

---

## Project Objectives

The main objectives of this project are to:

- Understand the structure of the housing dataset
- Investigate data quality and missing values
- Analyze the `SalePrice` target variable
- Apply a log transformation to reduce target skewness
- Explore numerical features and their relationships with house prices
- Explore categorical features and their relationship with house prices
- Prepare the dataset for feature engineering and regression modelling

---

## Project Workflow

The project currently follows this workflow:

1. Import Libraries
2. Load Dataset
3. Initial Data Understanding
4. Data Quality Investigation
5. Target Variable Analysis
6. SalePrice Log Transformation
7. Numerical Feature EDA
8. Categorical Feature EDA
9. Feature Engineering
10. Feature Engineering Validation
11. Train-Test Split
12. Data Preprocessing
13. Regression Model 
14. Model Evaluation
15. Model Comparison
16. Feature Importance Analysis

---

## Data Analysis

The dataset was initially inspected to understand:

- Dataset dimensions
- Column names
- Data types
- Numerical features
- Categorical features
- Summary statistics

Data quality was also investigated by checking:

- Missing values
- Duplicate rows
- Unique values
- Constant columns

---

## Target Variable Analysis

`SalePrice` was analyzed using descriptive statistics, skewness, histograms, and boxplots.

The target variable was found to be right-skewed, with some houses having considerably higher prices than the majority of the dataset.

A log transformation was therefore applied to create:

`LogSalePrice`

This transformation helps produce a more balanced target distribution for regression modelling.

---

## Numerical Feature EDA

Numerical features were explored using:

- Distribution plots
- Skewness analysis
- Correlation analysis
- Correlation heatmaps
- Scatter plots

Important numerical features investigated include:

- `OverallQual`
- `GrLivArea`
- `GarageCars`
- `GarageArea`
- `TotalBsmtSF`
- `1stFlrSF`
- `YearBuilt`

The analysis was used to identify numerical features that have strong relationships with `SalePrice`.

---

## Categorical Feature EDA

Categorical features were analyzed by examining their number of categories and category frequencies.

Important categorical features investigated include:

- `Neighborhood`
- `ExterQual`
- `KitchenQual`
- `GarageType`
- `BsmtQual`
- `Foundation`
- `HeatingQC`

Boxplots were used to compare `SalePrice` across different categories.

This analysis helps identify how characteristics such as neighborhood, construction quality, kitchen quality, and heating quality are associated with differences in house prices.

---

## Current Status

The project has currently completed the initial data understanding and EDA stages.

Completed:

- [x] Dataset loading
- [x] Initial data understanding
- [x] Data quality investigation
- [x] Target variable analysis
- [x] SalePrice log transformation
- [x] Numerical feature EDA
- [x] Categorical feature EDA
- [x] Feature engineering
- [x] Feature engineering validation
- [x] Train-test split
- [x] Data preprocessing
- [x] Regression models
- [x] Model evaluation
- [x] Model comparison
- [x] Feature importance analysis

---

## Project Structure

```text
PricePredict/
│
├── Data/
├── Images/
├── Notebooks/
│   └── PricePredict_Ames_Housing.ipynb
│
├── Outputs/
│   ├── model_comparison.csv
│   ├── feature_importance.csv
│   └── model_predictions.csv
│
├── src/
│   ├── feature_engineering.py
│   ├── preprocessing.py
│   └── modeling.py
|
├── Summary/
│   └── Summary/Residential_house_price_prediction_summary.pdf
├── README.md
|
└── .gitignore