# measure__customer_ceasing_repayment

Classifier: Risk models designed to assess the likelihood of a customer defaulting on repayment.
Goal:
The goal is to develop risk models in order to measure the probability of a customer ceasing repayment of their balance. Your task is to build a classifier that predicts which customers will be unable to pay their balance for 2 months within the next 12 months.

Focus:
For this task, we are mostly interested in observing your methodology. So, please focus on implementing the appropriate preprocessing steps while writing clean and documented code.

Dataset:
You are given two datasets, “X.csv” and “y.csv”, containing the features and the labels respectively. Your task is to split the dataset into train and test sets and fit only 2 classification algorithms on the training set. You may choose any classification algorithms that you prefer. After fitting, evaluate the performance of the two models on the test set.

The file “X.csv” has the following columns:
id: unique identifier of the account
existing_score: the score of the existing machine learning model (you may use it as an input or for checking if your model performs better than the existing model)
open_to_buy: the difference between the credit limit and the balance. If the customer does not have a credit card, it is NaN.
months_since_first_loan_issued: number of months since the first loan was issued. If the customer has not taken any loans, it is NaN
existing_credit_card_utilization: balance / credit limit * 100, e.g. 30 means that 30% of the credit limit is utilized. If the customer does not have a credit card already, it is NaN
n_months_mortgage_loan_paid: number of months during which the balance of the account decreased. If the customer does not have a mortgage already, it is NaN
The file “y.csv” contains the following columns:
id: unique identifier of the account
label: 1 if the account did not pay their balance for 2 months during the next 12 months, otherwise 0.
