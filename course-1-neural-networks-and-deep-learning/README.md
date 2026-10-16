# Course 1: Neural Network from Scratch on Breast Cancer Data

**Course:** Neural Networks and Deep Learning (DeepLearning.AI, Coursera)
**Certificate:** https://coursera.org/verify/EAC2740W0DH9

## Problem
Predict whether a tumor is **malignant** or **benign** from 30 measurements (radius, texture, area, and so on), using a neural network written with only NumPy.

## Dataset
Breast Cancer Wisconsin dataset, loaded from scikit-learn (569 samples, 30 features). No download needed.

## What the notebook does
1. Splits the data 80/20 and scales the features (scaler fitted on training data only)
2. Implements forward propagation, binary cross-entropy cost, backpropagation and gradient descent
3. Checks backpropagation against a numerical gradient
4. Trains a `[30, 8, 1]` network and compares five architectures and four learning rates
5. Compares with scikit-learn's Logistic Regression
6. Evaluates with a confusion matrix

## Results

| Model | Train accuracy | Test accuracy |
|---|---|---|
| Neural network `[30, 8, 1]` | 99.6% | 95.6% |
| scikit-learn Logistic Regression | 98.9% | 98.2% |

- More hidden units or layers did not improve test accuracy (all between 95.6% and 96.5%).
- Learning rate `0.001` was too slow; `0.1` and `0.5` trained well.
- The test set has 114 samples, so the gap between models is about 3 patients and should not be over-read.

## What I learned
_Write 2-3 sentences in your own words here. For example: what changed when you tried different hidden units or learning rates, and what surprised you._

## How to run
1. From the repo root: `pip install -r requirements.txt`
2. Open `neural_network_breast_cancer.ipynb` in Jupyter or Google Colab
3. Run all cells

## Tools
Python, NumPy, pandas, Matplotlib, scikit-learn (used only for the data, scaling and baseline)
