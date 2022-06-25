# Credit-Card-Risk-Analysis
**Goal** - Building a Machine Learning model to predict the likely hood of loan repayment on a given profile  <br />
**Skills used** Python, EDA, Machine Learnin <br>
**Libraries used**- Pandas,  Seaborn, Scikit learn, numpy, matplotlib <br>
**Score**  - Accuracy of 70% with a recall score of 100. <br />
**Best Fit Model**  - Naive bayes and Random Forest Classifier  <br />
# Introduction
Any leading bank would like to predict whether or not a candinate would be able to repay the loan. 
This projects uses Machine learning Algorithms to predict the possibility of loan repayment by a customer. 
First we Explore the data to understand the relation of defaulters in loan repayment with respect to age, education, debts etc
We use the relation to train the dataset to perform Classification Algorthims in Machine Learning
* **Analyzing data of over 1000 applicants to understand the features in project**
    Columns in the data - <br>
    The data contains the credit details about credit borrowers:<br>
    age - Age of Customer, ed - Eductation level of customer, employ: Tenure with current employer (in years) <br>
    address: Number of years in same address, income: Customer Income, debtinc: Debt to income ratio <br>
    creddebt: Credit to Debt ratio, othdebt: Other debts, default: Customer defaulted in the past (1= defaulted, 0=Never defaulted) <br>
    Total Entries - 1000 <br>
    Total Features - 11 <br>
    39.4 % of data in Checking account and 18.3 % of data in Saving accounts is missing which is handled.
* **Understanding the data by performning deep Analysis**
    Use seaborn and matplot lib to see the relation, distribution of data for better understanding
* **Pre-Processing the data as per requirement**
    The data contains multiple categorical values. After splitting the data into training and testing models we encode it using One Hot Encoder <br>
    Use manual encoding technique for ordinal columns <br>
    handle Missing values using KNN Imputer and delete the features with more than 40% missing values. <br>
    Cap the outlier values imputed using min max scalar to improve accuracy on test data. <br>
* **Metric Selection**
    The objective of this project is to minimize the loss by the company. Hence we want to identify maximum clients which are indeed prone to stop paying their debts. <br> 
    Hence we are persuing low number of false negatives which is type 2 error. 
    The metric which is preffered in this case is recall to minimize the loss. <br>
* **Model Selection**
    Models considered for the project are - KNeighborsClassifier, LogisticRegression, RandomForestClassifier, NaiveBayesClassifier
    After studying individual model and tune the hyperparameters using gridsearchcv we select Multi Naive Bayes as our best fit for the given data. <br>
    Score - recall=100, Accuracy=70 <br>

An accuracy of 70 percent was reached with a recall score of 100 using Multi Naive Bayes Algorithm


 *  Data set - Kaggle Credit_risk_analysis
