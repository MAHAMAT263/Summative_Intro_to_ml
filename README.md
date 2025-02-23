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
| Model Name                      | Regularization Technique | Optimizer | Early Stopping | Dropout Rate | Test Accuracy | F1 Score   | Recall     | Precision  |
| ------------------------------- | ------------------------ | --------- | -------------- | ------------ | ------------- | ---------- | ---------- | ---------- |
| Logistic Regression             | None                     | N/A       | None           | None         | **91.00%**    | **0.91**   | **0.91**   | **0.91**   |
| Optimized\_NN\_Adam             | None                     | Adam      | **Yes**        | None         | **93.72%**    | **0.9381** | **0.9288** | **0.9476** |
| NN\_SGD                         | None                     | SGD       | **Yes**        | None         | **90.80%**    | **0.9124** | **0.9355** | **0.8905** |
| NN\_RMSprop                     | None                     | RMSprop   | **Yes**        | None         | **93.38%**    | **0.9356** | **0.9380** | **0.9331** |
| NN\_RMSprop\_L1\_Regularization | L1 Regularization        | RMSprop   | **Yes**        | None         | **90.82%**    | **0.9141** | **0.9537** | **0.8777** |
| NN\_Dropout                     | None                     | SGD       | **Yes**        | 0.2          | **90.64%**    | **0.9110** | **0.9355** | **0.8878** |
| NN\_L2\_Regularization          | L2 Regularization        | SGD       | **Yes**        | None         | **91.03%**    | **0.9143** | **0.9340** | **0.8954** |
