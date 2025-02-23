## Classification Model Training and Evaluation For Loan approval 

## Problem Statement
Traditional loan approval processes suffer from inefficiencies, human biases, and inconsistencies that undermine fairness and trust. Manual processes are time-consuming and often lead to inaccuracies, resulting in financial exclusion or high default rates.

## Overview
This project focuses on developing a machine learning-based loan classification system to assist financial institutions in predicting the likelihood of loan approval. Traditional loan approval processes are often inefficient, prone to human bias, and time-consuming. By leveraging supervised machine learning algorithms, this system will analyze key features such as income, etc… to provide accurate and fair predictions.

## Challenges
The accuracy and almost all the metrics were too perfect , for the first sight, it looks like overfiting however the lost were high, that push me to see the data frame from the start and i found out that it were an inbalanced data , 10000 comparing to 35000 , this almost the four times , I used the ADASYN (Adaptive Synthetic Sampling) algorithm to balance the data.


## Dataset
The project utilized public datasets from Kaggle’s loan classification dataset.
Source: https://www.kaggle.com/code/youssefelbadry10/loan-approval-classification-eda-ml

## Objectives
1. Preprocess the dataset containing key loan application features.
2. Develop and train a supervised machine learning model with at least 90% accuracy.
3. Test and validate the system’s effectiveness.

## the video demo link: https://drive.google.com/file/d/1L4ZV4tlrEsNnrDCLymxNgJvWMGlOIHXN/view?usp=sharing


## Table Overview
Neural Networks (NNs) and a Machine Learning (ML) algorithm (Logistic Regression) were evaluated to determine the best classification model. Various NN architectures were tested with different optimizers (SGD, RMSprop, Adam) and regularization techniques (L1, L2, Dropout). The results showed that Optimized_NN_Adam achieved the highest accuracy (93.64%) and F1 score (0.9378), demonstrating that the Adam optimizer provided better generalization. NN_RMSprop followed closely with similar performance, while regularization techniques slightly balanced recall and precision without significantly improving accuracy. Logistic Regression performed well (91.00% accuracy), proving its effectiveness but falling short compared to deep learning models.

The comparison revealed that Neural Networks outperformed Logistic Regression, as they captured more complex patterns in the data. While ML models like Logistic Regression can still be effective for simpler tasks, deep learning approaches—especially with the right optimization techniques—achieved superior results. Among all models, Adam optimization proved to be the most effective choice, highlighting its ability to improve convergence and performance. Regularization and dropout techniques influenced recall and precision but were secondary to optimizer selection in determining overall accuracy.

## the output:
0 is denied
1 is approved

## 📝 Summary Table
| Model Name                      | Regularization Technique | Optimizer | Early Stopping  | Dropout Rate | Learning Rate | Test Accuracy | F1 Score   | Recall     | Precision  |
| ------------------------------- | ------------------------ | --------- | --------------- | ------------ | ------------- | ------------- | ---------- | ---------- | ---------- |
| Logistic Regression             | None                     | N/A       | None            | None         | None          | **91.00%**    | **0.91**   | **0.91**   | **0.91**   |
| Optimized_NN_Adam               | None                     | Default   | None            | None         | Default       | **93.64%**    | **0.9378** | **0.9352** | **0.9402** |
| NN_SGD                          | None                     | SGD       | Val Loss (p=5)  | None         | 0.01          | **90.19%**    | **0.9068** | **0.9314** | **0.8834** |
| NN_RMSprop                      | None                     | RMSprop   | Val Loss (p=5)  | None         | 0.002         | **93.46%**    | **0.9365** | **0.9416** | **0.9315** |
| NN_RMSprop_L1_Regularization    | L1 Regularization        | RMSprop   | Val Loss (p=5)  | None         | Default       | **91.45%**    | **0.9180** | **0.9340** | **0.9025** |
| NN_Dropout                      | None                     | SGD       | Val Loss (p=5)  | 0.2          | 0.001         | **90.20%**    | **0.9071** | **0.9340** | **0.8817** |
| NN_L2_Regularization            | L2 Regularization        | SGD       | Val Loss (p=5)  | None         | 0.001         | **90.79%**    | **0.9117** | **0.9277** | **0.8962** |

