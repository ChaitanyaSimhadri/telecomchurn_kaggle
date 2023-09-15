# Telecomchurn_kaggle Competetion
Telecom churn project for Kaggle competition

This Project is submitted to IIIT bangalore for a kaggle competetion with in the group and stood top in the competetion with scaore of 0.237.

### Problem Statement:

In the telecom industry, customers are able to choose from multiple service providers and actively switch from one operator to another. In this highly competitive market, the telecommunications industry experiences an average of 15-25% annual churn rate. Given the fact that it costs 5-10 times more to acquire a new customer than to retain an existing one, customer retention has now become even more important than customer acquisition.

For many incumbent operators, retaining high profitable customers is the number one business
goal. To reduce customer churn, telecom companies need to predict which customers are at high risk of churn. In this project, you will analyze customer-level data of a leading telecom firm, build predictive models to identify customers at high risk of churn.

In this competition, goal is to build a machine learning model that is able to predict churning customers based on the features provided for their usage.


 Dataset has total of 69999 columns  and 172 features, Dropped the features with has no variance which seems insignificant with no variance.
 After imputing missing values with mean and mode, churn percentage is at 10, as data is highly imbalanced.

### Observations from EDA:

Most people are recharging on last day of the month in all three months.
Let us derive date from the columns
As last date does not change in all three columns last_date_of_month_8,last_date_of_month_7 and last_date_of_month_6, let us drop these columns.

### Models and accuracy:

Accuracy of logistic regression using RFE is giving 90% accuracy
Random forest overfits with 99% on training data and 89% test data.
arpu_6,roam_ic_mou_8 and roam_og_mou_8 are top three variables.

## Using PCA for Feature elimination
Model has 89% accuracy
And model churns 37 Features which explains 90% variance
Most Important features are arpu6,onnet_mou_6 and offnet_mou_6

## Hyper-parameter tuning using Cross Validation

Random forest Seems to give better model of all other models.
13 max features are selected using Random search CV
8th month KPIs are strong indicatiors of churn
Outgoing minutes of Usage and Incoming minutes of ussage are strong indicators of churn
Day of last recharge and age on network too hints on Churning of a customer


https://www.kaggle.com/competitions/ml-lab-i-c40/leaderboard




