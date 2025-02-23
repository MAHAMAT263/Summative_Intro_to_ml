## Classification Model Training and Evaluation For Loan approval 

## Problem Statement
Traditional loan approval processes suffer from inefficiencies, human biases, and inconsistencies that undermine fairness and trust. Manual processes are time-consuming and often lead to inaccuracies, resulting in financial exclusion or high default rates.

## Overview
This project focuses on developing a machine learning-based loan classification system to assist financial institutions in predicting the likelihood of loan approval. Traditional loan approval processes are often inefficient, prone to human bias, and time-consuming. By leveraging supervised machine learning algorithms, this system will analyze key features such as income, etc… to provide accurate and fair predictions.


## Dataset
The project utilized public datasets from Kaggle’s loan classification dataset.
Source: https://www.kaggle.com/code/youssefelbadry10/loan-approval-classification-eda-ml

## Objectives
1. Preprocess the dataset containing key loan application features.
2. Develop and train a supervised machine learning model with at least 90% accuracy.
3. Test and validate the system’s effectiveness.




## 📝 Summary Table
| Model Name                      | Regularization Technique | Optimizer | Early Stopping | Dropout Rate | learning rate   | | Test Accuracy | F1 Score   | Recall     | Precision  |
| ------------------------------- | ------------------------ | --------- | -------------- | ------------ | --------------- | | ------------- | ---------- | ---------- | ---------- |
| Logistic Regression             | None                     | N/A       | None           | None         | None            | | **91.00%**    | **0.91**   | **0.91**   | **0.91**   |
| Optimized\_NN\_Adam             | None                     | default   | None           | None         | None            | | **93.64%**    | **0.9378** | **0.9352** | **0.9402** |
| NN\_SGD                         | None                     | SGD       | val_loss p=5   | None         | 0,001           | | **90.19%**    | **0.9068** | **0.9314** | **0.8834** |
| NN\_RMSprop                     | None                     | RMSprop   | val_loss p=5   | None         | 0,001           | | **93.46%**    | **0.9365** | **0.9416** | **0.9315** |
| NN\_RMSprop\_L1\_Regularization | L1 Regularization        | RMSprop   | val_loss p=5   | None         | 0,001           | | **91.45%**    | **0.9180** | **0.9340** | **0.9025** |
| NN\_Dropout                     | None                     | SGD       | val_loss p=5   | 0.2          | 0,001           | | **90.20%**    | **0.9071** | **0.9340** | **0.8817** |
| NN\_L2\_Regularization          | L2 Regularization        | SGD       | val_loss p=5   | None         | 0,001           | | **90.79%**    | **0.9117** | **0.9277** | **0.8962** |
