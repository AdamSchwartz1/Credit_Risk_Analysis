# Credit_Risk_Analysis

## Overview
The purpose of this analysis was to analyze credit risk records and use various supervised machine learning techniques to find a model that would best fit this data. Credit risk is an inherently unbalanced classification problem because there are a lot more good loans over risky loans. I will use a number of resampling methods to try and best fit this data.

Applications used: Python, pandas, imbalanced-learn, scikit-learn, jupyter notebook, and github

## Results
In this analysis, we did 6 different tests - 4 resampling methods and 2 ensemble methods. The resampling methods were Random Oversampling, SMOTE oversampling, Cluster Centroids for undersampling, and SMOTEENN for combination sampling. The ensemble methods were Balanced Random Forest Classifier and Easy Ensemble Classifier.

I generated an accuracy score, confusion matrix, and classification report for all of these tests to compare with each other. I will look at the accuracy score, recall, and precision for high risk items because that's what's being resampled and analyzed for model comparisson. 

|                                   | Accuracy | Recall | Precision |
|-----------------------------------|----------|--------|-----------|
| Naive Random Oversampling         |    64%   |   .66  |    .01    |
| SMOTE Oversampling                |    65%   |   .61  |    .01    |
| Cluster Centroid Undersampling    |    54%   |   .69  |    .01    |
| SMOTEENN Combo Sampling           |    64%   |   .70  |    .01    |
| Balanced Random Forest Classifier |    76%   |   .62  |    .03    |
| Easy Ensemble AdaBoost Classifier |    93%   |   .92  |    .09    |

Below are the results for each model.

### Random Oversampling
<img width="668" alt="random_oversample" src="https://user-images.githubusercontent.com/90946252/151725998-e7b3b4d4-cf81-4f50-aefc-9dd4796c5987.png">

### SMOTE Oversampling
<img width="671" alt="SMOTE_oversampling" src="https://user-images.githubusercontent.com/90946252/151726079-10139e7a-8698-4b68-b289-7d75f78b12f4.png">

### Cluster Centroids Undersampling
<img width="660" alt="cluster_centroid" src="https://user-images.githubusercontent.com/90946252/151726145-296b3411-1052-4902-9f02-8b2028eb3d32.png">

### SMOTEENN Combo Sampling
<img width="668" alt="SMOTEENN_combo" src="https://user-images.githubusercontent.com/90946252/151726112-612a68fe-9867-47b7-89bd-bcc153949164.png">

### Balanced Random Forest Classifier
<img width="667" alt="random_forest" src="https://user-images.githubusercontent.com/90946252/151726022-d8395df5-df89-4ae7-b16c-5096c81b2678.png">

### Easy Ensemble Classifier
<img width="666" alt="easy_ensemble" src="https://user-images.githubusercontent.com/90946252/151726037-1f142911-7133-4be5-8a26-69446c1b7751.png">

## Summary
Recall is most important because We want to limit false negatives which states it's predicted low risk, but is actually high risk. Precision isn't as important because if you have a false positive (predicted high risk but is actually low rise), you can run more tests to determine that it isn't. 
