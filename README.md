# credit-risk-classification

## Overview of the Analysis

In this challenge, machine learning models were used in order to identify the creditworthiness of borrowers by making use of historical lending data from a peer-to-peer lending services company. The analysis included variables such as loan size, borrower income, debt to income ratio to predict the if the borrowers were creditworthy a.k.a to determine whether the loan would be healthy or high-risk. The data was first split into training and testing sets. The labels were determined from the loan_stuatus column and the rest of the columns were considered as features. It was observed that in the historic data, there were inherently more number of instances with healthy loan status as opposed to high-risk. A logistic regression model was fit on the training data and once the model was trained on the training set, it was used to predict the data labels for the testing set. This model was then evaluated. 

The second model that was created took into account the unbalanced data within the two categories and resampling of the training data was done. This means that data points from the high-risk category were oversampled to ensure that both categories had the same number of samples. Logistic regression was run and the same steps as above were repeated.


## Results

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

     * This model had a balanced accuracy score of 0.95. 
     * The precision score for the healthy loan category was 1.00 whereas the precision score for the high-risk loan category was 0.85
     * The recall score for the healthy loan category was 0.99 whereas the recall score for the high-risk loan category was 0.91


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

     * This model had a balanced accuracy score of 0.99. 
     * The precision score for the healthy loan category was 1.00 whereas the precision score for the high-risk loan category was 0.84
     * The recall score for the healthy loan category was 0.99 whereas the recall score for the high-risk loan category was 0.99

## Summary

Overall, it seems like model 2 had a higher balanced accuracy score (0.99) than model 1 (0.95), a 4% increase. Model 2 also had a higher recall score for the high risk loan category (0.91) than model 1 (0.85), a 7% increase. However, model 2 had a precision score of 0.84 which is a 1% decrease from model 1 for the high-risk loan category. There were no differences in the precision and recall scores of the healthy loan predictions between either of the models. This is because oversampling was performed in model 2 which increased the data points for the high-risk loan category and balanced the dataset and reduced the bias. Model 2 is recommended because it takes into account data that has been oversampled from the minority category, hence making it more representative. Recall score is the ratio of correctly predicted positive observations to all predicted observations for that class. The increased recall-score for the high-risk loan category means that all individuals who fall into this category will be identified along with some individuals that belong to the healthy loan category, which would be a better outcome than being unable to identify and granting loans to individuals who belong to the high-risk loan category. Hence, in this case, it is better to have high recall scores for predicting the high-risk loan category as opposed to high precision scores.
