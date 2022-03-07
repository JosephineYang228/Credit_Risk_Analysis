# Credit_Risk_Analysis
## Overview of the loan prediction risk analysis
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Thus this project is designed to build and evaluate models by imbalanced-learn and scikit-learn libraries. Besides, this project oversample the credit card credit dataset from LendingClubusing by using a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Comparing two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.
## Results
 - Naive Random Oversampling  
 The balanced accuracy test it 65.0%.  
 The precision for the high_risk is 1% and the recall is 64%, F1 score is 2%.  
 The precision for the low_risk is 100.0% and the recall is 66%.
![NRO](https://github.com/JosephineYang228/Credit_Risk_Analysis/blob/8f80037601cb4b0419e08cc9d67c86f56bcc3757/image/NRO.png)  

 - SMOTE oversampling  
 The balanced accuracy test it 64.0%.  
 The precision for the high_risk is 1% and the recall is 70%, F1 score is 2%.  
 The precision for the low_risk is 100.0% and the recall is 58%.
![SO](https://github.com/JosephineYang228/Credit_Risk_Analysis/blob/d15ccac5e9a801139a5ee41cdaf0d2f841eb8d96/image/SO.png)  

 - Undersampling  
 The balanced accuracy test it 64.0%.  
 The precision for the high_risk is 1% and the recall is 59%, F1 score is 1%.  
 The precision for the low_risk is 100.0% and the recall is 43%.
![US](https://github.com/JosephineYang228/Credit_Risk_Analysis/blob/8f80037601cb4b0419e08cc9d67c86f56bcc3757/image/US.png)  

 - Combination (Over and Under) Sampling  
 The balanced accuracy test it 51.0%.  
 The precision for the high_risk is 1% and the recall is 70%, F1 score is 2%.  
 The precision for the low_risk is 100.0% and the recall is 58%.
![CS](https://github.com/JosephineYang228/Credit_Risk_Analysis/blob/8f80037601cb4b0419e08cc9d67c86f56bcc3757/image/CS.png)  

 - Balanced Random Forest Classifier  
 The balanced accuracy test it 79.1%.  
 The precision for the high_risk is 3% and the recall is 70%, F1 score is 7%.  
 The precision for the low_risk is 100.0% and the recall is 88%.
![BRFC](https://github.com/JosephineYang228/Credit_Risk_Analysis/blob/8f80037601cb4b0419e08cc9d67c86f56bcc3757/image/BRFC.png)  

 - Easy Ensemble AdaBoost Classifier  
 The balanced accuracy test it 91.8%.  
 The precision for the high_risk is 9% and the recall is 89%, F1 score is 16%.  
 The precision for the low_risk is 100.0% and the recall is 94%.
![EEAC](https://github.com/JosephineYang228/Credit_Risk_Analysis/blob/8f80037601cb4b0419e08cc9d67c86f56bcc3757/image/EEAC.png)  

## Summary
Sensitivity is an important index but there are situations in which precision is more important than sensitivity. In this case, I use 6 different models to train and predit the dataset and ranking the models in descending order according to the balance accuracy score as follows:  
 - Easy Ensemble AdaBoost Classifier. The balanced accuracy test it 91.8%.  
 - Balanced Random Forest Classifier. The balanced accuracy test it 79.1%.
 - Naive Random Oversampling. The balanced accuracy test it 65.0%.
 - The other 3 models has the same score in this case (64%).  

Besides, Easy Ensemble AdaBoost Classifier model also has the highest score at F1 score (16%) and low-risk recall (94%). Since the balance accuracy and recall score needs to fall within 0 and 1, with numbers closer to 1 being the better model, I would recommend Easy Ensemble AdaBoost Classifier model to use in this case.
