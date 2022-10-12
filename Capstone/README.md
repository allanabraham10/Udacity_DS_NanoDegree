# Udacity Starbucks Capstone Project

![image](https://user-images.githubusercontent.com/69242466/195322414-c73d1402-3353-43c1-8cda-4539fd19d6d2.png)

## Installations
Here are the different packages used for this project:

Numpy, Pandas, Sklearn

Matplotlib, Seaborn. Json

## Overview and Motivation

Starbucks, one of the world’s most popular coffee shops, frequently provides offers to its customers through its rewards app to drive more sales. These offers can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free).

**Motivation:** The goal of this project is to find some factors and build a machine learning(ML) that predicts what makes a customer complete an offer(regardless of the offer type). I am mostly interested in the demographics as I believe that they are bigger factors than the offer types.

Firstly, to best analyze the data thoroughly, Exploratory Data Analysis(EDA) is performed to find the data representations & characteristics. In this step, I will get to know the data better, as well as clean it. Secondly, with the data provided, I will answer the above questions with the help of charts and various ML models which will be fed the data from a merged dataset which consists of the following: portfolio, profile, transactional.

## Datasets

For this project, the data sets are provided by Starbucks and Udacity in the form of three JSON files. These contains simulated data that mimics customer behavior on the Starbucks rewards mobile app.

- portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.) (provided by Udacity)
- profile.json - demographic data for each customer (provided by Udacity)
- transcript.json - records for transactions, offers received, offers viewed, and offers completed (provided by Udacity)
- Starbucks_Capstone_notebook.ipynb: Jupyter Notebook with the full project spine.


Here are the schema and explanation of each variable in the files:

**portfolio.json**
-   id (string) - offer id
-   offer_type (string) - type of offer ie BOGO, discount, informational
-   difficulty (int) - minimum required spend to complete an offer
-   reward (int) - reward given for completing an offer
-   duration (int) - time for offer to be open, in days
-   channels (list of strings)

**profile.json**

-   age (int) - age of the customer
-   became_member_on (int) - date when customer created an app account
-   gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
-   id (str) - customer id
-   income (float) - customer's income

**transcript.json**

-   event (str) - record description (ie transaction, offer received, offer viewed, etc.)
-   person (str) - customer id
-   time (int) - time in hours since start of test. The data begins at time t=0
-   value - (dict of strings) - either an offer id or transaction amount depending on the record.

## Conclusion
The LGBM Classifier not only scored the highest f1-score with 0.58 which is the metric we have chosen to analyze the performance on test data, but also scored the highest accuracy. Therefore, I used this model to find the factors that can predict whether or not a customer will complete an offer.

After fine tuning the model, I found that the top 3 most important features that impacts a customer completing an offer is the time taken to act on it, the customer's income and the year the customer became a member.

## Medium Article
For a more detailed version on the project, please visit https://medium.com/@pa.allan10/starbucks-rewards-mobile-app-a-udacity-capstone-project-5e4a7451667a

## Acknowledgements
I would like to express my since thanks to Udacity for all their guidance and resources for the Data Science Nano Degree Program.
I would also like to express my gratitude to fellow Stack Overflow contributors who help make the debugging super easy.
