# Learning Model Report

## Overview

The goal of this analysis is to predict the success of charity applications using a neural network model. The model classifies applications as either successful (1) or unsuccessful (0) based on various features provided in the dataset. The target variable for this classification task is IS_SUCCESSFUL, with values of 1 and 0. The features for the model include all columns except IS_SUCCESSFUL, with EIN and NAME being removed as they do not contribute to the model’s predictions.

## Results

Neurons, Layers, and Activation Functions:

-Input Layer: Preprocessed numerical and encoded categorical data
-Hidden Layer 1: 80 neurons with ReLU activation
-Hidden Layer 2: 30 neurons with ReLU activation
-Output Layer: 1 neuron with Sigmoid activation

Model Performance:

-Training Accuracy: ~74%
-Validation Accuracy: ~72-73%

## Summary

The neural network model achieved a training accuracy of 74% and a validation accuracy between 72-73%. While these results are reasonable, they do not significantly exceed baseline expectations. To enhance the model's performance, several improvements were made during the training process. The data was standardized using StandardScaler, and infrequent values in the APPLICATION_TYPE and CLASSIFICATION columns were grouped as "Other" to reduce noise. Additionally, the model was trained for 100 epochs to ensure sufficient learning. Despite these efforts, the current model could still benefit from alternative approaches. Perhaps a Random Forest classifier could be a more suitable choice, as it handles imbalanced data more effectively and captures feature interactions better.