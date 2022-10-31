# Credit Risk Analysis

## Overview of the Project

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, I’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asked me to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once I´m done, I’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results 

- **Naive Random OverSampling:** 

1.  The balanced accuracy score is almost 65%
2.  The High risk precision is only 1% and the recall is 65%
3.  The Low risk precision is 100% and the recall is 64%
 
![image](https://user-images.githubusercontent.com/108365182/199050442-3afbacac-7689-4d3c-bd6d-a4ffd80d7dbf.png)


- **SMOTE Oversampling:** 

1.  The balanced accuracy score is 66%
2.  The High risk precision is only 1% and the recall is 63%
3.  The Low risk precision is 100% and the recall is 69%

![image](https://user-images.githubusercontent.com/108365182/199050231-14518d4d-bf4c-4d20-b6d1-e16c85914876.png)

- **Undersampling:** 

1.  The balanced accuracy score is 54%
2.  The High risk precision is only 1% and the recall is 69%
3.  The Low risk precision is 100% and the recall is 40%

![image](https://user-images.githubusercontent.com/108365182/199050971-ce84ebc6-b7a8-4508-8f74-bc721a9cf77d.png)

- **Combination (Over & Under) Sampling:** 

1.  The balanced accuracy score is 54%
2.  The High risk precision is only 1% and the recall is 69%
3.  The Low risk precision is 100% and the recall is 40%

(Same results as the undersampling model)

![image](https://user-images.githubusercontent.com/108365182/199051701-52fe5678-4028-4452-bbe1-cf16c7ed76d3.png)

