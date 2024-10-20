# Convolutional Neural Network on MNIST Dataset

### Project Overview

This project involves building and training a convolutional neural network (CNN) using Keras to classify hand-written digits from the MNIST dataset. This is a multiclass classification problem where the goal is to correctly identify the digit (0-9) based on a 28x28 grayscale image of the digit. 

### Dataset

This project works with the MNIST dataset which is a collection of images used for handwriting recognition. It contains labeled images of handwritten digits from 0 to 9. Each example corresponds to one hand-written image. The features will be comprised of numerical vectors (an n-dimensional array) that contain grey-scale pixel values that range from 0 to 255.

### Model Structure

- Input Layer: Accepts 28x28x1 grayscale images.
- Convolutional Layers: Four layers with increasing filter sizes (16, 32, 62, 128).
- Pooling Layer: Global average pooling used for dimensionality reduction.
- Output Layer: 10 units corresponding to the 10 possible digit classes.

### Results

The trained CNN achieved the following results:
- Loss: 0.1269
- Accuracy: 95.96%