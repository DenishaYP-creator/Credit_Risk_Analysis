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



## Summary: 
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

Three techniques to address class imbalance: 
1. Naive Random Oversampling : In Naive Random Oversampling the majority and minority classes are balanced. The data selection in one in which the minority class are randomly selected and added to the training set resultign in a balance data set. The disadvage of this metthod is that you  can end up losing critial information that is critcal to a model.
3. undersampling
4. combination approach of oversampling and undersampling

