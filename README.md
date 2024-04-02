# Credit risk classification
The following repository analyses credit risk classification of loans based on historical lending activities to identify the credit worth of borrowers.


### Methods
The dataset is comprised of 8 variables that was predicted to have an effect on the loan value. The final variable in the dataset, the 'loan_status', was classified into 0 or 1, where 0 represents a healthy loan status, and 1 has a high risk of defaulting. 

In this analysis, shallow learning was used to train the model, to determine potential risk values of future loans based on variables used in this analysis. We used Logistic Regression to determine whether the predicted value of the loan status is 0 or 1. The train-test dataset was split as 80:20.

#### Using Scikit-learn
The scikit-learn library was used for the Logistic Regression analysis to train the model. The dataset was split into a test size of 0.2 and train size of 0.8. The data is scaled using the StandardScaler module, given the variation in the dataset values.

### Analysis
By looking at the classification report, we see that the recall 