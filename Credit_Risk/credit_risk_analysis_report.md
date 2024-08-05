# Credit Risk Analysis Report

## Overview

The purpose of this analysis was to develop and evaluate a machine learning model to assess credit risk for loan applications. By utilizing logistic regression, the aim was to predict whether a loan would be classified as a healthy loan (0) or a high-risk loan (1) based on various financial and personal factors of the applicants. This model could potentially assist the company in making more informed lending decisions and managing risk effectively.

## Model Performance Metrics

* Accuracy: 0.99
  - The model correctly predicted the loan status for 99% of all cases in the test set.

* Precision:
  - Healthy loans (0): 1.00
  - High-risk loans (1): 0.87
  - The model is extremely precise in identifying healthy loans and reasonably precise for high-risk loans.

* Recall:
  - Healthy loans (0): 1.00
  - High-risk loans (1): 0.89
  - The model effectively identifies almost all healthy loans and a high proportion of high-risk loans.

* F1-score:
  - Healthy loans (0): 1.00
  - High-risk loans (1): 0.88
  - The F1-score, which balances precision and recall, is perfect for healthy loans and strong for high-risk loans.

## Summary and Recommendation

The logistic regression model demonstrates excellent performance in predicting both healthy and high-risk loans. With an overall accuracy of 99%, it provides highly reliable results for the majority of cases.

For healthy loans, the model shows perfect precision, recall, and F1-score (all 1.00). This means it correctly identifies all healthy loans without any false positives.

For high-risk loans, the model performs well, though not perfectly. With a precision of 0.87, it correctly identifies high-risk loans 87% of the time when it predicts a high-risk status. The recall of 0.89 indicates that it captures 89% of all actual high-risk loans in the dataset.

Given these results, I strongly recommend the use of this model by the company for credit risk assessment. The model's strengths include:

1. Excellent overall accuracy
2. Perfect prediction of healthy loans
3. Strong performance in identifying high-risk loans

The model's ability to correctly identify healthy loans without error is particularly valuable, as it can help the company confidently approve low-risk applications. While the performance on high-risk loans is not perfect, it still provides a significant improvement over random guessing and could be a valuable tool in flagging potentially problematic applications for further review.

However, it's important to note that about 11% of high-risk loans might be missed (false negatives), and about 13% of loans flagged as high-risk might actually be healthy (false positives). Therefore, I recommend using this model as part of a broader decision-making process, possibly in conjunction with other assessment methods or human review for borderline cases.

In conclusion, this logistic regression model provides a robust foundation for credit risk assessment and can significantly enhance the company's loan approval process and risk management strategies.
