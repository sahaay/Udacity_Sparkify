# Udacity_Sparkify

## Capstone Project
### Udacity's Data Scientist Nanodegree

### Project overview

This Project is towards Udacity's Data Scientist Nanodegree and it is about a fictional music streaming company called Sparkify, similar to companies like Spotify and Pandora. In this project, we will go through how to manipulate a big dataset to engineer relevant features for predicting customer churn and build and evaluate machine learning models using Apache Spark’s PySpark API and PySpark ML Package.
The dataset used for the project was 'mini_sparkify_event_data.json' containing data from Oct-Dec 2018 from Sparkify's platform. 

### Problem statement
Customer Churn is one of the most important metrics for businesses to evaluate. It is the percentage of customers that stopped using a company’s product or service during a certain time frame. 
This is important to keep track of because it costs more to acquire new customers than it does to retain existing customers. The goal of this project is to help Sparkify build a machine learning model that can predict when it is likely that a customer is going to churn, to be able to take action on this and prevent customers from cancelling their accounts. <> This kind of prediction model involves a binary classification problem, where a user can belong to one of two classes - churned or not churned. To solve this problem data exploration and pre-processing were done, including:
*	defining what churn is
*	exploring how churned and active users differ 
*	finding columns of interest to use in modeling, and create new features based on available data (feature engineering)
*	selecting which features are most suitable in modeling (feature selection)
*	testing different classification models to see their relevance
*	defining evaluation metrics to use to measure model performance on this dataset correctly
*	tuning hyperparameters to explore how we can improve model performance
*	evaluating the model performance and functions
*	discussing how to make further model improvements

### Installations

### Required installations:
•	Jupyter Notebook
•	Python 

### Required packages:
•	PySpark
•	NumPy
•	Pandas
•	Datetime
•	Matplotlib
•	Seaborn

### Reflection
Random Forest classifier was used to predict customer churn based on event log and user data.  Multiple variables related to event logs were recoded into new frequency variables per user, to be able to restructure the model input data to one row per unique user instead of one row per event.  The most recent event row per user was used to get the most updated data.  Categorical columns were converted into indices, one hot encoded them to separate numerical binary columns, scaled all numerical features using MinMaxScaler, and transformed all input features to one single vector to use in modeling.  Also, tested various classifiers as baseline models without any hyperparameter tuning, selected the best performing baseline model, which was a Random Forest classifier, and tuned its hyperparameters to improve the performance.  Finally, explored how to explain the model by looking at feature importances and its predictive power.
Acknowledgements
Udacity provided the data used for analysis.
