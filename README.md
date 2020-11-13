# Udacity_Sparkify

## Capstone Project
### Udacity's Data Scientist Nanodegree

### Project overview

This Project is towards Udacity's Data Scientist Nanodegree and it is about a fictional music streaming company called Sparkify, similar to companies like Spotify and Pandora.  In this project,the task was to manipulate a big dataset to engineer relevant features for predicting customer churn and build and evaluate machine learning models using Apache Spark’s PySpark API and PySpark ML Package.
The dataset used for the project was 'mini_sparkify_event_data.json' containing data from Oct-Dec 2018 and supplied by Udacity. 

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
Decision Tree classifier was used to predict customer churn based on event log and user data.  Multiple variables related to event logs were recoded into new frequency variables per user, to be able to restructure the model input data to one row per unique user instead of one row per event.  The most recent event row per user was used to get the most updated data.  

Categorical columns were converted into indices, one hot encoded them to separate numerical binary columns, scaled all numerical features using MinMaxScaler, and transformed all input features to one single vector to use in modeling.  

Also, tested various classifiers as baseline models without any hyperparameter tuning, selected the best performing baseline model, which was a Decision Tree classifier, and tuned its hyperparameters to improve the performance.  

Finally, explored how to explain the model by looking at feature importances and its predictive power.

A blog post detailing the approach and output is [here](http://kya-re.blogspot.com).

The code used for executing this project is [here](https://github.com/sahaay/Udacity_Sparkify.git).


### Acknowledgements
#### Dataset was supplied by [Udacity](http://udacity.com).

