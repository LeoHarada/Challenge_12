# Challenge 12

## Overview of the Analysis

* The purpose of this analysis is to accurately report the creditworthiness of borrowers. Healthy loans outnumber risky loans, posing a classification problem that's inherently imbalanced. Using different techniques like Logistic Regression and Resampling, we are able to provide a more accurate report in identifying the credit status of the borrowers being examined.
* The financial information used for our analysis was from the historical lending activity from a peer-to-oeer lending services company. This dataset of lending activity was used to build a model that can accurately identify and predict the creditworthiness of borrowers.
* The original data provided had loand size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks and total debt. These were used to determine the difference between a healthy loan and a high-risk loan. For our analysis, healthy loans = 0 and high-risk loans = 1. Using our Logistic Regression Model and value_counts function, we are able to distinguish the two and get the count of the target classes. We then predicted the number of each of these classes and determined how accurate our model was in determining the amount in each class.
* I first read the data and split the data into Training and Testing Sets. Then, fitting a logisitic regression model by using the training data. Saving the predicitons on the testing data labels by using the testing feature dtaa and the fitted model. Lastely, predicting a logistic regression model with resampled training data.
* I used the logistic regression model to predict the continuous variables of the original data. Then, resampling the data for a more accurate report of the creditworthiness of the borrowers. Using the logistic regression model again of the resampled data to have an equal number of data points.

## Results
**Machine Learning Module - 1**
(Balanced Accuracy Score = .952)

* Healthy Loans Precision: 1.00
* Healthy Loans Recall: .99
* Healthy Loans F1 Score: 1.00
* High-risk Loans Precision: .85
* High-risk Loans Recall: .91
* High-risk Loans F1 Score: .88

**Resampled Machine Learning Module - 2**
(Balanced Accuracy Score = .993)

* Healthy Loans Precision: 1.00
* Healthy Loans Recall: .99
* Healthy Loans F1 Score: 1.00
* High-risk Loans Precision: .84
* High-risk Loans Recall: .99
* High-risk Loans F1 Score: .91

## Summary
* I recommend the resampled logical regression model, as it's more accurate than the original model. With the amount of high-risk loans significantlly lower than healthy loans, the data isn't as accurate as if you used the resampled data, where the amount of high-risk loans equals the amount of healthy loans. Using the resampled model, the balanced accuracy score increases by about .041 (4%.) The recall increased by about 8% and the F1 score increased by about 3%.
* Performance does depend on the problem we're trying to solve, as it's more important to predict the high-risk loans than the healthy loans. Knowing the accurate amount of high-risk loans are more important to know because these are the ones that pose more risk for the lender/company. Knowing this information, the lender can make more informative strategic financial decisions.
