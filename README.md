# Handwritten Digit Classification with PyTorch

This repository contains the implementation of a handwritten digit classifier using the MNIST dataset. The project focuses on exploring different techniques to build, train, and evaluate a neural network.

## Overview

The project uses a fully connected neural network to classify digits (0–9) from the MNIST dataset. It includes key stages of machine learning workflows such as data preprocessing, model training, evaluation, and visualization. Additionally, it explores potential improvements like data augmentation and visualization of network weights and activations.

---

## Key Features

### 1. **Data Preprocessing**
- The pixel values of the MNIST dataset are normalized to the [0, 1] range for better model performance.
- Augmentation techniques like random rotations and affine transformations are explored but not applied in the final model to maintain comparability.

### 2. **Model Architecture**
- A fully connected neural network with the following structure:
  - Input Layer: Flattens the 28x28 image into a vector.
  - Hidden Layers: Two layers with ReLU activations (32 and 16 neurons).
  - Output Layer: Maps the input to 10 classes representing the digits.

### 3. **Training and Evaluation**
- Trained using CrossEntropyLoss and the Adam optimizer.
- Achieved **96% accuracy on the test set** without data augmentation.

### 4. **Visualizations**
- **Prediction Confidence**: Displays test samples with predicted labels and confidence scores to identify both correct and incorrect predictions.
- **Weight Visualizations**: Visualizes the weights of the first hidden layer to interpret the learned features.

### 5. **Model Improvements**
- Discusses potential enhancements:
  - Switching to a convolutional neural network (CNN) for better feature extraction.
  - Hyperparameter tuning for further optimization.
  - Revisiting data augmentation to explore its impact on model generalization.

This repository serves as a hands-on project to explore fundamental concepts in neural networks and practical techniques for debugging and improving models.
