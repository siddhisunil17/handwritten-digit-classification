# Handwritten-Digit-Classification
A classification pipeline for handwritten digit recognition using the MNIST dataset.

Overview

This project focuses on classifying handwritten digits from the MNIST dataset using various machine learning models. The goal is to evaluate different models, optimize performance, and deploy the best-performing model for real-world applications.

Features

1. Data Preprocessing: Standardization, normalization, and feature engineering.
2. Model Training: Implementation of multiple classifiers including Logistic Regression, Ridge Classifier, Random Forest, and XGBoost.
3. Performance Evaluation: Comparison based on Accuracy, F1-Score, Precision, and Recall.
4. Dimensionality Reduction: Principal Component Analysis (PCA) for feature compression.
5. Robustness Testing: Evaluation on noisy data to assess real-world applicability.
6. Deployment Readiness: Selection of the best model for future production use.

Dataset

The MNIST dataset consists of 70,000 grayscale images of handwritten digits (0-9), each of size 28x28 pixels.
1. Training Set: 60,000 images
2. Test Set: 10,000 images
Dataset Source: http://yann.lecun.com/exdb/mnist/

Installation

To set up the project locally, follow these steps:
1. Clone the repository
2. Install dependencies
3. Run model training and evaluation

Results Summary

The result document summarizes the performance of the models based on Accuracy, F1-Score (Test), Cross-Validation Mean F1-Score, and Standard Deviation.
Random Forest emerged as the best-performing model with the highest accuracy and F1-Score, indicating its robustness for this task.

Observations

1. Logistic Regression achieved an average accuracy of ~93%, making it a reliable linear classifier for this task.
2. Ridge Classifier showed lower accuracy (~85%) compared to Logistic Regression and Random Forest, indicating its limited performance for high-dimensional data like MNIST.
3. Random Forest significantly outperformed other models with an accuracy of ~99.86% and an F1-Score of 0.9985. Its hyperparameter tuning helped achieve optimal results.
4. Cross-validation results for Random Forest indicate consistent performance with minimal variance.

Conclusion

Based on the results, Random Forest is selected as the final deployment model due to its superior performance metrics. Its ability to handle high-dimensional data and deliver near-perfect classification accuracy makes it the ideal choice for this task.

Deployment Recommendation

Based on the results of original, PCA-reduced, and noisy data evaluations:
1. Random Forest is the recommended model for deployment due to its excellent performance across all tested scenarios.
2. XGBoost is also a viable option, offering similar performance with the ability to handle high-dimensional and noisy data efficiently.
3. Logistic Regression remains a reasonable choice when computational efficiency is a priority.

References

MNIST Dataset: http://yann.lecun.com/exdb/mnist/
Scikit-learn: https://scikit-learn.org/


