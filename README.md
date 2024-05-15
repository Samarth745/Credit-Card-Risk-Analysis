# Credit Card Risk Analysis
![Image](https://img.freepik.com/free-vector/risk-management-concept-illustration_114360-7037.jpg?t=st=1715780785~exp=1715784385~hmac=0f11b35256075d85a7dec855271d5ea94483e4b6b55bfd883dd91d843166a73b&w=740)
## Introduction:
The Credit Card Risk Analysis project aims to build a robust machine learning model to predict the likelihood of loan repayment based on customer profiles. By leveraging data science techniques, including exploratory data analysis (EDA) and machine learning algorithms, this project provides valuable insights for financial institutions to assess credit risk accurately.

## Project Goal:
The primary goal of this project is to develop a predictive model that helps financial institutions determine whether a customer is likely to repay their loan. By analyzing various features such as age, education level, income, and debt-to-income ratio, the model aims to minimize the risk of default and optimize lending decisions.

## Skills Used:
- Python
- Exploratory Data Analysis (EDA)
- Machine Learning

## Libraries Used:
- Pandas
- Seaborn
- Scikit-learn
- NumPy
- Matplotlib

## Data Overview:
The dataset used in this project contains credit details of borrowers, including features such as age, education level, tenure with current employer, income, debt-to-income ratio, and previous default history. The dataset comprises 1000 entries and 11 features. Notably, 39.4% of data in the Checking account and 18.3% in the Saving accounts column were missing, which were handled during preprocessing.

## Data Preprocessing:
The preprocessing steps included handling missing values, encoding categorical variables using One Hot Encoder, manual encoding for ordinal columns, and outlier treatment using Min-Max Scalar. KNN Imputer was employed to handle missing values, and features with more than 40% missing values were deleted to ensure data integrity.
Preprocessing the data We will use the following steps on input sets before building a model
- Remove unwanted columns
- Split the data in Train test parts
- Encode categorical columns using OneHot Encoder
- Handling Outliers
- handling Missing Values
- Scale the columns

## Exploratory Data Analysis (EDA):
EDA was conducted using Seaborn and Matplotlib to understand the relationships and distributions within the dataset. Insights gained from EDA informed feature selection and model building.
Here we check credit amount confidance for each category
Key points that we discovered in EDA
- There is a high relation between credit amoount and duration
- In scatterplot we notice that for high credit amount we have high duration for goodloans
- Risk is highly relaated to Duration and credit amount

## Model Selection:
#### Metric 
Since our objective is to minimize company loss, predicting the risk of client default. a good recall rate is desirable because we want to identify the maximum amount of clients that are indeed prone to stop paying their debts Thus, we are pursuing a small number of False Negatives <br>

Several classification algorithms were considered for the project, including KNeighborsClassifier, LogisticRegression, RandomForestClassifier, and NaiveBayesClassifier. The models were evaluated and hyperparameters were tuned using GridSearchCV to select the best-performing model.

## Best Fit Model:
After thorough evaluation, the Multi Naive Bayes algorithm was selected as the best-fit model for the given data. It achieved an accuracy of 70% with a recall score of 100%, indicating its effectiveness in identifying clients prone to default.

## Results
#### Before 
| Algorithm                | Accuracy | Recall     |
|--------------------------|----------|------------|
| Mult Naive Bayes        | 69.0     | 100.0      |
| Bern Naive Bayes        | 68.0     | 94.117647  |
| Logistic Regression     | 69.0     | 91.176471  |
| Random Forest Classifier| 69.0     | 86.764706  |
| K-Nearest-Neighb        | 60.0     | 76.470588  |
| Gaus Naive Bayes        | 62.0     | 75.0       |

#### After FineTuning
| Algorithm                | Accuracy | Recall     |
|--------------------------|----------|------------|
| Mult Naive Bayes        | 69.0     | 100.0      |
| Random Forest Classifier| 70.0     | 92.647059  |
| K-Nearest-Neighb        | 66.0     | 91.176471  |

## Data Source:
The dataset used in this project was sourced from Kaggle under the name "Credit_risk_analysis."



## Contributing:
Contributions to this project are welcome! 
If you have any ideas for improvements or feature enhancements, feel free to open an issue or submit a pull request.


## Contact Information:
For any inquiries or feedback regarding this project, please email me [Samarth Prabhu](prabhusamarth001@gmail.com)
