# NHL Expected Goals Model
A machine learning model that predicts the probability of an NHL shot resulting in a goal, built using XGBoost and trained on 4 seasons of NHL play-by-play data.

## Demo App
[Link](https://nhl-xg-app.streamlit.app/)

## Data
Play-by-play data collected from the NHL Stats API via [nhl-api-py](https://pypi.org/project/nhl-api-py/).

Features include: Distance, Angle, Shot Type, Rebound, Skater Differential, Shooting on Empty Net, Period, Overtime, Goal Differential, Goalie Save %

## Model
XGBoost classifier trained with hyperparameter tuning via RandomizedSearchCV, optimizing for Average Precision (AUCPR).

## Files
- `data_collection.ipynb` - data pipeline and feature engineering
- `shot_data.csv` - dataset of shots from the 2021-22 to 2024-25 regular seasons
- `xgboost.ipynb` - model training and evaluation