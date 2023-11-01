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

I went through the following stages of the machine learning to process the analysis: Pre-processing (cleaning and preparing the raw data), then training (recognizing the pattern), then validating and evaluating the model.

First, I used the supervised learning classification model called Logistic Regression to predict the probability of the binary healthy loans vs high-risk loans event to occur. Then, I used the resampling method to generate more data points as to balance the dataset and make a more accurate model.

The results

Summary
Overall, both models worked quite well with accuracy scores above 90%. However, Model 2 had a higher balanced accuracy score of 99.6% compared to 94.4% of Model 1. Thus, Model 2 is a better classifier of loan status.

From our results it is clear that it is more difficult to accurately classify high-risk loans. However, from our domain knowledge, we know that it is more important to be able to correctly predict high-risk loans as not doing so poses a danger to lenders.

Here are the concluding recommendations:

Use Model 2, where high-risk loans are over-represented for predicting loan status.
If possible, feed the model with more training data on high-risk loans to improve accuracy.
This model is good enough to run a pilot classifying project, where this model is the first step for predicting loan status. This way, the model can be evaluated with real time data, and improved upon as needed.
In this model, we used logistic regression, but it may be worthwhile to try other supervised learning models like Random Forest, KNN or Tensor Flow, to see if they yield better results.
