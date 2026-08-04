# CIFAR-10 Dataset Information

## Description

CIFAR-10 is a widely used benchmark dataset for image classification tasks in machine learning and deep learning. It contains 60,000 color images divided into 10 object categories.

The dataset was developed by researchers at the Canadian Institute for Advanced Research (CIFAR).

## Dataset Statistics

| Attribute         | Value          |
| ----------------- | -------------- |
| Total Images      | 60,000         |
| Training Images   | 50,000         |
| Testing Images    | 10,000         |
| Number of Classes | 10             |
| Images per Class  | 6,000          |
| Image Resolution  | 32 × 32 pixels |
| Channels          | 3 (RGB)        |

## Classes

| Label | Class      |
| ----- | ---------- |
| 0     | Airplane   |
| 1     | Automobile |
| 2     | Bird       |
| 3     | Cat        |
| 4     | Deer       |
| 5     | Dog        |
| 6     | Frog       |
| 7     | Horse      |
| 8     | Ship       |
| 9     | Truck      |

## Data Distribution

Each class contains:

* 5,000 training images
* 1,000 testing images

This makes the dataset balanced across all categories.

## Sample Applications

CIFAR-10 is commonly used for:

* Image Classification
* Convolutional Neural Network Research
* Deep Learning Education
* Transfer Learning Experiments
* Computer Vision Benchmarking

## Dataset Loading

In this project, the dataset is loaded directly from TensorFlow Keras:

```python
from tensorflow.keras.datasets import cifar10

(X_train, y_train), (X_test, y_test) = cifar10.load_data()
```

## Preprocessing Applied

The following preprocessing steps were performed:

1. Pixel normalization:

   * Convert image values from 0–255 to 0–1

2. Label encoding:

   * Convert integer labels into one-hot encoded vectors

3. Train-validation split:

   * 20% of training data used for validation during training

## Source

Official TensorFlow Dataset:

https://www.tensorflow.org/api_docs/python/tf/keras/datasets/cifar10
