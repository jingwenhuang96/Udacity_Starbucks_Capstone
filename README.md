# Starbucks Capstone Challenge


### Project Overview

This is a capstone project of the Data Scientist Nanodegree Program of Udacity. 

This data set contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Sometimes, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks. However, not all users receive the same offer, and that is the challenge to solve with this data set.

### Problem Statement

Problem Definition: To determine which demographic groups respond best to which offer type, with transaction, demographic and offer data. To solve this problem, we need to find a measure, that is responsive rate for each group of people. Comparing responsive rate between groups and make a suggestion about sending offers to which groups of people based on the responsive rate.

### Dataset Overview

This data set is a simplified version of the real Starbucks app because the underlying simulator only has one product whereas Starbucks actually sells dozens of products.
There is a folder call 'data' containing three files:

- portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
-  profile.json - demographic data for each customer
- transcript.json - records for transactions, offers received, offers viewed, and offers completed
Here is the schema and explanation of each variable in the files:

#### portfolio.json
id (string) - offer id
offer_type (string) - type of offer ie BOGO, discount, informational
difficulty (int) - minimum required spend to complete an offer
reward (int) - reward given for completing an offer
duration (int) - time for offer to be open, in days
channels (list of strings)

#### profile.json
age (int) - age of the customer
became_member_on (int) - date when customer created an app account
gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
id (str) - customer id
income (float) - customer's income

#### transcript.json
event (str) - record description (ie transaction, offer received, offer viewed, etc.)
person (str) - customer id
time (int) - time in hours since start of test. The data begins at time t=0
value - (dict of strings) - either an offer id or transaction amount depending on the record

The transactional data shows user purchases made on the app including the timestamp of purchase and the amount of money spent on a purchase. This transactional data also has a record for each offer that a user receives as well as a record for when a user actually views the offer. There are also records for when a user completes an offer. 


### Libraries and Dependency

Below are the library and dependency needed to run the Jupter notebook
- Pandas
- Numpy
- Math
- Json
- Matplotlib.pyplot
-Seaborn
-Sklearn
from sklearn.linear_model 
from sklearn.model_selection
from sklearn.metrics 
from sklearn.preprocessing
from sklearn.ensemble
from sklearn.tree 


### File Overview

Starbucks_Capstone_notebook.ipynb:

This notebook contains whole process of how I explore data, clean data and visualize data

'data' folder: 

- portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
-  profile.json - demographic data for each customer
- transcript.json - records for transactions, offers received, offers viewed, and offers completed

pic1 and pic2:

This picture is to display how to setup a necessary environment in case we need it


### Analysis

There is blog introducing how I analyze and visualize data: 
https://medium.com/@forever.aiqi/starbucks-capstone-challenge-4509320cad74

### Result

In the notebook, I use three classical machine learning method: Logistic regression, decision tree and random forest model

After tuning the parameter for decision tree and random forest model, the performance improves than the beginning of model, finally the decision tree shows best result among three models



