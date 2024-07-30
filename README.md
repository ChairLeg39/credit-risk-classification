# credit-risk-classification
KU Boot Camp Module 20 Challenge

## Overview

The purpose of this analysis was to develop and evaluate a machine learning model to assess credit risk for loan applications. By utilizing logistic regression, the aim was to predict whether a loan would be classified as a healthy loan (0) or a high-risk loan (1) based on various financial and personal factors of the applicants. This model could potentially assist the company in making more informed lending decisions and managing risk effectively.

## Requirements

1. Data Preparation
2. Model Creation and Training
3. Model Evaluation
4. Performance Analysis

## Methodology

### 1. Data Preparation
- Read lending_data.csv into a Pandas DataFrame
- Create labels (y) from "loan_status" column
- Create features (X) from remaining columns
- Split data into training and testing sets using train_test_split

### 2. Model Creation and Training
- Initialize logistic regression model
- Fit model using training data (X_train and y_train)

### 3. Model Evaluation
- Generate predictions using testing feature data (X_test)
- Create confusion matrix
- Generate classification report

### 4. Performance Analysis
- Analyze model's predictive capability for healthy loans (0) and high-risk loans (1)
- Interpret confusion matrix and classification report metrics
- Assess overall model performance and potential applications

## Findings

For healthy loans (0), the model performs exceptionally well in predicting healthy loans. Both precision and recall are 1.00, indicating perfect performance for this class. This means the model correctly identifies almost all healthy loans and has very few false positives.

For high-risk loans (1), the model's performance is good but not perfect for high-risk loans. Precision of 0.87 means that when the model predicts a loan is high-risk, it's correct 87% of the time. Recall of 0.89 indicates that the model correctly identifies 89% of all actual high-risk loans. The F1-score of 0.88 shows a good balance between precision and recall for this class.

The overall accuracy of 0.99 is very high, indicating that the model correctly classifies 99% of all loans. The macro average F1-score of 0.94 shows good performance across both classes. The weighted average F1-score of 0.99 reflects the model's strong overall performance, considering class imbalance.

For a more detailed analysis, please view the `credit_risk_analysis_report.md`.


