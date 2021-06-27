# Credit Risk Report

## Overview of the loan prediction risk analysis

The purpose of the analysis is to develop credit risk models that specifically handle the unbalanced classes of fraud data. Specifically, sampling techniques are used to make up the different in classes. Random oversampling and SMOTE algorithms are used to oversample, and ClusterCentroids is used to undersample. SMOTEENN is used to do a combination of over and undersampling. Balanced random forest and easy ensemble is used to train models.

## Results

### Random Oversampling

Using random oversampling and passing the data into a logistic regression, a balanced accuracy score of 64.95% is found. The model has a precision of 1% and recall of 73%.

### SMOTE

Using SMOTE oversampling and passing the data into a logistic regression, a balanced accuracy score of 65.84% is found. The model has a precision of 1% and recall of 63%.

### Cluster Centroids

Using Cluster Centroids undersampling and passing the data into a logistic regression, a balanced accuracy score of 54.42% is found. The model has a precision of 1% and recall of 69%.

### SMOTEENN

Using SMOTEENN combination sampling and passing the data into a logistic regression, a balanced accuracy score of 61.57% is found. The model has a precision of 1% and recall of 68%.


### Balanced Random Forest

Using the balanced random forest classifer, a balanced accuracy score of 78.85% is found. The model has a precision of 3% and recall of 70%.

### Easy Ensemble

Using the easy ensemble classifer, a balanced accuracy score of 93.17% is found. The model has a precision of 9% and recall of 92%.

## Summary

There are many ways to handle unbalanced class data in the credit risk world. In this report, three resampling techniques and two classifiers are explored in order to determine which technique gave the best results.

Overall, the resampling techniques with logisitic regression gave poor results in the 55-65% range for balanced accuracy. The ensemble techniques performed much better with balanced accuracy of 70%+.

It is recommended that easy ensemble classifer would be used due it it's better result in balanced accuracy and almost every result in imbalanced classification report. While the precision is poor, the cost of false positive (classifying high risk when load is low risk) is low in credit risk.
