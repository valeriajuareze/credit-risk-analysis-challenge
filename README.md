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

1.  The balanced accuracy score is 66%
2.  The High risk precision is only 1% and the recall is 80%
3.  The Low risk precision is 100% and the recall is 53%

![image](https://user-images.githubusercontent.com/108365182/200338100-9907cedc-2bda-41d9-ac3e-c3ea3f58f41c.png)


- **Balanced Random Forest Classifier:** 

1.  The balanced accuracy score is 78%
2.  The High risk precision is 3% and the recall is 70%
3.  The Low risk precision is 100% and the recall is 87%

![image](https://user-images.githubusercontent.com/108365182/200336989-50b25851-17ec-48de-8561-efdcc09c0bfa.png)

- **Easy Ensemble AdaBoost Classifier:** 

1.  The balanced accuracy score is 93%
2.  The High risk precision is 9% and the recall is 92%
3.  The Low risk precision is 100% and the recall is 94%

![image](https://user-images.githubusercontent.com/108365182/200337440-83c916fc-ccb2-48be-b8f4-63c77ec50b36.png)

## Summary

In brief, all model´s results to predict high risk candidates are the following ones:


**1. Naive Random OverSampling:** 65% accuracy score, 1% precision, 65% recall

**2. SMOTE OverSampling:** 66% accuracy score, 1%  precision, 63% recall

**3. Undersampling:** 54% accuracy score, 1%  precision, 69% recall

**4. Combination (Over & Under) Sampling::** 66% accuracy score, 1%  precision, 80% recall

**5. Balanced Random Forest Classifier:** 78% accuracy score, 3%  precision, 70% recall

**6. Easy Ensemble AdaBoost Classifier:** 93% accuracy score, 9%  precision, 92% recall

Based on our previous results, my recommendation is to use the Easy Ensemble AdaBoost Classifier. It has an accuracy score of 93% which is much higher than the other ones. Also, the precision of 9% and the recall of 92% are the highest rates. Therefore, this model will be the best choice to predict credit risk. 

