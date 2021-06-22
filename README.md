# Credit Risk Analysis

Syed Ahmed
June 22, 2021 

## Overview 

This project utilizes various machine learning algorithms to predict credit risk by means of classification. 

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, I will employ different techniques to train and evaluate models with unbalanced classes. Jill, our client, asks us to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I will use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. From here, we can compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

## Results 
