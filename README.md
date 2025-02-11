# credit-risk-classification
Challenge 20

The sources for my code were: solved class exercises, Github, ChatGPT, Google, and YouTube. 

Analysis for credit_risk_classification challenge

OVERVIEW

This logistic regression model analyzed a data set of 77,537 records with the following data categories: loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status. Loan status was indicated by either a “0” (healthy loan) or a “1” (high-risk loan). 

The purpose of analyzing this data was to predict the risk of a loan, whether it was healthy or high risk. First, the data was split into training and testing datasets using train_test_split. Then LogisticRegression was used with a random state of 1 using the training data (X_train and y_train). After that, predictions on the testing data were produced. 

RESULTS

The logistic regression model performed exceptionally well in classifying loan types, achieving an overall accuracy of 99 percent. 

Results for Loan Type 0 (Healthy):

•	Precision: 100 percent

•	Recall: 100 percent

•	F1-score: 100 percent

•	Number of supporting records: 18759

The perfect 100 percent across all metrics indicates the model correctly identified all instances of this loan type/category 0 with no misclassifications. 

Results for Loan Type 1 (High-Risk):

•	Precision: 87 percent

•	Recall: 95 percent

•	F1-score: 91 percent

•	Number of supporting records: 625

SUMMARY

While this was a strong performance, the results suggest there are false positives present in the results for this loan type/category 1. It should be noted the number of supporting records is drastically fewer than that of the healthy loan type (category 0), and that should be considered as a potential impacting factor.

Overall, the Macro Average scores for Precision (0.94), Recall (0.97), and F1-score (0.95) show a balanced performance of the model across both loan types. The Weighted Average scores are close to perfect (0.99), which reflect primarily the accuracy of loan type 0 (healthy). While this model demonstrates high effectiveness and accuracy, slight misclassification occurrences within the loan type 1 (high-risk) needs to be improved still. Options could include class balancing or adjusting decision thresholds for the two loan types. 
