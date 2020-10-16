# Project Name
Portfolio return calculation using Capital Asset Pricing Model

## Table of contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Setup](#setup)
* [Status](#status)
* [Inspiration](#inspiration)
* [Contact](#contact)

## General info
CAPM is the model that describes the relationship between the expected return and risk of securities
S&P500 is being used as benmark index.
Stock prices of 8 stocks has been considered from January 2012 to April 2020

python's plotly.express for interactive chart

## Technologies
* Python - version 3.9
* IDE - Jupyter notebook


## Setup
Use "!pip install 'module' for necessary packages in Jupyter cell
i.e : !pip install plotly

## Code Examples
Calculating Daily return
# Function to calculate the daily returns 
def daily_return(df):
  df_daily_return = df.copy()
    # Loop through each stock
  for i in df.columns[1:]:
    # Loop through each row belonging to the stock
    for j in range(1, len(df)):
      # Calculate the percentage of change from the previous day
      df_daily_return[i][j] = ((df[i][j]- df[i][j-1])/df[i][j-1]) * 100
    # set the value of first row to zero, as previous value is not available
    df_daily_return[i][0] = 0
  return df_daily_return

Calculate beta and alpha

------

To-do list:
* I have used equal weights for the portfolio, can be optimized further with monte carlo simulation

## Status
Project is finished


## Inspiration
Project inspired by one of the tutorial from Udemy by Dr. ryan

## Contact
Created by [@sukamal01](https://github.com/sukamal01) - feel free to contact me!