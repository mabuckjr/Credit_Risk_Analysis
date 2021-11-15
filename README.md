# Credit Risk Analysis
## Overview of the Analysis
This project required me to use various supervised machine learning tools to evaluate the credit risk of a bank's customers. The goal was to figure out which of the 6 tools would work best for determining the credit risk of their customers, and if any of the aforementioned tools were viable options for the bank to use in the future. The 4 various sampling algorithms I used were:
- Naive Oversampling
- SMOTE Oversampling
- Undersampling
- Combination Sampling (SMOTEENN)
- Balanced Random Forest Classifier
- Easy Ensemble AdaBoost Classifier
The first two algorithms involved oversampling the "high risk" customer data to balance the testing variables. Then, I undersampled the "low risk" customer data, which basically is the opposite of the oversampling process, but yields a similar result by balancing the data. The Combination Sampling involves finding a middleground for both sets of training data, oversampling the "high risk" training set and undersampling the "low risk" training data.
