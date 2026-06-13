# Insurance Premium Prediction

## Overview

This project predicts the recommended insurance premium amount for customers based on demographic, policy, and health-related attributes using Machine Learning techniques.

The objective is to build a regression model that helps insurance companies estimate suitable premium values by analyzing customer information and policy characteristics.

---

## Problem Statement

Insurance providers need accurate premium estimation to balance risk and profitability. Manual premium calculation can be time-consuming and inconsistent.

This project uses historical customer data to develop a predictive model that estimates the recommended insurance premium automatically.

---

## Dataset Features

The dataset contains customer and policy-related information including:

* Upper Age
* Lower Age
* Reco Insurance Type
* Accomodation Type
* Is Spouse
* City Code
* Health Indicator
* Holding Policy Duration
* Holding Policy Type

### Target Variable

* Reco_Policy_Premium

---

## Project Workflow

### 1. Data Loading and Exploration

* Loaded insurance dataset
* Examined dataset structure
* Checked data types
* Identified missing values
* Generated descriptive statistics

### 2. Exploratory Data Analysis

* Distribution analysis of premium values
* Histogram and boxplot visualization
* Correlation analysis
* Feature-target relationship analysis
* Detection of outliers and skewness

### 3. Data Preprocessing

* Missing value handling
* Conversion of problematic values such as "14+"
* Categorical feature encoding
* Frequency encoding for City_Code
* Numerical feature transformation

### 4. Feature Engineering

Created additional features such as:

* age_gap = Upper_Age - Lower_Age
* is_joint_policy

These engineered features improved model performance and interpretability.

### 5. Model Building

The following regression models were trained and compared:

* Linear Regression
* Ridge Regression
* Random Forest Regressor
* Gradient Boosting Regressor

### 6. Hyperparameter Tuning

* GridSearchCV was used for model optimization.
* Multiple parameter combinations were evaluated to identify the best-performing model.

### 7. Model Evaluation

Evaluation metrics used:

* R² Score
* RMSE (Root Mean Squared Error)
* MAE (Mean Absolute Error)

---

## Final Results

| Metric   | Value   |
| -------- | ------- |
| RMSE     | 2785.59 |
| MAE      | 2265.15 |
| R² Score | 0.8135  |

The model explains approximately 81% of the variance in insurance premium values, demonstrating strong predictive performance.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab

---

## Machine Learning Concepts Applied

* Data Cleaning
* Exploratory Data Analysis
* Feature Engineering
* Categorical Encoding
* Regression Modeling
* Hyperparameter Tuning
* Model Evaluation
* Feature Importance Analysis

---

## Future Improvements

* XGBoost implementation
* LightGBM implementation
* SHAP explainability analysis
* Advanced feature engineering
* Automated model selection

---

## Author

Chada Jayasen Reddy

B.Tech in Computer Science and Engineering

Kakatiya Institute of Technology and Science, Warangal
