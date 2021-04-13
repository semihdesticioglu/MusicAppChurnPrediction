# Music App Churn Prediction with Pyspark on IBM Cloud Pak

![](images/customer-churn.jpg )
### Table of Contents

1. [Project Overview](#ProjectOverview)
2. [Findings on ML processes](#FindingsonMLprocesses)
3. [File Descriptions](#FileDescriptions)
4. [Instructions](#Instructions)
                          

<a name="ProjectOverview"></a>
## 1. Project Overview
In this project , I will explain my Udacity Data Scientist track graduation project: churn modelling for music app Sparkify. 

Sparkify is a fictional digital music service application for mobile phones and computers created by Udacity for some projects. It is same as with Spotify or other music streaming apps. It has same type of data as we are used to in web site event type data. When a user plays a song or open the app, all these actions are logged to database with their event types. With these data a lot of experiments can be done.

In this project , I tried to create a churn model with the given data. Creating new features on feature engineering section added valueable improvements to the model.

This project is created as a part of Udacity Data Scientist Nanodegree Program.

### Data:
In this project, we have small , medium and full datasets. I used medium size dataset (237MB) on IBM Cloud Pak solution. I used Pyspark on analysis and modelling. Spark with Hadoop is used because of big data. Using PySpark, you can work with RDDs in Python programming language and use Spark on Hadoop systems easily.

Data includes 1 json file:

1. medium-sparkify-event-data.json: Event based log data of users. I cant upload it to github since it is 237MB.


<a name="FindingsonMLprocesses"></a>
## 2. Findings & Conclusion


In this project, we had a small-medium sized event type dataset for a fictional music app. We wanted to build a churn model who quit using the app. If we can forecast these customers before they leave, we can reach them and promote some campaigns or discounts and dont lose customer. This will make company more profitable. 

Analyzing dataset and features in it show some indicators about churn. In addition to these ready tabular formatted features, we added some features that measures user behavior, consumption and attributes. Adding these extra features have made our model more solid and powerful.

In the final section, we tried some ready models from pyspark.ml library and choiced Logistic Regression algorithm with default settings. We could say our features in dataset effect our customers' churn probability increasingly or decreasingly. These weights of the features are model's parameters, the only difference is these total weights and multiplying with feature values gets into a sigmoid function and turn to a probability value for churning.

![](images/comparison.png )

In this project , we used IBM Watson Studio and its' spark&hadoop features to analyze data more easily. We used pyspark python module to reach and work in spark&hadoop systems.

Many thanks to Udacity and data providers for this project. 


<a name="FileDescriptions"></a>
## 3. File Descriptions
~~~~~~~
        MusicAppChurnPrediction
          |-- Sparkify-Feature Engineering & Modelling with IBM Cloud.ipynb    - Feature Enginering and Modelling Notebook                      
          |-- Sparkify-EDA_IBM_Cloud.ipynb  - Exploratory Data Analysis Notebook 
          |-- images
                |-- classifier.pkl    //machine learning model's best estimator prameters in a pickle file
          |-- README
          |-- Licence
~~~~~~~


<a name="Instructions"></a>
## 4. Instructions for deploying web app on local:

