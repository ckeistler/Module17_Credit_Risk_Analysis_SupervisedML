# Credit_Risk_Analysis

## Overview
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we need to employ different techniques to train and evaluate models with unbalanced classes.
  
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

## Results

#### Results by Machine Learning Model
  
  - RandomOverSampler: 
  
        Accuracy: 65.16%  
        high_risk: 1% Precision, 62% Recall, F1 0.02
        low_risk: 100% Precision, 68% Recall, F1 0.81
        
![ROS](https://user-images.githubusercontent.com/88443672/148702436-f7999479-c3f7-485c-adb7-cb7b3a975035.png)

  - SMOTE: 
  
        Accuracy: 62.42% 
        high_risk: 1% Precision, 59% Recall, F1 0.02
        low_risk: 100% Precision, 66% Recall, F1 0.80
        
![smote](https://user-images.githubusercontent.com/88443672/148702450-33e73106-3ac3-44ed-a5fb-334a1aaea584.png)

  - ClusterCentroids: 
        
        Accuracy: 62.42% Accuracy
        high_risk: 1% Precision, 60% Recall, F1 0.01
        low_risk: 100% Precision, 43% Recall, F1 0.60
        
![cc](https://user-images.githubusercontent.com/88443672/148702457-9aef8113-79b7-453c-a0a7-ccb6b8dd7dd3.png)

  - SMOTEENN: 
       
        Accuracy: 51.60%
        high_risk: 1% Precision, 70% Recall, F1 0.02
        low_risk: 100% Precision, 58% Recall, F1 0.73
        
 ![smoteenn](https://user-images.githubusercontent.com/88443672/148702422-ca9a4379-2d7d-47a9-9a3e-b8f9e5a680ad.png)
 
  - BalancedRandomForestClassifier: 
        
        Accuracy: 78.78%
        high_risk: 4% Precision, 67% Recall, F1 0.07
        low_risk: 100% Precision, 91% Recall, F1 0.95
        
 ![rfc1](https://user-images.githubusercontent.com/88443672/148701859-78c6d873-a634-4d9a-b803-9039bf9fe0f5.png)
 ![rfc](https://user-images.githubusercontent.com/88443672/148701878-ace53fcb-8f82-4956-9dd3-e8a7413f2d08.png)

  - EasyEnsembleClassifier: 
        
        Accuracy: 92.47%
        high_risk: 7% Precision, 91% Recall, F1 0.14
        low_risk: 100% Precision, 94% Recall, F1 0.97
        
 ![eec](https://user-images.githubusercontent.com/88443672/148701855-78b92631-91b1-4a02-8d2e-8c0be37fb260.png)

  
## Summary
