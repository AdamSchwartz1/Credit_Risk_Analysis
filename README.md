# Credit_Risk_Analysis

## Overview
The purpose of this analysis was to analyze credit risk records and use various supervised machine learning techniques to find a model that would best fit this data. Credit risk is an inherently unbalanced classification problem because there are a lot more good loans over risky loans. I will use a number of resampling methods to try and best fit this data.

Applications used: Python, pandas, imbalanced-learn, scikit-learn, jupyter notebook, and github

## Results
In this analysis, we did 6 different tests - 4 resampling methods and 2 ensemble methods. The resampling methods were Random Oversampling, SMOTE oversampling, Cluster Centroids for undersampling, and SMOTEENN for combination sampling. The ensemble methods were Balanced Random Forest Classifier and Easy Ensemble Classifier.

I generated an accuracy score, confusion matrix, and classification report for all of these tests to compare with each other. I will look at high risk items for the classification report because that's what's being resampled and analyzed. 



## Summary
Recall is most important because We want to limit false negatives which states it's predicted low risk, but is actually high risk. Precision isn't as important because if you have a false positive (predicted high risk but is actually low rise), you can run more tests to determine that it isn't. 