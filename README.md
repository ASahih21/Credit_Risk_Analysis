# Supervised Machine Learning Credit Risk Analysis

The purpose of this analysis is to select an algorithm that can best predict HIGH or LOW credit risk by training using historical credit information. This is done by using a number of resampling models and algorithms to find a configuration with the best fit based on their accuracy and precision scores.

## Background

Multiple methods were used, some resampling the data to provide an even analysis for low and high risk borrowers with Logistic Regression (there were far fewer "high risk" borrowers identified in the dataset than "low risk"). Other methods utilized 'ensemble' imbalanced learning modules. All of these were compared to determine what the best method may be for predicting credit risk in the data.


## Conclusions and Recommendations

The above indicates that each method saw very high precision for predicting low risk borrowers, while seeing extrememly low precision predicting high risk borrowers. Recall scores using resampling within the Logistic Regression model were highest on average for Random Oversampling and SMOTE. Individual scores were highest for Low Risk using SMOTE, and High Risk using SMOTEENN. Balanced accuracy among the resampling methods was highest for Random Oversampling. 

The ensemble methods saw recall scores on average to be highest for the Easy Ensemble Classifier, but individually the Balanced Random Forest Classifier saw the highest value for Low Risk and Easy Ensemble Classifier for High Risk. Balanced accuracy among the ensemble methods was highest for the Easy Ensemble Classifier.

Given that the dataset is imbalanced, the recall and balanced accuracy scores are the better metrics to follow. Given this, the best performing model for the data was the Easy Ensemble Classifier method. Further exploration should be done, removing columns that do not perform well (if at all) given the importance scores.
