# Sparkify Udacity Capstone Project

### Goal

In this repository you can find the Jupyter notebook and features dataset for the Udacity Capstone Project. The goal of the same is to build a predictive model to detect users, who will cancell their subscription, before they cancel it to develop specific offers and advertisement campaigns for them.

### Required installation

The following packages/libraries are required the data loading, preprocessing and machine learning algorithm:

- Python
- Pyspark
- Pandas
- Numpy
- Matplotlib
- Seaborn

### General procedure

The code has been developed using Pyspark, since it should be scalable for the complete dataset, which has a size of 128 GB compared to the 128 MB dataset used for the local project development.

Thus, in a first step an Exploratory Data Analysis is carried out to understand the different variables and structure of the dataset. Once the provided information is understood, a churn column is created to use as label for the subsequent model.

With this churn column in mind, we have continue the EDA to find the optimal features, which can help to understand the behaviour of the churned and non-churned users.

After creating a new dataset with some engineered features, a ML model is developed testing different approaches: logistic regression, random forest and a GBT model.

Results from the first and last models look promising without great optimization.

### Original dataset

This dataset reflects user interaction with the platform. The following information is provided:
- artist
- auth
- firstName
- gender
- itemInSession
- lastName
- length
- level
- location
- method
- page
- registration
- sessionId
- song
- status
- ts
- userAgent
- userId
 
### ML features dataset

This dataset contains just one row per user with the following informations:
- Time since registration
- Mean time per day
- Mean time per session
- Mean no. of songs played per session
- Mean no. of different artist played per session
- Mean no. of interactions per session
- Gender
- Status
- Type of user: free or pay
- Distribution of pages visits

### Authors

Pablo Cosio, pca_92@hotmail.com

### Acknowledgements

Thanks to Udacity for providing the data.
