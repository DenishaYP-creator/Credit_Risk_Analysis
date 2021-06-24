# Credit_Risk_Analysis
 


Write a brief summary and analysis of the performance of all the machine learning models used in this Challenge.

## Overview of the analysis: 
Explain the purpose of this analysis.



**The deliverables for this Challenge are as follows:**
- Deliverable 1: Use Resampling Models to Predict Credit Risk
- Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk
- Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
- Deliverable 4: A Written Report on the Credit Risk Analysis (README.md)

**File Upload to this Credit_Risk_Analysis GitHub repository:**
1. credit_risk_resampling.ipynb file.
2. credit_risk_ensemble.ipynb file.
3. README.md with written analysis.


## Results: 
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

#### Three techniques to address class imbalance: 
1. Oversampling
2. Undersampling
3. Combination approach of Oversampling & Undersampling

Machine Learning Model | What it does!| Results  | Disadvantages of Method
------------ | -------------  | ------------- | -------------
Naive Random Oversampling(NRO)| In  NRO minority class are randomly selected from the data and added to the training set | Increase in the size of the minority data leading to a balance data set.| You can end up losing critial information that can be vital to a ML model.
SMOTE Oversampling (Synthetic Minority Oversampling Technique) | The minority class are selected from an occurance of that minority class closest neihborbor | Creates new values. | You can end up with outlineirs since it relies on the neighboring value.
Random Undersampling | The majority class are randomly decreased in the training set | Decrease in the size of the majority data leading to a balance data set.|  You  must have sufficent data to select from otherwise we can end up losing critial information that can be vital to a ML model

Machine Learning Model | What it does!| Results  | Disadvantages of Method
------------ | -------------  | ------------- | -------------
Combination (Over and Under) Sampling | In Combination (Over and Under) Sampling | resulting in| The disadvantage of this metthod
Balanced Random Forest Classifier | Mutiples decision trees are fitted into a forest tree with weak learning trees. It then   trains model agaist a small subset of the initial dataset. | Reduction of variance of the model leading to increase accuracy  | Not ideal for skewed distribution classification
Easy Ensemble AdaBoost Classifier | Use of Bootstraping and agreegation of implmented in the model. Bootstraping a repested process in with random sample of minority class are taken and placed back into the general data population. Each bootstrap minoriity class sample set is ran idenpendently againt subset of the majpority class and labeled based on prediction durign the agrregation process| Minority weighted classifier average label predictions intended to faciliate the correction of misclassification.   | The disadvantage of this metthod




Oversample the minority class with SMOTE.
Clean the resulting data with an undersampling strategy. If the two nearest neighbors of a data point belong to two different classes, that data point is dropped.

