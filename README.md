# credit-risk-classification

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* The purpose of this analysis is to create a ML model that would be able to predict a healthy vs a high-risk loan, which may lead to it deciding what loans to approve.
* The financial data this was based on was; loan size, interest rate, borrower's income, debt to income of borrower, 
					    number of accounts the borrower has, negative marks of borrower, total debt of borrower, and loan status (for training).
* We wanted to predict the loan status column correctly during this analysis.
* We set up a logistical regression model using lbfgs solver at first, then we evaluated and resampled the data to improve the model using random over sampler. 
  This was in an attempt to over sample the minority data as the first modelling attempt did not have enough of that data.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Balanced accuracy score is 0.9520
    * Precision rate is 1.00 for `0` and 0.85 for `1`
    * Recall rate is 0.99 for `0` and 0.91 for `1`

* Machine Learning Model 2:
    * Balanced accuracy score is 0.9947
    * Precision rate is 0.99 for `0` and 0.99 for `1`
    * Recall rate is 0.99 for `0` and 0.99 for `1'

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* The 2nd model seems to perform better as it performed as well if not better on every measureable metric.
* Performance absolutely depends on what we are trying to predict, as if our model approved a loan which was actually a high-risk loan we have a chance of not being paid back for that loan.
  As opposed to incorrectly approving a healthy loan which simply means we have lost out on potential business, but do not have a potential liability for the future.
