## Overview

The project implements a Convolutional Neural Network (CNN) to classify different types of motor bearing faults based on statistical features. The model achieves high accuracy in distinguishing between normal operation and various fault conditions including ball faults, inner race (IR) faults, and outer race (OR) faults with different severity levels.

## Dataset

The dataset consists of various time-domain features extracted from vibration signals:
- `max`, `min`, `mean`, `rms`, `skewness`, `kurtosis`, `crest`, `form`
- Target variable: `fault` (10 different classes including Normal and various fault types)

## Features

- Exploratory Data Analysis (EDA) of motor fault data
- Feature correlation analysis and selection
- Data preprocessing with standardization
- Implementation of a CNN classifier
- Model evaluation with confusion matrix and classification reports
- Model saving and prediction functionality

## Requirements

Dependencies are listed in requirements.txt and include:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- torch (PyTorch)

## Usage

1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run the notebook lab.ipynb to train and evaluate the model
4. Use the provided functions to make predictions with new data

## Model Architecture

The implemented CNN architecture includes:
- Multiple convolutional layers with batch normalization
- Adaptive average pooling
- Fully connected layers with dropout for regularization
- 128-64-10 neuron configuration in the classifier part

## Performance

The model achieves high classification accuracy and can reliably distinguish between different fault types, making it suitable for predictive maintenance applications in industrial settings.
