# Deep Learning Specialization Projects

Hands-on projects from the [Deep Learning Specialization](https://www.deeplearning.ai/courses/deep-learning-specialization/) by DeepLearning.AI on Coursera.

Each course has its own folder. The project in each folder applies that course's ideas to a dataset outside the course. These projects do not include the course's graded assignment solutions.

## Progress

| Course | Topic | Project | Status |
|---|---|---|---|
| 1 | Neural Networks and Deep Learning | [Neural network from scratch (NumPy) for breast cancer classification](course-1-neural-networks-and-deep-learning/) | Done |
| 2 | Improving Deep Neural Networks | Regularization, optimizers and hyperparameter tuning on the Course 1 project | Planned |
| 3 | Structuring Machine Learning Projects | Dev set, precision/recall and error analysis on the same project | Planned |
| 4 | Convolutional Neural Networks | Image classification project | Planned |
| 5 | Sequence Models | Wind turbine wind speed forecasting | Planned |

## Course 1 at a glance

A neural network written with only NumPy that predicts whether a tumor is malignant or benign.

- Forward propagation, binary cross-entropy cost, backpropagation and gradient descent implemented by hand
- Backpropagation checked against a numerical gradient
- Compared network sizes and learning rates
- Compared with scikit-learn's Logistic Regression: 95.6% test accuracy for the network vs 98.2% for the baseline. On this small dataset the simple model did at least as well.

Full details are in the [Course 1 folder](course-1-neural-networks-and-deep-learning/).

## Setup

```
pip install -r requirements.txt
jupyter notebook
```

Later courses may need extra libraries (for example TensorFlow). Each course folder will say so.

## Author

Pallavi Kaushik
