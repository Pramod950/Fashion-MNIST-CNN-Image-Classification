# Fashion-MNIST-CNN-Image-Classification

## Project Overview

This project builds a Convolutional Neural Network (CNN) model to classify fashion product images from the Fashion MNIST dataset into 10 different categories. The model uses data augmentation, dropout, and early stopping to improve performance and reduce overfitting.

## Problem Statement

Develop a deep learning model that can accurately classify clothing images into their respective categories using the Fashion MNIST dataset.

## Dataset Information

* Dataset: Fashion MNIST
* Training Samples: 60,000
* Test Samples: 10,000
* Image Size: 28 × 28 pixels
* Channels: 1 (Grayscale)
* Number of Classes: 10

## Classes

* T-shirt/Top
* Trouser
* Pullover
* Dress
* Coat
* Sandal
* Shirt
* Sneaker
* Bag
* Ankle Boot

## Data Preprocessing

* Normalized pixel values from 0-255 to 0-1
* Used 20% of training data for validation
* Applied data augmentation to improve generalization

## Data Augmentation

* Rotation: ±10°
* Horizontal Flip
* Zoom: 10%

## CNN Architecture

* Conv2D (32 Filters, 3×3, ReLU)
* MaxPooling2D (2×2)
* Conv2D (64 Filters, 3×3, ReLU)
* MaxPooling2D (2×2)
* Flatten Layer
* Dense Layer (128 Units, ReLU)
* Dropout (0.5)
* Output Layer (10 Units, Softmax)

## Model Training

* Optimizer: Adam
* Loss Function: Sparse Categorical Crossentropy
* Batch Size: 32
* Epochs: 20
* Validation Split: 20%
* Early Stopping: Enabled

## Model Performance

* Test Accuracy: 85.63%
* Training and Validation Accuracy remained close
* No significant overfitting observed

## Key Findings

* CNN successfully classified fashion images with good accuracy.
* Data augmentation improved model generalization.
* Dropout reduced overfitting.
* Similar classes such as Shirt, T-shirt/Top, and Pullover were harder to distinguish.

## Future Improvements

* Add Batch Normalization layers
* Increase model depth with additional CNN layers
* Tune hyperparameters
* Apply model quantization for mobile deployment

## Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib
* Scikit-learn

## Conclusion

This project demonstrates the use of Convolutional Neural Networks (CNNs) for image classification. The model achieved 85.63% test accuracy and showed good generalization through the use of data augmentation, dropout, and early stopping.
