# ML Model Comparison: Decision Trees vs KNN on Airbnb Dataset

### Project Overview

This project explores and compares two machine learning models: Decision Trees (DT) and K-Nearest Neighbors (KNN). The goal is to predict whether an Airbnb host is a 'super host' based on a variety of features from the Airbnb NYC "listings" dataset. This project is part of a machine learning lab where we experiment with various hyperparameters to find the best performing model.

### Dataset

We use a preprocessed version of the Airbnb NYC "listings" dataset, which includes the following steps:
- Handling missing values and outliers
- Removing unstructured fields

The dataset contains 28,022 rows and 43 columns, with the target variable being host_is_superhost (a binary classification problem).

### Results

- The best performing model was a Decision Tree with a max_depth of 8, achieving an accuracy of 83.4%.
- The best performing KNN model used k=22 and the Manhattan distance metric, achieving an accuracy of 78.0%.