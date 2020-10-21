Project Name
============

The exact goal of the model is to develop a model to predict the quality of applicants, in this case we're calling quality applicants as those who reach a particular screen of onboarding process of the application process. In this case we're only focused on the onboarding process, so definition of quality is going to be people who reach the e-sign part of onboarding process.

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

Lending companies work is to analyse the financial history of their loan applicants and they choose whether or not the applicant is risky or not. Companies can of course just organically wait for them to come to them through their website or mobile app or they can set up advertisement campaigns to reach out to those possible applicants. Other times lending companies’ partners with P2P lending marketplaces, these P2P marketplaces are web sites or companies that receive a lot of loan applications and who serve as intermediaries to link these applicants to lending companies.

Objective:
In this project we're going to assess the quality of the leads company receives from these marketplaces by predicting whether or not they're going to reach a particular screen in the process.
Product: Loan
Goal: 
The exact goal of the model is to develop a model to predict the quality of applicants, in this case we're calling quality applicants as those who reach a particular screen of onboarding process of the application process. In this case we're only focused on the onboarding process, so definition of quality is going to be people who reach the e-sign part of onboarding process.

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
parameters = {"max_depth": [None],
              "max_features": [3, 5, 7],
              'min_samples_split': [8, 10, 12],
              'min_samples_leaf': [1, 2, 3],
              "bootstrap": [True],
              "criterion": ["entropy"]}

from sklearn.model_selection import GridSearchCV
grid_search = GridSearchCV(estimator = classifier, 
                           param_grid = parameters,
                           scoring = "accuracy",
                           cv = 10,
                           n_jobs = -1)

t0 = time.time()
grid_search = grid_search.fit(X_train, y_train)
t1 = time.time()
print("Took %0.2f seconds" % (t1 - t0))


rf_best_accuracy = grid_search.best_score_
rf_best_parameters = grid_search.best_params_
rf_best_accuracy, rf_best_parameters

To-do list:

-   Ran logistic regression. Need to run other algorithm to check for better accuracy

Status
------

Model	                                     Accuracy	  Precision	Recall	   F1 Score
0	Logistic Regression	               0.562535	  0.576386	0.706432   0.634817
1	SVM (Linear)	                       0.568398	  0.577769	0.735996   0.647354
2	SVM (RBF)	                       0.591569	  0.605730	0.690871   0.645505
3	Random Forest (n=100)	               0.621720	  0.640098	0.678942   0.658948
4	Random Forest (n=100, GSx2 + Entropy)  0.625070	  0.640828	0.690353   0.664669
5	Random Forest (n=100, GSx2 + Gini)     0.630932	  0.646236	0.694502   0.669500

Random forest with Gini accuracy criteria has been selected with 63% accuracy

Inspiration
-----------

Project inspired by one of the tutorials from Udemy

Contact
-------

Created by [@sukamal01](https://github.com/sukamal01) - feel free to contact me!
