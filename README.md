# CIFAR-10 Image Classification using Convolutional Neural Networks (CNN)

## Overview

This project implements a Convolutional Neural Network (CNN) using TensorFlow/Keras to classify images from the CIFAR-10 dataset. The model is trained to recognize ten different object categories and demonstrates the use of deep learning techniques for image classification.

## Dataset

The project uses the CIFAR-10 dataset, which consists of 60,000 color images of size 32×32 pixels distributed across 10 classes:

* Airplane
* Automobile
* Bird
* Cat
* Deer
* Dog
* Frog
* Horse
* Ship
* Truck

The dataset contains:

* Training Images: 50,000
* Testing Images: 10,000
* Classes: 10
* Image Size: 32 × 32 × 3 (RGB)

## Model Architecture

The CNN architecture consists of:

1. Convolution Layer (32 filters, 3×3, ReLU)
2. Max Pooling Layer (2×2)
3. Convolution Layer (64 filters, 3×3, ReLU)
4. Max Pooling Layer (2×2)
5. Convolution Layer (128 filters, 3×3, ReLU)
6. Flatten Layer
7. Dense Layer (128 neurons, ReLU)
8. Dropout Layer (0.5)
9. Output Layer (10 neurons, Softmax)

## Training Configuration

| Parameter        | Value                    |
| ---------------- | ------------------------ |
| Optimizer        | Adam                     |
| Loss Function    | Categorical Crossentropy |
| Epochs           | 10                       |
| Batch Size       | 64                       |
| Validation Split | 20%                      |

## Preprocessing

* Pixel values normalized to range [0, 1]
* Labels converted to one-hot encoded vectors
* Dataset automatically loaded from TensorFlow Keras

## Evaluation Metrics

The model is evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* Classification Report

## Results

Example performance obtained from the notebook:

| Metric    | Score |
| --------- | ----- |
| Accuracy  | 71%   |
| Precision | 71%   |
| Recall    | 71%   |
| F1-Score  | 71%   |

### Class-wise Highlights

* Best performing classes: Automobile, Ship, Truck
* Challenging classes: Cat, Dog, Bird
* Strong recall observed for Frog and Ship categories

## Visualizations

The notebook generates:

* Sample dataset images
* Class distribution plot
* Training vs Validation Accuracy graph
* Training vs Validation Loss graph
* Confusion Matrix
* Feature Maps from Convolutional Layers

## Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

## Running the Project

## Installation

```bash
pip install -r requirements.txt
```

## Running the Project

Open the notebook in Google Colab or Jupyter Notebook and execute all cells sequentially.

```bash
jupyter notebook
```

or upload the notebook to Google Colab.

## Learning Outcomes

* Understanding CNN architecture design
* Image preprocessing and normalization
* Model training and validation
* Performance evaluation using classification metrics
* Visualization of convolutional feature maps
