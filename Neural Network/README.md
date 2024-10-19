# Neural Network Model

### Project Overview

This project involves building and training a feedforward neural network using Keras for binary classification. The model predicts whether an Airbnb host is a 'super host' based on various features in the Airbnb dataset.

### Dataset

The dataset used is airbnbData_train.csv, which is a preprocessed version of the Airbnb NYC listings dataset. It includes:
- One-hot encoding of categorical variables
- Scaling of numerical variables
- Impuation of missing values

The target variable is host_is_superhost, a binary classification where True represents super hosts and False represents non-super hosts.

### Model Architecture

- Input Layer: 1 layer with input shape equal to the number of features
- Hidden Layers: 3 layers with 64, 32, 16 units respectively, usig ReLU activation
- Output Layer: 1 layer with 1 unit and sigmoid activation for binary classification

### Results

Confusion Matrix (Initial Model):
- True Positives: 4854
- True Negatives: 907
- False Positives: 794
- False Negatives: 451

### Performance Tuning

#### Adjusting Layers:
- Adding a fourth hidden layer with 8 units improved true negatives but reduced true positives.
- Adding a fifth hidden layer with 4 units resulted in higher true positives but more false positives.
The original architecture had a more balanced performance.

#### Epochs Tuning:
- With epochs=50: Slightly worse than 100 epochs but ran faster.
- With epochs=20: Significantly faster but resulted in worse performance, showing the importance of tuning the number of epochs.