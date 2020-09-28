# Supervised-Machine-Learning-and-Credit-Risk

In this project we performed Supervised Machine Learning  using the data file LoanStats_2019Q1, to make credit risk predictions based on training data compared to testing data.Several different prediction models were utilized to process the data and are included in two seperate files credit_risk_ensemble and credit_risk_resampling. 

In both files we trained for a logistic regression classifier utlizing Scikit-Learn using the resampled data. From there we calculated precision,recall/sensitivty, balanced accuracy score, and the confusion matrix to evaluate and compare the modles.

### In the credit_risk_ensemble we compared two ensemble algorithms, Balanced Random Forest Classifier and Easy Ensemble AdaBoost Classifier. 

### Balanced Random Forest Classifier
Accuracy Score: 78.8%
Confusion Matrix : Confusion Matrix: TP: 71, FN:30, FP: 2153, TN: 14951

Precision:
High Risk: 0.03
Low Risk Risk: 1.0

Recall/Sensitvity:
High Risk: 0.70
Low Risk Risk: 0.87

### Easy Ensemble Adaboost Classifier 

Accuracy Score: 93.1%
Confusion Matrix : Confusion Matrix: TP: 93, FN:8, FP: 983, TN: 16121

Precision:
High Risk: 0.03
Low Risk Risk: 1.0

Recall/Sensitivity:
High Risk: 0.70
Low Risk Risk: 0.87

The Easy Ensemble AdaBoost Classifier model outperformd The RainForest Classifier in this comparision. The Easy Ensemble Adaboost has higher True Positvies, 93 vs 71, lower False Negatives,  8 vs 30, and a higher balanced accuracy score 93.1% vs 78.8%.

### In the credit_risk_resampling we compared two oversampling algorithms, Naive Random Oversampling and Smote Oversampling. We then created created one undersampling algorithm , Cluster Centroids, to determine which algorithm results compared to the oversampling algorithms performed the best. Finally we used combination sampling , SMOTEEN, to compare to the previous sampling models. 

### Naive Random Oversampling

Accuracy Score: 65.4%
Confusion Matrix : Confusion Matrix: TP: 70, FN:31, FP: 6571, TN: 10533

Precision:
High Risk: 0.01
Low Risk Risk: 1.0

Recall/Sensitivity:
High Risk: 0.69
Low Risk Risk: 0.62

### Smote Oversampling 

Accuracy Score: 66.2%
Confusion Matrix : Confusion Matrix: TP: 64, FN:37, FP: 527, TN: 11837

Precision:
High Risk: 0.01
Low Risk Risk: 1.0

Recall/Sensitivity:
High Risk: 0.63
Low Risk Risk: 0.69

### Undersampling

Accuracy Score: 54.71
Confusion Matrix : Confusion Matrix: TP: 69, FN:32, FP: 10071, TN: 7033

Precision:
High Risk: 0.01
Low Risk Risk: 1.0

Recall/Sensitivity:
High Risk: 0.68
Low Risk Risk: 0.41

### Combination Sampling SMOTEEN

Accuracy Score:64.4%
Confusion Matrix : Confusion Matrix: TP: 73, FN:28, FP: 7413, TN: 9691

Precision:
High Risk: 0.01
Low Risk Risk: 1.0

Recall/Sensitivity:
High Risk: 0.72
Low Risk Risk: 0.57



All 4 models are similarly ranged with Undersampling having the lowest balanced accuracy score 54.71 while the other three prediction models ran close ranging between 64 % -   66 %.
Combination sampling with SMOTEEN is proably the best model. While the balanced accuracy score is only the thrid highest the varaince between them is small. It producs a higher number of true postives and a lower number of false negatives. 

# Summary 

The Easy Ensemble AdaBoost Classifier model outperformed the other prediction model. The Easy Ensemble Adaboost has the highest True Positvies, the lowest False Negatives, and  the highest balanced accuracy score. 


