# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis was to use various techniques to train and evaluate a model based on loan risk. We used a CSV file which contained historical lending activity from a peer-to-peer lending services company. The model is being used to identify the creditworthiness of borrowers. The target column that we were trying to predict is the "loan_status" column. We used LogisticRegression which is a classification algorithm and then used RandomOverSampler which over-samples the minority class(es) by picking samples at random with replacement. 

## Results

Machine Learning Model 1:
  - In the first model, we split the data in training and testing sets and then fitted the trainig data to our model. We then used the test data to make predictions and compared those predictions to the rest of the test data.
    - Accuracy: 95%
    - Precision: Healthy Loan precision is 100%, while High-Risk-Loan precision is 85%.
    - Recall scores: Healthy Loan recall score is 99%, while High-Risk-Loan recall score is 91%.



Machine Learning Model 2:
  - In the second model, we started by utilizing RandomOverSampler which randomly duplicated examples from the minority class (High-Risk-Loan). We then applied it to the training data and fitted it to our model using LogisticRegression. We then used the test data to make predictions and compared those predictions to the rest of the test data.
    - Accuracy: 99%
    - Precision: Healthy Loan precision is 99% and High-Risk-Loan precision is 99%.
    - Recall scores: Healthy Loan recall score is 99% and High-Risk-Loan recall score is 99%.

## Summary

It appears that the model works best when we utilize RandomOverSampler to resample the data before testing and training it using LogisticRegression. We can tell it works best due to the difference in accuracy. The first model yielded an accuracy percentage of 95% while the second model yielded an accuracy percentage of 99%. I do believe performance can depend on the problem we aim to solve, simply because using this data you run the risk of having false positives and false negatives. That can skew the data and not give a super accurate predictions. Out of the two models, I would recommend the resampling first. Although, it would be wise to compare the second model to other machine learning models, just to see if other models can be more effective than the one we tested. 

