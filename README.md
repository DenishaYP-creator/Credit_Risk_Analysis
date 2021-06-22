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

Cluster Centroid Undersampling



## Summary: 
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

Machine Learning Model | Balanced Accuracy Score| Precision Score| Recall Score
------------ | -------------  | ------------- | -------------
Naive Random Oversampling| In  Naive Random Oversampling the the minority class are randomly selected from the data and added to the training set resulting in increase in the size of the minority data| set resulting in increase in the size of the minority data leading to a balance data set.|  The disadvantage of this metthod is that you  can end up losing critial information that can be vital to a ML model.
SMOTE Oversampling | In Oversampling(Synthetic Minority Oversampling Technique), on the other hand, the minority class are selected from an occurance of that minority class closest neihborbor | resulting in the creation of new values. | The disadvantage of this metthod is that you  can end up with outlineirs.
Random Undersampling | In  Udersampling the the majority class are randomly decreased in the training set | resulting in decrease in the size of the majority data leading to a balance data set.| The disadvantage of this metthod is that you  must have sufficent data to select from otherwise the we can end up losing critial information that can be vital to a ML model
Combination (Over and Under) Sampling | 0.57 | 0.99| 0.51


Balanced Random Forest Classifier | 0.79 |  0.99 |  0.91 
Easy Ensemble AdaBoost Classifier | 0.92 | 0.99 | 0.94 

Three techniques to address class imbalance: 

3. Randome Undersampling:  In  Udersampling the the majority class are randomly decreased in the training set resulting in decrease in the size of the majority data leading to a balance data set. The disadvantage of this metthod is that you  must have sufficent data to select from otherwise the we can end up losing critial information that can be vital to a ML model
4. combination approach of oversampling and undersampling

Instead

