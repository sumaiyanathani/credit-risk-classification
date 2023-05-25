# credit-risk-classification

## Overview of the Analysis

In this challenge, machine learning models were used in order to identify the creditworthiness of borrowers by making use of historical lending activity from a peer-to-peer lending services company. The analysis included variables such as loan size, borrower income, debt to income ratio to predict the if the borrowers were creditworthy a.k.a to determine whether the loan would be healthy or high-risk. The data was first split into training and testing sets. The labels were determined from the loan_stuatus column and the rest of the columns were considered as features. It was observed that in the historic data, there were inherently more number of instances with healthy loan status as opposed to high-risk. A logistic regression model was fit on the training data and once the model was trained on the training set, it was used to predict the data labels for the testing set. This model was then evaluated. 

The second model that was created took into account the unbalanced data witin the two categories and resampling of the training data was done. 

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

-- Talk about the balance and how the recall score for category 1 was lesser


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

-- How the recall score for category 1 increased

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

-- Overall, Model 2 is recommended because it takes into account data that has been oversampled from the minority category, hence more representative and balanced.

If you do not recommend any of the models, please justify your reasoning.
