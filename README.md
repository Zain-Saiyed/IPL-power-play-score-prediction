# IPL-power-play-score-prediction

## Aim:
Our goal is to estimate the total runs made by a team in a power play of a cricket match, such as the IPL, based on a collection of factors such as cricketer and bowler names, their prior game performance and statistics, and other features.

For detailed code implementations and functionalities, refer to the provided [Project's Python notebook - _Click here_.](https://github.com/Zain-Saiyed/IPL-power-play-score-prediction/blob/main/IPL%20Power%20Play%20Prediction.ipynb)

## Features - IPL Runs Dataset

- **match_id**: Unique identifier for each match.
- **season**: The season in which the match took place.
- **start_date**: Date of the match.
- **venue**: Stadium or location where the match was played.
- **innings**: Indicates the innings number (1st or 2nd) in the match.
- **ball**: Sequence number of the ball within an over.
- **batting_team**: Team currently batting.
- **bowling_team**: Team currently bowling.
- **striker**: Batsman facing the ball.
- **non_striker**: Batsman at the non-striker's end.
- **bowler**: Bowler delivering the ball.
- **runs_off_bat**: Runs scored by the batsman without extras.
- **extras**: Additional runs scored, not off the bat (wides, no balls, byes, leg byes, penalties).
- **wides**: Wide deliveries bowled.
- **noballs**: No-ball deliveries bowled.
- **byes**: Runs scored due to byes.
- **legbyes**: Runs scored as leg byes.
- **penalty**: Runs scored from penalties.
- **wicket_type**: Type of wicket taken (caught, bowled, run-out, etc.).
- **player_dismissed**: Batsman dismissed on the delivery.
- **other_wicket_type**: Additional description of wicket type.
- **other_player_dismissed**: Additional player dismissed (if multiple dismissals occurred).

## Notebook Overview

- **Importing Necessary Packages**: Importing required libraries and setting up connections (like PyMongo for MongoDB).

- **Data Processing and Preparation**: Functions to fetch batsmen and bowler information, data padding, and data encoding.

- **Model Training**: Utilizing a Linear Regression model on IPL dataset features.

- **Model Evaluation**: Splitting data into training and testing sets, calculating Mean Squared Error (MSE) for model evaluation.

- **Saving Trained Model**: Saving the trained model and label encoder objects using joblib.

- **Prediction**: Loading the trained model and performing predictions on new data inputs.

- **MongoDB Integration**: Functions to create a MongoDB database, convert CSV files to collections, and load data from MongoDB to dataframes.

- **Main-Test Functionality**: A looped function to train the model or predict on the trained model based on user input.

## Usage

1. Install required dependencies (`pandas`, `numpy`, `scikit-learn`, etc.).
2. Load the IPL dataset and necessary statistics datasets.
3. Use the provided functions to train the model or make predictions.

## Conclusion

Through this project, we developed a predictive model for estimating power play runs in cricket matches but also streamlined the process of leveraging historical data, player statistics, and various match factors to make accurate predictions. This model extends beyond cricket, laying a firm groundwork for predictive analytics in sports. Its approach extends to broader sports domains where historical data and player performance influence outcomes. By showcasing the power of predictive analytics in sports, this project highlights the value of data-driven decision-making and its potential to revolutionize game strategies and performance evaluation in the sports industry.

<hr>

---

***
