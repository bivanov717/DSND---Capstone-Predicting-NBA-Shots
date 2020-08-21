# NBA Shot Prediction

## Project motivation
In this repo you'll find a sample code that anlyses NBA Shot Logs and tests two machine learning modules to predict if a shot is going to be successful. The two main questions that I was interested into analyzing and answering are : 

1. What are the most important factors to consider for a shot to be successful?
2. Can we use the general data provided behind each shot to predict if a shot is going to be made?

## File Description

For this project there are:
-	one data file - NBA Shot Logs.csv
-	one notebook available - NBA Shot Logs Analysis.ipynb

## Requirements

- Pandas v1.0.3
- Numpy v1.18
- Matplotplib v3.2.1
- Seaborn v0.10.1
- Scikit-Learn v0.224
- XGBoost 1.20=.0
- datetime
- Jupyter Notebook(only if running locally)

## Results

The analysis helped come to the following conclusions:
1. Lead time appears to be about 100 days for all holidays, with family holidays having slightly shorter lead time, compared to non-family. The price and lead time have a small negative correlation.
2. The main explanatory variables for price (Average Daily Rate) appear to be Reserved Room Type, Assigned Room Type and Market Segment.
3. The bookings are predominantly spread within the summer months, with a fall down in the winter.

## Suggested Improvements


## Blog Post
A full blog post describing the results can be found [here](: 


# Acknowledgements
The data has been taken from [Kaggle](https://www.kaggle.com/dansbecker/nba-shot-logs)
