# Customer Churn Prediction

A machine learning project for predicting customer churn using XGBoost.

## Project Overview

This project builds a binary classification model to predict whether a customer is likely to leave the company.

The project covers data preprocessing, categorical feature encoding, model training, cross-validation, hyperparameter tuning, and model evaluation.

## Dataset

The dataset contains customer information such as:

* Credit Score
* Geography
* Gender
* Age
* Tenure
* Balance
* Number of Products
* Activity Status
* Estimated Salary
* Card Type
* Satisfaction Score
* Point Earned

The target variable is `Exited`, where:

* `0` = Customer stayed
* `1` = Customer exited

## Data Cleaning

The `Complain` feature was removed because it showed strong target leakage. Its values were highly correlated with the target variable `Exited`, which could lead to unrealistic model performance.

Therefore, `Complain` was excluded from the features used for training the model.

## Model

**XGBoost Classifier**

The model was evaluated using:

* Accuracy
* Confusion Matrix
* Precision
* Recall
* F1-Score
* ROC-AUC
* Cross-Validation

Hyperparameter tuning was performed using `GridSearchCV`.

## Technologies

* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* Jupyter Notebook

## Project Files

* `Customer_Churn_Prediction.ipynb` — Complete machine learning workflow
* `Customer-Churn-Records.csv` — Dataset
