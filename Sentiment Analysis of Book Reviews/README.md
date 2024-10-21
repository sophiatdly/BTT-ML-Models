# Sentiment Analysis on Book Reviews

### Project Overview

This project implements a feedforward neural network using Keras for sentiment classification of Amazon book reviews. The network is designed to predict whether a book review is positie or negative, utilizing TF-IDF vectorizer to convert text into numerical features.

### Dataset

The dataset used is a collection of Amazon book reviews stored in bookReviews.csv and contains the following columns:
- Review: The text of the book review.
- Positve Review: A binary label where 1 indicates a positive revieww and 0 indicates a negative review.

### Model Architecture

The neural network has the following architecture
- Input layer: Corresponding to the vocabulary size of the TF-IDF vectorizer.
- Hidden Layers: 3 hidden layers with 64, 32, and 16 units with ReLU activation, respectively.
- Dropout Layers: Dropout regularization is applied after each hidden layer to prevent overfitting.
- Output Layer: A single unit with sigmoid activation for binary classification.

### Training

- The model was trained using Stochastic Gradient Descent (SGD) as the optimizer with a learning rate of 0.5.
- Binary cross-entropy was used as the loss function, and accuracy was used as the evaluation metric.
- Early stopping was applied by monitoring the validation loss.
- Number of epochs: 40 epochs were used to train the model with an 80/20 split for training and validation.

Training was performed on the vectorized text data, and dropout regularization was applied to prevent overfitting.

### Results

- Loss: 0.4697
- Accuracy: 81.87%
- ROC AUC Score: 0.9114
