# Credit_Risk_Analysis

## Overview
- The objective of this project was to evaluate models and various sampling techniques to predict credit risk. 
- The Logistic regression model performance was compared when using the follwing sampling algorithms:
  - RandomOverSampler
  - SMOTE
  - ClusterCentroids
  - SMOTTEEN

This was compared to the performance of BalancedRandomForestClassifier and EasyEnsembleClassifier Machine Learning models.

## Results

### Oversampling

RandomOverSampler + LogisticRegression 
![RandomOverSampler + LogisticRegression](https://user-images.githubusercontent.com/76575162/136497392-5a8f5835-4834-41bf-a459-f7f1b47c31f5.png)

SMOTE + LogisticRegression
![SMOTE + LogisticRegression](https://user-images.githubusercontent.com/76575162/136497430-666d4842-3fd1-4489-be97-a500ea60f814.png)


### Undersampling
ClusterCentroids + LogisticRegression
![ClusterCentroids + LogisticRegression](https://user-images.githubusercontent.com/76575162/136497501-03befd4f-af4c-4755-8b94-bb7025f9a465.png)

### Combination (Over and Under Sampling)

SMOTEENN + LogisticRegression
![SMOTEENN + LogisticRegression](https://user-images.githubusercontent.com/76575162/136497549-a6871e6e-637f-4fee-a08e-16c771b6295b.png)

### Ensemble Learners

BlancedRandomForestClassifier
![BlancedRandomForestClassifier](https://user-images.githubusercontent.com/76575162/136497668-7b23c55e-fe8f-44f4-9037-03caca795c9c.png)

EasyEnsembleClassifier
![EasyEnsembleClassifier](https://user-images.githubusercontent.com/76575162/136497699-d3456d09-7a72-468c-9f41-4c6a7247b652.png)

## Summary

It seems that undersampling really reduced the recall and barely scored over 50% for the accuracy score. SMOTTEENN scored a bit better on both metrics, but it seems that if this dataset were to be analyzed using logistic regression, oversampling would be the way to go.

The best way to predict credit risk, however, is to use the EasyEnsembleClassier model which scored much better than every other method tried for this project.

With a balanced accuracy score of 93.17%, 99% precision, and 94% recall, it is extemely successful at predicting credit risk correctly.
