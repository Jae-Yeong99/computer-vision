Cats vs Dogs Classification

This project implements an image classification model to distinguish between cats and dogs using PyTorch.

Goal: Classify input images as Cat (0) or Dog (1)

Dataset: Kaggle tongpython/cat-and-dog

Framework: PyTorch

Model: Custom Convolutional Neural Network (CNN) without using pretraind model

Metric: Accuracy

1. Data Loading & Preprocessing

Custom CatDogDataset class (PyTorch Dataset)

Transformations applied:

Resize → 128x128

Convert to Tensor

Normalize → (0.5, 0.5, 0.5)

2. Model Architecture

A custom CNN built with:

Multiple Conv2D + ReLU + MaxPool layers

Fully Connected (Linear) layers

Sigmoid activation for binary classification

3. Training

Optimizer: Adam

Loss Function: Binary CrossEntropy

Device: Supports GPU (cuda) if available

Training Loop: Epoch-based training with progress tracking

4. Evaluation

Evaluate performance on the test set

Compute accuracy

Visualize sample predictions vs. ground truth
