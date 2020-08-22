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
- XGBoost 1.2.0
- datetime
- Jupyter Notebook(only if running locally)

## Results

The final results from the three models are presented below. The main metric considered here is the F1 score, with the Logistic Regression having the highest one. However, the results are similar across the board.

```
╔═══════════╦═══════════╦═══════╦════════╗
║   Metric  ║Logistic   ║Random ║XGBoost ║
║           ║Regression ║Forest ║        ║
╠═══════════╬═══════════╬═══════╬════════╣
║ Accuracy  ║   0.585   ║ 0.576 ║ 0.590  ║
║ Precision ║   0.583   ║ 0.584 ║ 0.620  ║
║ Recall    ║   0.583   ║ 0.519 ║ 0.472  ║
║ MSE       ║   0.415   ║ 0.424 ║ 0.410  ║
║ F1 Score  ║   0.583   ║ 0.550 ║ 0.534  ║
╚═══════════╩═══════════╩═══════╩════════╝
```

The most important features recognized are Shot Distance, Game Clock, Shot Clock and Closest Defender Distance.

For a full article documenting the results, please refer to the blog post [here](https://medium.com/@b_ivanov/predicting-nba-shots-943b07975995).

## Suggested Improvements

1. Gather further data for Margin and Outcome at the point of the shot i.e. what is the point margin between the teams and what team is winning when the shot is made. Those could potentially be extremely useful fields as players can potentially feel pressured to take riskier and quicker shots if they are currently losing the game.

2. Additional data points around the effectiveness of the players in both offense and defense could potentially be extremely valuable as predictors. Statistics such as FG%, 2 Point %, and 3 Point % as a starting point could help us evaluate players effectiveness on the offensive end. Additionally, some states such as steals and blocks can help us evaluate the player's ability to defend. The analysis above excluded the player's effect and focused mainly on the technicalities behind the shot, however, the ability of the player could be a very important determining factor here.

3. Explore further parameters for the models. I have tried optimizing it with a few parameters, however, there is further opportunity to improve and experiment here.

3. Try different models to classify the shots. I have used the 3 most popular classifiers, however, with more data points we could expand the analysis further and try models such as Support Vector Machine or Neural Networks.

# Acknowledgements
The data has been taken from [Kaggle](https://www.kaggle.com/dansbecker/nba-shot-logs)
