# Module 13 - classification-challenge

This challenges leverages data from an Internet Service Provider or ISP to allow for the theoretical exercise of classifying email data as either spam or not spam.  

In this exercise we will utilize both a Logistic Regression and Random Forest Classifier machine learning model and compare the results to determine which model more effectively handles the spam filtering use case. 

### Part 1 - Data verification, Training and Scaling

In the first part of the exercise we will pull the data from the UCI ML Learning library for spam data:

 Dataset Source: [UCI Machine Learning Library](https://archive.ics.uci.edu/dataset/94/spambase)

 Next we identify our target value of ```spam``` and set up the appropriate data for training.

 We will utilize the ```train_test_split``` function of the ```sklearn.model_selection``` library for training and testing our data. 

 Before running the data through a model the training and testing data will be scaled using ```StandardScaler``` from the ```sklearn.preprocessing``` library.  

 ### Part 2 - Creating and comparing the logistic regression and random forest models

The second part of our exercise creates 2 models as follows using the scaled dataset:

- A logistic regresion using ```LogisticRegression``` from the ```sklearn.linear_model``` library
- A random forest classifier using ```RandomForestClassifier``` from the ```sklearn.ensemble``` library

Once complete and trained the ```accuracy_score``` function of ```sklearn.metrics``` is used to dertermine which of the models is more accurate.
