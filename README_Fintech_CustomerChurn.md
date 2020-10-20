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
