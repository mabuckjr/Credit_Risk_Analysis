# Credit Risk Analysis
## Overview of the Analysis
This project required me to use various supervised machine learning tools to evaluate the credit risk of a bank's customers. The goal was to figure out which of the 6 tools would work best for determining the credit risk of their customers, and if any of the aforementioned tools were viable options for the company to use in the future. The 4 various sampling algorithms I used were:
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

The Undersampling algorithm generated a model that has a 68% balanced accuracy score, 99% precision score, and a 63% recall score.
### Combination Sampling
![](https://github.com/mabuckjr/Credit_Risk_Analysis/blob/main/Resources/Combination_Sampling.PNG)

The Combination algorithm generated a model that has a 68% balanced accuracy score, 99% precision score, and a 58% recall score.
### Balanced Random Forest Classifier (BRFC)
![](https://github.com/mabuckjr/Credit_Risk_Analysis/blob/main/Resources/Balanced_Random_Forest.PNG)

The BRFC algorithm generated a model that has a 79% balanced accuracy score, 99% precision score, and a 87% recall score.
### Easy Ensemble AdaBoost Classifier
![](https://github.com/mabuckjr/Credit_Risk_Analysis/blob/main/Resources/Easy_Ensemble_AdaBoost.PNG)

The Easy Ensemble AdaBoost algorithm generated a model that has a 93% balanced accuracy score, 99% precision score, and a 94% recall score.
## Summary
Unfortunately, most of these models would not be a good fit for the purposes of analyzing credit risk. With most of the balanced accuracy scores being below 70%, there is just too much room for error. If the predictions weren't reviewed by someone after the model analyzed someone's loan eligibility, someone would have a high chance of being put into the wrong category. The biggest issue is that all of the models have a harder time predicting those with high risk, meaning that someone may be given a loan that would be considered at risk of defaulting on their loan. The potential losses seem to outweigh the negatives for most part.

There were two models that did much better than the other 4, and those were the ones created using the BRFC and AdaBoost algorithms. It seems that ensemble classifiers did a much better job predicting those who are truly "high risk." Of the 2 algorithms, Easy Ensemble AdaBoost created the best model. With more tweaking and more random states, it could be a good tool to use for quickly identifying those who may be in the "high risk" category, and then those could be reviewed by employees who can determine which candidates from the narrowed down list for who would actually be "low risk." Some may slip through and have to default on their loans with the model as it is, but with more data added to the model and a human employee regularly reviewing loan applications, it could be a tool that saves a lot of overhead costs with the automation of a mudane, tedious task.
