Project Name
============

Minimizing churn of subscription product through analysis of financial habbits

Table of contents
-----------------

-   [General info](#general-info)
-   [Technologies](#technologies)
-   [Setup](#setup)
-   [Status](#status)
-   [Inspiration](#inspiration)
-   [Contact](#contact)

General info
------------

Description of each Columns

churn  - Active = No | Suspended < 30 = No Else Churn = Yes
age - age of the customer
city - city of the customer
state- state where the customer lives
postal_code - zip code of the customer
zodiac_sign- zodiac sign of the customer
rent_or_own - Does the customer rents or owns a house 
more_than_one_mobile_device - does the customer use more than one mobile device
payFreq- Pay Frequency of the cusomter
in_collections - is the customer in collections
loan_pending - is the loan pending
withdrawn_application - has the customer withdrawn the loan applicaiton 
paid_off_loan- has the customer paid of the loan
did_not_accept_funding - customer did not accept funding
cash_back_engagement - Sum of cash back dollars received by a customer / No of days in the app
cash_back_amount - Sum of cash back dollars received by a customer
used_ios- Has the user used an iphone
used_android - Has the user used a android based phone
has_used_mobile_and_web - Has the user used mobile and web platforms
has_used_web - Has the user used MoneyLion Web app
has_used_mobile - as the user used MoneyLion  app
has_reffered- Has the user referred
cards_clicked - How many times a user has clicked the cards
cards_not_helpful- How helpful was the cards
cards_helpful- How helpful was the cards
cards_viewed- How many times a user viewed the cards
cards_share- How many times a user shared his cards
trivia_view_results-How many times a user viewed trivia results
trivia_view_unlocked- How many times a user viewed trivia view unlocked screen
trivia_view_locked - How many times a user viewed trivia view locked screen
trivia_shared_results- How many times a user shared trivia results 
trivia_played - How many times a user played trivia 
re_linked_account- Has the user re linked account
un_linked_account - Has the user un linked account
credit_score - Customer's credit score

Everyone who subscribe to company scription from the product that we're working with is one that
can provide our customers with a lot of value even if they have yet to realize the goal of the project
is to predict what users are likely to unsubscribe so that we can focus on reengage in those users.
This can be done with simple reminders that the benefits we offer them or we're creating more products
that may appeal to those users.

The challenge in this study will be working for a company that provides finance striking products to
its customers.This product comes in the shape of Christian and not just with the usual features like credit cards
or loans in financial education.We have been tasked with identifying the users or letting the castle description so that we can start
building more features that they may find value.This will in turn increase profit.
Because these finances trecking Prato we have access to customer finances as well as how they leverage
their product to handle those finances because financial data can be unreliable and delayed.

Technologies
------------

-   Python - version 3.9
-   IDE - Jupyter notebook

Setup
-----

Use "!pip install 'module' for necessary packages in Jupyter cell
i.e : !pip install pandas

Code Examples
-------------

from sklearn.model_selection import train_test_split
X_train, X_test, y_train, y_test = train_test_split(dataset.drop(columns = 'churn'), dataset['churn'],
                                                    test_size = 0.2, stratify = dataset['churn'],
                                                    random_state = 0)



To-do list:

-   Ran logistic regression. Need to run other algorithm to check for better accuracy

Status
------

Accuracy came as 63%. Project is finished

Inspiration
-----------

Project inspired by one of the tutorial from Udemy

Contact
-------

Created by [@sukamal01](https://github.com/sukamal01) - feel free to contact me!
