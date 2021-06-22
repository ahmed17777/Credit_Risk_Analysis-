# Credit Risk Analysis

Syed Ahmed
June 22, 2021 

## Overview 

This project utilizes various machine learning algorithms to predict credit risk by means of classification. 

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, I will employ different techniques to train and evaluate models with unbalanced classes. Jill, our client, asks us to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I will use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. From here, we can compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

## Resources 
All data used in analysis is from LoanStats_2019Q1.csv

## Results 

The following are the training and target variables used: 

![1](https://user-images.githubusercontent.com/45697471/123008811-9349ce00-d389-11eb-8128-d092ee4b24e1.png)


### Oversampling 

In this section, I will compare two oversampling algorithms to determine which algorithm results in the best performance. I will oversample the data using the naive random oversampling algorithm and the SMOTE algorithm. For each algorithm, I will follow the following steps:

- View the count of the target classes using Counter from the collections library.
- Use the resampled data to train a logistic regression model.
- Calculate the balanced accuracy score from sklearn.metrics.
- Print the confusion matrix from sklearn.metrics.
- Generate a classication report using the imbalanced_classification_report from imbalanced-learn.
- Use a random state of 1 for each sampling algorithm to ensure consistency between tests

![2](https://user-images.githubusercontent.com/45697471/123008821-96dd5500-d389-11eb-9383-fd296c8d78a3.png)


![3](https://user-images.githubusercontent.com/45697471/123008852-a8bef800-d389-11eb-912c-fdd1a7887010.png)


### Undersampling 

In this section, I will test an undersampling algorithms to determine which algorithm results in the best performance compared to the oversampling algorithms above. I will undersample the data using the Cluster Centroids algorithm and complete the folliowing steps:

- View the count of the target classes using Counter from the collections library.
- Use the resampled data to train a logistic regression model.
- Calculate the balanced accuracy score from sklearn.metrics.
- Print the confusion matrix from sklearn.metrics.
- Generate a classication report using the imbalanced_classification_report from imbalanced-learn.
- Use a random state of 1 for each sampling algorithm to ensure consistency between tests

![4](https://user-images.githubusercontent.com/45697471/123008875-b70d1400-d389-11eb-8d7a-1b5ba237e5d2.png)


### Combination Sampling 

In this section, I will test a combination over- and under-sampling algorithm to determine if the algorithm results in the best performance compared to the other sampling algorithms above.  For each algorithm, I will:

- Train the model using the training data.
- Calculate the balanced accuracy score from sklearn.metrics.
- Print the confusion matrix from sklearn.metrics.
- Generate a classication report using the imbalanced_classification_report from imbalanced-learn.
- For the Balanced Random Forest Classifier onely, print the feature importance sorted in descending order (most important feature to least important) along with the feature score
- Use a random state of 1 for each algorithm to ensure consistency between tests

![5](https://user-images.githubusercontent.com/45697471/123008895-c4c29980-d389-11eb-9041-36fe32c74ac7.png)


### Ensemble Learners 

In this section, I will compare two ensemble algorithms to determine which algorithm results in the best performance. I will train a Balanced Random Forest Classifier and an Easy Ensemble AdaBoost classifier . For each algorithm, I will follow these steps: 

- Train the model using the training data.
- Calculate the balanced accuracy score from sklearn.metrics.
- Print the confusion matrix from sklearn.metrics.
- Generate a classication report using the imbalanced_classification_report from imbalanced-learn.
- For the Balanced Random Forest Classifier onely, print the feature importance sorted in descending order (most important feature to least important) along with the feature score
- Use a random state of 1 for each algorithm to ensure consistency between tests


![6](https://user-images.githubusercontent.com/45697471/123008908-c9874d80-d389-11eb-9042-6e8ef5561815.png)


![7](https://user-images.githubusercontent.com/45697471/123008914-cc823e00-d389-11eb-9009-4cc904eeac67.png)
