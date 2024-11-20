# Binary Tumor Classifier with Deep Learning
This repository contains a binary tumor classifier for the Kaggle ISIC 2024 competition, which distinguishes between benign and malignant tumors using images. The project is designed to serve as both a learning resource and a functional model, incorporating detailed explanations of the methodology and technical approaches.

Overview
The primary goal of this project is to:

Develop a baseline model achieving at least 70% accuracy.
Refine the model to achieve over 95% accuracy through iterative improvements.
The dataset used is a subset of the ISIC Archive containing fewer than 400 labeled images (malignant or benign), along with a metadata CSV file.

Key Features
In this project, you will learn how to:

Prepare image classification metadata from a CSV file.
Use data augmentation techniques to address data scarcity.
Build a CustomDataset class and manage DataLoaders for training and validation.
Train a neural network using PyTorch to classify tumors with high accuracy.
Dataset
The ISIC dataset is available at: ISIC Archive.

Preprocessing Steps:
Metadata Preparation:
The CSV file includes labels for each image (malignant or benign).
Data Augmentation:
Techniques such as flipping, rotating, and cropping are applied to expand the dataset and improve generalization.
Model Architecture
The baseline model is built using PyTorch and follows this architecture:

Convolutional Neural Network (CNN) backbone for feature extraction.
Fully connected layers for binary classification.
Further architectural enhancements include:

Use of pretrained models (e.g., ResNet or EfficientNet).
Optimization through hyperparameter tuning and advanced loss functions.
Training and Evaluation
Training:
Data is split into Training and Validation sets.
The model is trained using:
Cross-Entropy Loss as the loss function.
Adam Optimizer for adaptive learning rates.
Evaluation:
Metrics:
Accuracy: Ensures baseline goal (≥ 70%) is achieved.
Precision, Recall, and F1-Score: Assess the model's robustness.
A confusion matrix is used to evaluate predictions.
