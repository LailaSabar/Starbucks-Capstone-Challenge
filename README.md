# Starbucks Capstone Challenge
This project is a part of Udacity Data Science Nanodegree

### Table of Contents

1. [Project Overview](#overview)
2. [Project Components](#components)
3. [Installation](#installation)
4. [File Descriptions](#files)
5. [Instructions](#instructions)
6. [Acknowledgements](#licensing)
7. [Results](#results)
## Project Overview<a name="overview"></a>

Starbucks provided simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks. Not all users receive the same offer, and that is the challenge to solve with this data set.
The task is to combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type.


## Project Components<a name="components"></a>

The problem that I chose to solve was to build a model that predicts whether a customer will respond to an offer or not.
Here are the main steps that I followed through the analysis :  

1- Exploring and cleaning the given data sets.  
2- Combinig data sets to get a final clean data containing relevant features.  
3- Split data into training and test data sets / Scaling features.  
4- Select the appropriate performance matrix.  
5- Train the classifier and choosing the best estimator using GridSearch.    
6- Calculate features importance given by the best estimator.  
7- Compute performance of the model using test data, and plot a confusion matrix.  

## Installation<a name="installation"></a>

 - The code should run with no issues using Python versions 3.*.
 - No extra besides the built-in libraries from Anaconda needed to run this project
 - Data Processing & Machine Learning Libraries: NumPy, SciPy, Pandas, Sciki-Learn
 - Data Visualization: Matplotlib, Seaborn

## File Descriptions<a name="files"></a>

The data is contained in three files:

* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
* profile.json - demographic data for each customer
* transcript.json - records for transactions, offers received, offers viewed, and offers completed

Here is the schema and explanation of each variable in the files:

**portfolio.json**
* id (string) - offer id
* offer_type (string) - type of offer ie BOGO, discount, informational
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) - time for offer to be open, in days
* channels (list of strings)

**profile.json**
* age (int) - age of the customer 
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income

**transcript.json**
* event (str) - record description (ie transaction, offer received, offer viewed, etc.)
* person (str) - customer id
* time (int) - time in hours since start of test. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record

## Instructions<a name="instructions"></a>

1. The entire anlaysis is contained within the jupyter notebook.
2. All 3 json files should be located in data folder.


### Acknowledgements<a name="licensing">

This project was completed as part of the [Udacity Data Science Nanodegree]. The dataset used in this project contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. [Starbucks® Rewards program: Starbucks Coffee Company](https://www.starbucks.com/rewards/).

## Results<a name="results"></a>
The main observations of the code are published on medium [here](https://medium.com/@lailasb2/starbucks-capstone-challenge-b95b0931bab4)

