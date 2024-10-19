# Logistic Regression Evaluation

### Project Overview

This project demonstrates the evaluation phase of the machine learning life cycle using logistic regression to solve a binary classification problem. The dataset is used from Airbnb, and the goal is to predict whether an Airbnb host is a 'super host'.

### Dataset

The dataset used is airbnbData_train.csv, which is a preprocessed version of the Airbnb NYC listings dataset. It includes:
- One-hot encoding of categorical variables
- Scaling of numerical variables
- Impuation of missing values

The target variable is host_is_superhost, a binary classification where True represents super hosts and False represents non-super hosts.

### Results

- Default Logistic Regression Model: AUC of 0.76
- Optimized Logistic Regression Model (with C=10000): AUC of 0.82
- Model with Feature Selection (Top 5 Features): AUC of 0.81
- Best Model with All Features: AUC of 0.82