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

#### Recommendation: 
Based on the above results, the Balanced Random Forest Classifier has a Balanced Accuracy Score of 0.79, Precision Score of 0.99, and a Recall Score; therefore, we recommend using the Balanced Random Forest Classifier techniques to solve for unbalanced credit card risk classification problem. In the Balanced Random Forest Classifier, Multiples decision trees are fitted into a forest tree with weak learning trees. It then trains the model against a small subset of the initial dataset resulting in the reduction of the variance of the model leading to increase accuracy

Machine Learning Model | What it does!| Results  | Disadvantages of Method
------------ | -------------  | ------------- | -------------
Naive Random Oversampling(NRO)| Minority classes are randomly selected from the data and added to the training set | Increase in the size of the minority data leading to a balanced data set.| You can end up losing critical information that can be vital to an ML model.
SMOTE Oversampling (Synthetic Minority Oversampling Technique) | The minority class are selected from an occurrence of that minority class closest neighbor or | Creates new values. | You can end up with outliners since it relies on the neighboring value.
Random Undersampling | The majority class, is randomly decreased in the training set | Decrease in most of the data, leading to a balanced data set.|  You  must have sufficient data to select from; otherwise, we can end up losing critical information that can be vital to an ML model
Combination (Over and Under) Sampling | Use Combination of SMOTE Over Sampling and Edited Nearest Neighbors (ENN) Under Sampling to remove outliers.  | Data point are dropped when if nearest neighbors are from two different classes | You  must have sufficient data to select from; otherwise, we can end up losing critical information that can be vital to an ML model
Balanced Random Forest Classifier | Multiples decision trees are fitted into a forest tree with weak learning trees. It then trains the model against a small subset of the initial dataset. | Reduction of variance of the model leading to increase accuracy  | Not ideal for skewed distribution classification
Easy Ensemble AdaBoost Classifier | Random sample of minority class train sequentially against a subset of the majority class and labeled based on prediction | Minority weighted classifier average label predictions intended to facilitate the learning during the next iteration and makes corrections of misclassification to the previous sets to minimize the pseudo-residuals  | Can be difficult to interperet 



