# credit-risk-classification
Module 20 Machine Learning HW

Report:
## Overview of the Analysis

This machine learning analysis will use and compare two techniques to train and evaluate a model based on a borrowers loan risk:

* We will predict whether or not a borrow is a safe bet to offer a healthy loan, based on previous data including: income, number of accounts, total debt, interest rate and the size of the loan.

* 75035 healthy loans and 2500 risk loans were collected for comparison. 

*  Data was split into Training and Testing sets and then fit to a logistic regression model. After saving the predictions for the testing data, the models performance is evaluated by generating a confusion matrix and offering a clasification report.

* The same procedure was followed, but using the balanced accuracy score imported from the RandomOverSampler module from imbalanced-learn.

## Results

Machine Learning Model 1:
  * Accuracy = 99.2%
  * Precision = 100% Predicted healthy loans were healthy, whilst 85% of at-risk loans actually defaulted.
  * Recall = 99% for healthy loans, and 91% for at-risk loans

Machine Learning Model 2:
  * Accuracy = 99.4%
  * Precision = 100% Predicted healthy loans were healthy, whilst 84% of at-risk loans actually defaulted.
  * Recall = 99% for healthy loans, and ALSO 99% for at-risk loans (lower "false negative" rate suggests more "risky" borrowers may be given a chance.)

## Summary

Both models predict loan-risk adequately.

* The logistic regression model, based on the balanced data, predicts the feasibility of loans slightly better than the original. In addition to being 99.4% accurate, it is also satifactorily precise in identifying both high-risk and healthy loans. However, it does predict healthy scores most precisely. The improved recall number suggests that there is less error in identifying additional healthy loans that may have been overlooked in the previous model. 

