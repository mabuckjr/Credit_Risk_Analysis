# Credit Risk Analysis
## Overview of the Analysis
This project required me to use various supervised machine learning tools to evaluate the credit risk of a bank's customers. The goal was to figure out which of the 6 tools would work best for determining the credit risk of their customers, and if any of the aforementioned tools were viable options for the bank to use in the future. The 4 various sampling algorithms I used were:
- Naive Oversampling
- SMOTE Oversampling
- Undersampling
- Combination Sampling (SMOTEENN)
- Balanced Random Forest Classifier
- Easy Ensemble AdaBoost Classifier
### Explanation of the different Algorithms
The first two algorithms involved oversampling the "high risk" customer data to balance the testing variables. Naive Oversampling duplicates examples from the minority class to balance the machine learning process. SMOTE Oversampling differs from Random Sampling by creating new synthetic examples from the minority class that are similar to the rest of the class. Then, I undersampled the "low risk" customer data, which basically is the opposite of the oversampling process, but yields a similar result by balancing the data. The Combination Sampling involves finding a middleground for both sets of training data, oversampling the "high risk" training set and undersampling the "low risk" training data. The Balanced Random Forest Classifier tool randomly undersamples each bootstrap sample to balance it. Easy Ensemble AdaBoost ensemble uses a group of AdaBoost learners trained on different balanced bootstrap sample by random under-sampling.
## Results
### Naive Oversampling
![](https://github.com/mabuckjr/Credit_Risk_Analysis/blob/main/Resources/Naive_Oversampling.PNG)

The Naive Random Oversampling algorithm generated a model that has a 67% balanced accuracy score, 99% precision score, and a 63% recall score.
### SMOTE Oversampling
![](https://github.com/mabuckjr/Credit_Risk_Analysis/blob/main/Resources/SMOTE_Oversampling.PNG)

The SMOTE Oversampling algorithm generated a model that has a 66% balanced accuracy score, 99% precision score, and a 69% recall score.
### Undersampling
![](https://github.com/mabuckjr/Credit_Risk_Analysis/blob/main/Resources/Undersampling.PNG)

The SMOTE Oversampling algorithm generated a model that has a 68% balanced accuracy score, 99% precision score, and a 63% recall score.
### Combination Sampling
![](https://github.com/mabuckjr/Credit_Risk_Analysis/blob/main/Resources/Combination_Sampling.PNG)

The SMOTE Oversampling algorithm generated a model that has a 66% balanced accuracy score, 99% precision score, and a 63% recall score.
