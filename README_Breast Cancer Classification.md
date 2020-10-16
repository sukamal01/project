Project Name
============

Breast cancer classification project with Support Vector Machine Algorithm

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

Predicting if the cancer diagnosis is benign or malignant based on several observations/features.

-   30 features are used, examples:
    - radius (mean of distances from center to points on the perimeter)
    - texture (standard deviation of gray-scale values)
    - perimeter
    - area
    - smoothness (local variation in radius lengths)
    - compactness (perimeter^2 / area - 1.0)
    - concavity (severity of concave portions of the contour)
    - concave points (number of concave portions of the contour)
    - symmetry
    - fractal dimension ("coastline approximation" - 1)

-   Datasets are linearly separable using all 30 input features
-   Number of Instances: 569
-   Class Distribution: 212 Malignant, 357 Benign
-   Target class:
    - Malignant
    - Benign

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

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.model\_selection import train\_test\_split
from sklearn.svm import SVC
from sklearn.metrics import classification\_report, confusion\_matrix
from sklearn.model\_selection import GridSearchCV
X\_train, X\_test, y\_train, y\_test = train\_test\_split(X, y, test\_size = 0.20, random\_state=123)

Used 20% of the data as test data to predict
--------------------------------------------

To-do list:

-   Can be further enhanced with openCv and deep learning network with the help of image processing

Status
------

Project is finished

Inspiration
-----------

Project inspired by one of the tutorial from Udemy by Dr. ryan

Contact
-------

Created by [@sukamal01](https://github.com/sukamal01) - feel free to contact me!
