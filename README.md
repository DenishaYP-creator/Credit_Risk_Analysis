# Credit_Risk_Analysis

## Overview of the analysis: 
In this project, we the Scikit learn, imbalanced libraries, and a credit card dataset from LendingClub, a peer-to-peer lending services company to build, train and evaluate varios Machine Learning models. The ML techniques used in this project helped to solve for unbalanced risk classification in our LendingClub credit card dataset.

**The deliverables for this Challenge are as follows:**
- Deliverable 1: Use Resampling Models to Predict Credit Risk (File Upload credit_risk_resampling.ipynb file)
- Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk (File Upload credit_risk_resampling.ipynb file)
- Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk (File Upload credit_risk_ensemble.ipynb file.)
- Deliverable 4: A Written Report on the Credit Risk Analysis (README.md)


## Results:  Performance Machine Learning model. 
Each models was evaluted to determine the following: 
- **Balance Accurancy Score:**
Average Number of recalled/predictions each model got right.  High accurancy score yeild greater score of accurancy when making predictions. 
- **Precision Score:**
Number of correct positive predicted observations compared to the total number of positive predicted observations. High precision score yeild a low false positive rate. 
- **Recall Score:**
Number of correct positive predicted observations compared to the number of positive predicted observations in a class. High recall score yeild a low false positive rate.



**Note:

Machine Learning Model | Balanced Accuracy Score| Precision Score| Recall Score
------------ | -------------  | ------------- | -------------
Naive Random Oversampling| 0.59 | 0.99|  0.53
SMOTE Oversampling | 0.61 | 0.99| 0.66
Undersampling | 0.50 | 0.99| 0.45
Combination (Over and Under) Sampling | 0.57 | 0.99| 0.51
Balanced Random Forest Classifier | 0.79 |  0.99 |  0.91 
Easy Ensemble AdaBoost Classifier | 0.92 | 0.99 | 0.94 

<hr> </hr>



## Summary: 
#### Recommendation: 
In the Balanced Random Forest Classifier, multiples decision trees are fitted into a forest tree with weak learning trees. It then trains the model against a small subset of the initial dataset resulting in the reduction of the variance of the model leading to increase accuracy. 

Based on the above results, the Balanced Random Forest Classifier has a 79% Balanced Accuracy rate, 99 % Precision rate, and a Recall rate of 91%; therefore, we recommend using the Balanced Random Forest Classifier techniques to solve for unbalanced credit card risk classification problem since all score have higher outcomes therefore yeilding a low false positive rate.

Machine Learning Model | What it does!| Results  | Disadvantages of Method
------------ | -------------  | ------------- | -------------
Naive Random Oversampling(NRO)| Minority classes are randomly selected from the data and added to the training set | Increase in the size of the minority data leading to a balanced data set.| You can end up losing critical information that can be vital to an ML model.
SMOTE Oversampling (Synthetic Minority Oversampling Technique) | The minority class are selected from an occurrence of that minority class closest neighbor or | Creates new values. | You can end up with outliners since it relies on the neighboring value.
Random Undersampling | The majority class, is randomly decreased in the training set | Decrease in most of the data, leading to a balanced data set.|  You  must have sufficient data to select from; otherwise, we can end up losing critical information that can be vital to an ML model
Combination (Over and Under) Sampling | Use Combination of SMOTE Over Sampling and Edited Nearest Neighbors (ENN) Under Sampling to remove outliers.  | Data point are dropped when if nearest neighbors are from two different classes | You  must have sufficient data to select from; otherwise, we can end up losing critical information that can be vital to an ML model
Balanced Random Forest Classifier | Multiples decision trees are fitted into a forest tree with weak learning trees. It then trains the model against a small subset of the initial dataset. | Reduction of variance of the model leading to increase accuracy  | Not ideal for skewed distribution classification
Easy Ensemble AdaBoost Classifier | Random sample of minority class train sequentially against a subset of the majority class and labeled based on prediction | Minority weighted classifier average label predictions intended to facilitate the learning during the next iteration and makes corrections of misclassification to the previous sets to minimize the pseudo-residuals  | Can be difficult to interperet 

# PICTURE OF RESULTS 
#### Naive Random Oversampling
[![Naive-Random-Sampling.png](https://i.postimg.cc/K8X6vP8s/Naive-Random-Sampling.png)](https://postimg.cc/VdRGKbMj)

#### SMOTE Oversampling  
[![SMOTEOversampling.png](https://i.postimg.cc/XvLm8tcT/SMOTEOversampling.png)](https://postimg.cc/yJJL6QGP)

#### Undersampling
[![Undersampling.png](https://i.postimg.cc/cL95tfxS/Undersampling.png)](https://postimg.cc/xXmPWJNx)

#### Combination (Over and Under) Sampling 
[![Combination-Over-and-Under-Sampling-png.png](https://i.postimg.cc/3RSMKzkg/Combination-Over-and-Under-Sampling-png.png)](https://postimg.cc/G8ygK7J2)

#### Balanced Random Forest Classifier 
[![Balance-Random-Forest-Classifier.png](https://i.postimg.cc/05njSNwf/Balance-Random-Forest-Classifier.png)](https://postimg.cc/ThyTMfQL)

#### Easy Ensemble AdaBoost Classifier
[![Easy.png](https://i.postimg.cc/8c9qvWBc/Easy.png)](https://postimg.cc/D4QjkSN3)
