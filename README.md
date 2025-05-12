# A CNN-based Image Classifier for Brain Stroke Detection

## Overview
This project implements a Convolutional Neural Network (CNN) model to classify brain MRI images for stroke detection. It uses a binary classification approach to determine the presence or absence of a stroke in grayscale medical images. The model is trained and evaluated using the publicly available **TEKNO21 Brain Stroke Dataset**.

## Dataset
- **Source**: TEKNO21 Brain Stroke Dataset
- **Type**: Brain MRI images with binary labels (stroke / no stroke)
- **Preprocessing**: Images resized to 128x128, converted to grayscale, and normalized.

## Model Architecture
A simple CNN consisting of:
- Two convolutional layers with ReLU activation and MaxPooling
- Flattened and passed through two fully connected layers
- Dropout regularization to reduce overfitting
- Final output with 2 logits for binary classification

## Training
- **Loss Function**: CrossEntropyLoss
- **Optimizer**: Adam
- **Epochs**: 20
- **Batch Size**: 32

## Evaluation Metrics
Model performance on the validation set:

Accuracy  : 95.12%
Precision : 96.56% (class 1), 92.86% (class 0)
Recall    : 95.49% (class 1), 94.50% (class 0)
F1-Score  : 96.02% (class 1), 93.67% (class 0)
