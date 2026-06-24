# FIFA World Cup Win Probability Predictor  ⚽

A Machine Learning project that predicts the win probability of teams in FIFA World Cup matches based on match statistics like possession, shots, fouls, and expected goals (xG).

## Project Overview

This project analyzes historical FIFA World Cup match data from 1974 to 2022 and builds a Random Forest classifier to predict whether the home team will win a match based on in-game statistics.

## Features

- Exploratory Data Analysis (EDA) with visualizations
- Feature Engineering to create target variables
- Random Forest ML model with 77% accuracy
- Win Probability Predictor function for any two teams
- Feature Importance analysis to find what stats matter most

## Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Dataset

FIFA World Cup Enhanced Dataset (1974-2022) sourced from Kaggle.
Contains match statistics including possession, shots, shots on target, fouls, yellow cards, red cards, expected goals (xG), and attendance.

## Key Findings

- The model achieved **77% accuracy** on test data
- **Fouls, shots on target, and away fouls** were the top 3 most important features for predicting a win
- Home teams win more frequently than away teams in World Cup matches
- 1982 World Cup had the highest average goals per match

## How to Run

1. Clone this repository
```bash
git clone https://github.com/Omraut18/fifa-worldcup-predictor.git
```

2. Install required libraries
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

3. Open `worldcup.ipynb` in VS Code or Jupyter Notebook and run all cells

## Win Probability Predictor

You can predict win probability for any match by calling:

```python
predict_win_probability(
    possession_home=55, possession_away=45,
    shots_home=14, shots_away=10,
    shots_ontarget_home=6, shots_ontarget_away=4,
    home_xg=1.8, away_xg=1.2,
    fouls_home=12, fouls_away=14,
    yellow_cards_home=1, yellow_cards_away=2
)
```

## Project Structure

```
fifa-worldcup-predictor/
    Ball data/
        fifa_world_cup_enhanced_1974_2022.csv
    worldcup.ipynb
    README.md
```

## Author

Om Raut
