# STARBUCKS

In this project I would be exploring the starbuck and created a machine learning model that predict theh offer a person recieves from starbucks and if the individual complete their orders. There are 3 dataset to be explored in this project. The data in this project was downloaded here. The result of this project would give insight to people that want to get into the business of shortlet to understand how prices are determined and factors that affect it

# ACKNOWLEDGE

## DATA CREDIT

UDACITY 

STARBUCK

# PROJECT MOTIVATION
This project is meant to answer some questions that stakeholders would have about the different promo offers that starbuck offers, giving clearity to the conversion rate of the promo

# DATA UNDERSTANDING

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

https://medium.com/@madurichard09/starbucks-capstone-project

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

# DATA PREPARATION

Dealing with incorrect data type: The became_member_on column in the profile.json file is strings. 

Missing Values: The missing values in the gender column of the profile.json file was replaced by the mode gender. Also the income column in the same dataset has missing variable which was replaced with the mean income


# LIBRARIES USED

The following libraries were used to excute this project

> 1. Numpy

> 2. Pandas

> 3. Matplot

> 4. Seaborn

> 5. Scikit Learn

> 6. stat.model

## Installations:

This libraries work in latest python and they can be installed by running this code

pip install -r requirement.txt

# SUMMARY OF THE RESULTS

Firstly I built a modle that predicts the event 

The acccuracy for individual model are as follows:

	Model	Accuracy Score

0	KNN	0.741303

1	RANDOM FOREST	0.716042

2	ADA BOOST	0.724038

3	Naive Bayes	0.454262

Secondly I built a model that predicts the event

The acccuracy for individual model are as follows:


Model	Accuracy Score

0	KNN	0.741303

1	RANDOM FOREST	0.716042

2	ADA BOOST	0.724038

3	Naive Bayes	0.454262
