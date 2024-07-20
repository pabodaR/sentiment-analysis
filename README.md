# Sentiment Analysis Project

## Table of Contents
1. [Introduction](#introduction)
2. [Project Overview](#project-overview)
3. [Dataset](#dataset)
4. [Data Preprocessing](#data-preprocessing)
5. [Modeling](#modeling)
6. [Evaluation](#evaluation)
7. [Results](#results)

## Introduction
Sentiment analysis is the process of determining whether a piece of text is positive, negative, or neutral. This project aims to classify customer reviews of Alexa products as either positive or negative using machine learning techniques.

## Project Overview
- **Objective:** Predict the sentiment of customer reviews
- **Features:** Data exploration, preprocessing, model selection, evaluation, visualization

## Dataset
- **Source:** https://www.kaggle.com/datasets/ruchawagh/amazon-alexa-dataset/data
- **Description:** This dataset contains customer reviews of Alexa products with columns such as 'rating', 'date', 'variation','verified_reviews', and 'feedback' (target variable: 1 for positive, 0 for negative).

## Data Preprocessing
- Handling missing values
- Handling duplicate values
- Normalization/Standardization
- Feature scaling
- Text preprocessing (lowercasing, removing punctuation, tokenization, stemming)

## Modeling
- Models used: Logistic Regression, Random Forest, Support Vector Machine (SVM)
- The performance of models against train and test sets were compared to select the most suitable model.

## Evaluation
### Metrics: Accuracy

| Model                   | Train Accuracy     | Test Accuracy      |
|-------------------------|--------------------|--------------------|
| Logistic Regression     | 0.9606576629477392 | 0.9192886456908345 |
| Random Forest           | 0.9935408103347034 | 0.9124487004103967 |
| Support Vector Machine  | 0.9841456253669995 | 0.9274965800273598 |

## Results
- **Logistic Regression:** The model performs well in both the training (96.07%) and test (91.93%) sets, showing good generalization with minimal overfitting.
- **Random Forest:** The model achieves near-perfect accuracy on the training set (99.35%) but shows lower performance on the test data (91.24%), indicating overfitting.
- **Support Vector Machine (SVM):** This model performs well on both the training (98.41%) and test (92.75%) sets. It offers a good balance between training and testing accuracy without significant overfitting.

### Conclusion
The Support Vector Machine (SVM) is recommended for this sentiment analysis task. It provides the highest test accuracy (92.75%) with a good balance between training and testing performance, making it a reliable model for predicting sentiment.
