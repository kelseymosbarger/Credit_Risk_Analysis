# Credit_Risk_Analysis
Module 17 - Machine Learning

## Overview of Analysis

Using machine learning, this assignment builds classification models to predict an applicant's credit risk and categorize it as high or low credit risk. This project will evaluate and train six different machine learning models and whether or not they can accurately predict credit risk.

## Results

#### Naive Random Oversampling 
Randomly selects the minority class to add to the training set until it is balanced with the majority class.

- Balanced Accuracy Score : 63.7% credit risk model prediction accuracy
- Precision: High Risk(1%) and Low Risk(100%) classification prediction accuracy
- Recall: High Risk(70%) and Low Risk(57%) classification accuracy

#### SMOTE Oversampling 
Synthetic minority oversampling thechnique (SMOTE), increases related classes and scales them with the increase in the minority class to be a new value.

- Balanced Accuracy Score : 63.0% credit risk model prediction accuracy
- Precision: High Risk(1%) and Low Risk(100%) classification prediction accuracy
- Recall: High Risk(70%) and Low Risk(57%) classification accuracy


#### Undersampling
Decreases the Majority class to balance with the minority class.

- Balanced Accuracy Score : 51.0% credit risk model prediction accuracy
- Precision: High Risk(1%) and Low Risk(100%) classification prediction accuracy
- Recall: High Risk(70%) and Low Risk(57%) classification accuracy


#### Combination Sampling
Increases the Minority class while removing outlier in the majority class

- Balanced Accuracy Score : 63.8% credit risk model prediction accuracy
- Precision: High Risk(1%) and Low Risk(100%) classification prediction accuracy
- Recall: High Risk(70%) and Low Risk(57%) classification accuracy


#### Balanced Random Forest Classifier
using decision trees, the minority class is over sampled

- Balanced Accuracy Score : 78.8% credit risk model prediction accuracy
- Precision: High Risk(4%) and Low Risk(100%) classification prediction accuracy
- Recall: High Risk(67%) and Low Risk(91%) classification accuracy

#### Easy Ensemble AdaBoost Classifier
Adaboost trians the model to recognize errors, and assign additional weight to the errors in each iteration until the error is smaller

- Balanced Accuracy Score : 92.5% credit risk model prediction accuracy
- Precision: High Risk(7%) and Low Risk(100%) classification prediction accuracy
- Recall: High Risk(91%) and Low Risk(94%) classification accuracy



## Summary

Resampling is not as accurate as the ensemble methods. In this instace, the best model to use is the Easy Ensemble AdaBoost Classifier, as it outshines each of the other models in every category. One thing to be aware of before relying soley on this model to analyze credit risk is that there is a possibility that you will recieve a false positive for "high risk" predictions. With an accuracy score of 92.5% I would say it is worth rolling out as the 7.5% of the model that is not accurate will reject low risk clients as it classified them as high risk.

