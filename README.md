# Credit-Card-Default-Prediction
A Logistic Regression based classification model to predict Credit Defaulting

Here, we use scikit-learn, a popular machine learning package in python to train and tune a classifier.
A particularly useful feature is that all classifiers (and linear models) are called using the same API, so it is easy to test between different models (see the sklearn-intro notebook for examples).

## Dataset
The dataset we use is the default of credit card clients Data Set. There are two data files: "CreditDefault_training.csv" and "CreditDefault_Xtest.csv" Both files have the following fields, except the label ("default.payment.next.month") which is not available in "CreditDefault_Xtest.csv"

Features:

1.  LIMIT_BAL: Amount of the given credit (NT dollar): it includes both the individual consumer credit and his/her family (supplementary) credit.
2.  SEX: (1 = male; 2 = female)
3.  DUCATION: (six levels: 1,2,3,4,5,6)
4.  ARRIAGE: (1 = married; 2 = single; 3 = others)
5.  AGE

From "PAY_1" to "PAY_6": History of past payment (Repayment status: -2: Balance paid in full and no transactions this period; -1: Balance paid in full, but account has a positive balance at end of period due to recent transactions for which payment has not yet come due; 0: Customer paid the minimum due amount, but not the entire balance; 1 = payment delay for one month; 2 = payment delay for two months; . . .; 8 = payment delay for eight months; 9 = payment delay for nine months and above.)
6.  PAY_1: the repayment status in September, 2005
7.  PAY_2: the repayment status in August, 2005
...
11. PAY_6: the repayment status in April, 2005

From "BILL_AMT1" to "BILL_AMT6": Amount of bill statement (NT dollar).
12. BILL_AMT1 : amount of bill statement in September, 2005
13. BILL_AMT2 : amount of bill statement in August, 2005
...
17. BILL_AMT6 : amount of bill statement in April, 2005

From "PAY_AMT1" to "PAY_AMT6": Amount of previous payment (NT dollar).
18. PAY_AMT1 : amount paid in September, 2005
19. PAY_AMT2 : amount paid in August, 2005
...
23. PAY_AMT6 : amount paid in April, 2005

Target:

default.payment.next.month: binary variable, whether default payment (Yes = 1, No = 0)

Training dataset, "CreditDefault_training.csv", contains 3985 rows and 24 columns. This is the training set containing both of the features and the target. Test dataset, "CreditDefault_Xtest.csv", contains 1000 rows and 23 columns. This is the test set which only contains the features.

Prediction task is to determine whether there's credit default for a person.

## Model
Refer this [Link]() for the code.
