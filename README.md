# credit-risk-classification
Learning supervised machine learning

## Overview of the Analysis

  We are using machine learning to help create a system that will help banks decide who they will give loans to, and any risks they run by giving individuals a large loan.
  The information we fed to the model includes the size of the loan, the interest rate, the borrower income, the debt to income ration of the borrower, the number of their accounts, any derogatory marks, their total debt, and the status of their loan as a label. The focus of all of this, is to make a machine learning model that can accurately and consistently predeict whether an individual should be loaned a set amount, or if they run a high risk of defaulting on the loan. To do this, we are using a logistical regression model.

## Results

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

              precision    recall  f1-score   support

           0       1.00      1.00      1.00     15001
           1       0.86      0.91      0.88       507

    accuracy                           0.99     15508
   macro avg       0.93      0.95      0.94     15508
weighted avg       0.99      0.99      0.99     15508



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

              precision    recall  f1-score   support

           0       1.00      0.99      1.00     15001
           1       0.85      0.99      0.92       507

    accuracy                           0.99     15508
   macro avg       0.93      0.99      0.96     15508
weighted avg       1.00      0.99      0.99     15508

## Summary


Model 2 seems to be the better of the models. We can tell becuase its recall and f1 scores are higher for '1' which scored very poorly in the first model due to the lack of sampling. 

In this model, it's clear that we should focus on the results for '0'. This would mean we are focused on determining if a loan is healthy. Because the results are binary, we need to focus on our more accurate condition (0). Now we have a perfectly precise model to ensure we do not classify a high-risk loan as a healthy one.