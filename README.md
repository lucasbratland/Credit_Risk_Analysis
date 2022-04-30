# Credit_Risk_Analysis
## Overview
The purpose of this analysis is to predict high credit card risk using machine learning. The features (factors going into the predictive model) include various information on the amount and type of credit, credit limit, home ownership, annual income, current and past debt, utility payments, previous bankruptcy, and other financial hardships. The goal of the analysis is to use machine learning algorithms to identify applicants with high risk for default on their credit card payments.

The same dataset was used for all analyses. Data was cleaned and transformed into numerical constructs prior to analysis.

The following machine learning models were used to predict high credit card risk.

- Naive random over-sampling
- SMOTE over-sampling
- Cluster centroids under-sampling
- SMOTEENN combination (over and under) sampling:
- Balanced Random Forest Classifier ensemble sampling
- Easy Ensemble AdaBoost Classifier

## Results
Here are the accuracy, precision, sensitivity and specificity scores:
| Model | Accuracy | Precision | Sensitivity | Specificity |
| :---: | :---: | :---: | :---: | :---: |
| Naive | 0.65 | 0.01 | 0.71 | 0.58 |
| SMOTE | 0.66 | 0.01 | 0.63 | 0.68 |
| Cluster | 0.54 | 0.01 | 0.69 | 0.40 |
| SMOTEEN | 0.64 | 0.01 | 0.72 | 0.57 |
| Random Forest| 0.79 | 0.03 | 0.70 | 0.87 |
| AdaBoost| 0.93 | 0.09 | 0.92 | 0.94 |

## Summary and Recommendation
When looking at all the models, AdaBoost and Random Forest excelled at Accuracy. None ofthe models were good at precision. All models were trelatively moderate with sensitivity except the AdaBoost which was better than the rest. 

Because of the potential costs of missing a high risk customer I would recommend using the AdaBoost model. The sensitivity of this model at .92 is the best in this measure. This would give us the least amount of false negatives.  