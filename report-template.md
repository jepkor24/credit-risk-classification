# Module 20 Report Template
# Overview of the Project

The purpose of this analysis is to develop a machine learning model that can predict the credit worthiness of borrowers based on the lending data. The data set contains information about the loans such as loan size, interest rate, borrower income, debt to income ratio, number of accounts, total debt,loan status and derogatory marks.

The objective is to train and evaluate the logistic regression model to classify loans into two categories i.e. healthy loans(0) or high-risk loans(1). This will help the business to make better decisions on who is eligible for the loans to avoid risk of defaulting on the loans.

The goal is to develop a reliable model to improve risk management and enhance the issuance of loan process to its customers and at the same time minimize false positives and false negatives

## Analysis 
Below are the steps taken to perform the analysis:  
- The analysis starts with identify the target variables and the features based on the structure of the data
- Once we have identified our target and features, we then split the data in order to have data for training and data for testing
- The instantiation of the logistic regression model to ensure consistency and with default values
- Fitting the model using a subset of the data that has been split in the previous step
- Identify the patterns from the training data and if consistent with outcome
- Apply the test data to the trained model to see if the data or information is consistent or different
- Evaluate the performance of the model using the confusion matrix and the classification report. The confusion matrix provides a visualization of the performance of the classification model and the classification report provides a more detailed evaluation of the the models performance regarding precision, recall, f1-score, support and also using weighted average to evaluate data sets that are not equal in volume of data sets.

## Results

**For class 0 (healthy loans):**

**Precision:** 100% (1.00) - This means that all the loans predicted as healthy were actually healthy. 
**Recall:** 100% (1.00) - This indicates that all actual healthy loans were correctly identified by the model. 
**F1-score:** 100% (1.00) - The harmonic mean of precision and recall is at 100% which is good. 
**Support:** 18,759 - This is the number of actual occurrences of healthy loans in the test dataset; which is a good sample to use.

**For class 1 (high-risk loans):**

**Precision:** 87% (0.87) - Among the loans predicted as high-risk, 87% were actually high-risk.  
**Recall:** 89% (0.89) - The model correctly identified 89% of the actual high-risk loans.  
**F1-score:** 88% (0.88) - The F1-score, which balances precision and recall, is also high considering the uneven data sets of healthy and high risk loans.  
**Support:** 625 - This is the number of actual occurrences of high-risk loans in the test dataset.  
**Accuracy:** 99% - This is the overall accuracy of the model, indicating that 99% of the predictions were correct, which is also supported by the training and testing data sets values(Training Data score: 0.9914878250103177, Testing Data score: 0.9924164259182832)  
**Weighted Average:** 99% The weighted average of the performance of the model was 99% accuracy even considering the disparity of data sets of healthy and high-risk loans  

## Summary

The model performs very well for class 0, with good precision, recall, and F1-score. For class 1, while precision, recall, and F1-score are slightly lower than class 0, they are still quite high, indicating strong predictive performance. The high accuracy and high scores across all metrics suggest that the model is highly effective at distinguishing between healthy and high-risk loans. Overall, based on this classification report, the logistic regression model appears to be very successful in predicting both healthy and high-risk loans.
