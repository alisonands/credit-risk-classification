# Credit risk classification
The following repository analyses credit risk classification of loans based on historical lending activities to identify the credit worth of borrowers.


### Methods
The dataset is comprised of 8 variables that was predicted to have an effect on the loan value. The final variable in the dataset, the 'loan_status', was classified into 0 or 1, where 0 represents a healthy loan status, and 1 has a high risk of defaulting. 

In this analysis, shallow learning was used to train the model, to determine potential risk values of future loans based on variables used in this analysis. We used Logistic Regression to determine whether the predicted value of the loan status is 0 or 1. The train-test dataset was split as 80:20.

#### Using Scikit-learn
The scikit-learn library was used for the Logistic Regression analysis to train the model. The dataset was split into a test size of 0.2 and train size of 0.8. The data is scaled using the StandardScaler module, given the variation in the dataset values.

### Results
**Confusion matrix**
|||
|:----:|:----:|
| 14940 |  71 |
|   11  | 486 |


**Classification report**
|   | Recall | Precision | f1-score |
|:-:|:------:|:---------:|:--------:|
| 0 |  1.00  |    1.00   |   1.00   |
| 1 |  0.87  |    0.98   |   0.92   |

$\text{Accuracy} = \frac{14940 + 486}{14940 + 71 + 11 + 486} = 99.4\% $

### Analysis
By looking at the classification report, we see that the recall and precision scores are 100% for predicting 0, the 'healthy' loans, and 87% and 98% for the high-risk loans, respectively. As the recall determines how often there are false negatives, 98% is a strong value for determining the high-risk labels, and we can conclude that this model can be used to determine the outcome of the loan status. Additionally, the accuracy is 99.4%, which will return strong predictions for the data. 

As with all ML models, these results should expect inaccuracies in some cases, and should be wary when determining the status of the high-risk credit loans.
