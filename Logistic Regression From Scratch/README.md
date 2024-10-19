# Logistic Regression from Scratch

### Project Overview

In this project, I implemented logistic regression from scratch using Python, without relying on libraries like scikit-learn for model training. The goal was to gain a deeper understanding of how logistic regression works by coding the model and its optimization algorithm (gradient descent) manually.

I benchmarked the custom implementation against scikit-learn's built-in logistic regression and compared the results, including the fitted weights, intercept, and execution speed.

### Dataset

I used the Airbnb NYC listings dataset, which has been preprocessed to include one-hot encoding for categorical variables, scaling for numerical variables, and imputation of missing values.

Label: host_is_superhost (whether the host is a super host, binary classification problem).
Features:
- review_scores_rating
- review_scores_cleanliness
- review_scores_checkin
- review_scores_communication
- review_scores_value
 host_response_rate
- host_acceptance_rate

### Results

#### Weights and Intercepts

The fitted weights and intercept from both my implementation and scikit-learn's logistic regression model were very similar.

My Implementation:
- Weights: [0.5669, 0.4923, 0.2016, 0.2555, -0.0059, 1.7159, 0.2648]
- Intercept: -1.8291
  
Scikit-learn Implementation:
- Weights: [0.5669, 0.4922, 0.2015, 0.2556, -0.0059, 1.7159, 0.2648]
- Intercept: -1.8291

#### Runtime Comparison

- My Implementation: ~33 ms per loop
- Scikit-learn Implementation: ~101 ms per loop
