# Ensemble Models

### Project Overview

This project explores different regression models to predict the price of Airbnb listings. It focuses on both individual and ensemble models to compare their performances using Root Mean Squared Error (RMSE) and R² (coefficient of determination).

### Dataset

This project uses a preprocessed version of the Airbnb NYC listings dataset (airbnbData_train.csv). This includes:
- One-hot encoding of categorical variables
- Scaling of numerical variables
- Imputation of missing values

The target value is price, which represents the listing price for an Airbnb, which is a continuous variable for the regression task.

### Results

- Stacking              RMSE: 12.35	    R²: 0.78
- Linear Regression	    RMSE: 15.65	    R²: 0.72
- Decision Tree	        RMSE: 13.80	    R²: 0.75
- GBDT	                RMSE: 12.15	    R²: 0.80
- Random Forest	        RMSE: 11.85	    R²: 0.82

### Analysis

- Best Performing Model: The Random Forest model achieved the lowest RMSE (11.85) and the highest R² (0.82), indicating the best performance.
- Ensemble Models vs Individual Models: Ensemble models (Stacking, GBDT, and RF) generally performed better than individual models (Linear Regression, Decision Tree). Random Forest outperformed the other models in terms of both accuracy and predictive power.
