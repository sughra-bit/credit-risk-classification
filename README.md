# credit-risk-classification

Overview of the Analysis

Objective:

The purpose of this analysis is to use various techniques to train and evaluate a model based on loan risk by using a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

The dataset reflected the following financial information: 
Loan size, 
Interest rate,
Borrower income, 
Debt-to-income ratio, 
Number of accounts,
Derogatory marks 
Total debt of each loan application.

In the dataset, we can see there is a discrepancy between the healthy loans (0) counts and the high-risk loans (1) counts: 75036 healthy loans count vs 2500 high-risk count.

Following steps of the machine learning was used to process the analysis: 
cleaning and preparing the raw data, 
training (recognizing the pattern), then 
validating and evaluating the model.

Used the supervised learning classification model (Logistic Regression) to predict the probability of the binary healthy loans vs high-risk loans event to occur. Then, I used the resampling method to generate more data points as to balance the dataset and make a more accurate model.

The results

Model 1:

Accuracy - the model displays 18679 true positive results and 558 true negative results.

Precision - the ratio of the correctly predicted true positives to the total predicted positive observations: the model performs better predicting healthy loans (precision 1) than high-risk loans (precision 0.87).

Recall - the ratio of actual positives identified correctly: the model performs better predicting healthy loans (recall 1) than high-risk loans (recall 0.89).

Support - the number of actual occurrences of the class in the specified dataset: according to the support column, the model is imbalanced in the training data (healthy loans 18759 vs high-risk loans 625), indicating structural weaknesses in the reported scores, in the evaluation process.

Machine Learning Model 2:

Accuracy - the model displays 55945 true positive results and 55954 true negative results.

Precision - the ratio of the correctly predicted true positives to the total predicted positive observations: the model performs equally well for predicting healthy loans (precision 0.99) and high-risk loans (precision 0.99).

Recall - the ratio of actual positives identified correctly: the model performs equally well for predicting healthy loans (recall 0.99) and high-risk loans (recall 0.99).

Support - the number of actual occurrences of the class in the specified dataset: according to the support column, the model is balanced in the training data (healthy loans 56277 vs high-risk loans 56277), indicating structural strength in the reported scores, in the evaluation process.


Summary
Overall, both models worked quite well with accuracy scores above 90%. However, Model 2 had a higher balanced accuracy score of 99.6% as compared to 94.4% of Model 1. Thus, Model 2 is a better classifier of loan status.
