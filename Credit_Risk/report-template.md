# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

The idea is to create a machine learning model, this is intended to determine if a loan is safe or risky based on the loan status.
This is based on the loan status provided by the finantial institution.
It was used a logistic regresion model which had an impressive accuracy.


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  * For the healthy loan, the precision is 1, the recall is 1, the f1-score is 1 and the support is 18759
  * For the high-risk loan, the precision is 0.87, the recall is 0.89, f1-score is 0.88 and the support is 625

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  * For the healthy loan, the precision is 1, the recall is 1, the f1-score is also 1 and the support is 18579
  * For the high-risk, the precision is 0.87, the recall is 1, the f1-score us 0.93 and the support is 625

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

The results indicate the model is better predicting healthy loans.
The reason behind this is the number of records for healthy loans is greater than the high risk.
To fix this, we used the RandomOverSampler module which adds more data from the high risk loans.
It is recommended to have a balanced set of data to avoid false positives.
