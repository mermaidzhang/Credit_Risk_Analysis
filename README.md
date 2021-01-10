# Credit_Risk_Analysis

## Overview 

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes.

In this report, I will used RndomOversampler, and SMOTE to oversample the data; and undersample the data using ClusterCentroids. Then,a combination of both over and undersampling approcach were conducted using SMOTEENN. 

BalanceRandomForestClassifier and EasyEnsembleClassifier were used to reduce bias then predict the creadit risk. Lastly, recommendations were made on all approaches were used. 

## Results 


### Naïve Random Oversampling

With the “Random Oversampling” method, the accuracy score is 0.65.  For high risk applications, precision is 0.01, recall is 0.74, and  f1 score is 0.02.  For low risks, precision is 1.00, recall is 0.55, and f1 score is 0.71.

### SMOTE

With the “SMOTE” method, the accuracy score is 0.66.  For high risk applications, precision is 0.01, recall is 0.63, and f1 score is 0.02.  For low risks, precision is 1.00, recall is 0.69, and f1 score is 0.82.


### Cluster Centroid 
With the “Cluster Centroid” method, the accuracy is 0.54.  For high risk applications, precision is 0.01, recall is 0.67, and f1 score is 0.01.  For low risks, precision is 1.00, recall is 0.42, and f1 score is 0.58.

### Combination (Over and Under) 
With the “Combination (Over and Under)” method, specifically the SMOTEENN, the accuracy is 0.64.  For high risk applications, precision is 0.01, recall is 0.70, and f1 score is 0.02.  For low risks, precision is 1.00, recall is 0.58, and f1 score is 0.73.

### Balanced Random Forest
With the “Balanced Random Forest” method, the accuracy is 0.79.  For high risk applications, precision is 0.03, recall is 0.70, and f1 score is 0.06.  For low risks, precision is 1.00, recall is 0.87, and f1 score is 0.93.

### Easy Ensemble Classifier
With the “Easy Ensemble Classifier” method, the accuracy is 0.93.  For high risk applications, precision is 0.09, recall is 0.92, and f1 score is 0.16.  For low risks, precision is 1.00, recall is 0.94, and f1 score is 0.97.


## Summary & Reommendations 

The accuracy score for Naïve Random Oversampling, SMOTE and Cluster Centroid were all in the range of 54-65%.  The precision for high risk from all models were very low but the precision for low risk from all model were 1.00. Hence, those three models were not suitable as the high rsk percisions were low. The Easy Ensemble Classifier approach has highest accuracy among all models, with 0.93.  The precision for this model is low with 0.09 and the balanced random forest only had 0.04. Lastly,  Easy Ensemble Classifier is recommended to predict the most accure data. 
