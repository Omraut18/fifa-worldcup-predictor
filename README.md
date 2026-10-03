# FIFA World Cup Win Probability Predictor ⚽

A Machine Learning project that predicts the win probability of FIFA World Cup matches using historical match data and FIFA rankings.

## Project Overview

This project analyzes 49,000+ international football match results from 1872 to 2024 and FIFA ranking data to build a Random Forest classifier that predicts whether the home team wins, away team wins, or the match ends in a draw.

## Features

- Exploratory Data Analysis (EDA) with visualizations
- Filtered 1,068 actual FIFA World Cup matches from 49,000+ records
- Merged FIFA ranking points for each team at the time of the match
- Random Forest ML model for 3-class outcome prediction
- Win Probability Predictor function for any two teams using latest FIFA rankings
- Visualizations: Top 10 winning teams, goals per year trend, match outcome distribution

## Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Git

## Datasets

- `results.csv` — 49,547 international football results (1872–2024) from Kaggle
- `fifa_rankings.csv` — FIFA ranking points for all teams over time (1992–2022)
- `fifa_matches.csv` — FIFA match data with rankings
- `goalscorers.csv` — Goal scorer details per match
- `shootouts.csv` — Penalty shootout results

## Key Findings

- **Brazil** is the most winning team in World Cup history
- Average goals per match have **declined significantly** since the 1950s — modern football is more defensive
- **45.7% of World Cup matches** are home wins, showing strong home advantage
- Draws are the hardest outcome to predict — even with ranking data
- Adding FIFA ranking points as features improved away win prediction significantly

## Model Performance

- 3-class classification: Home Win, Away Win, Draw
- Accuracy: ~45% (vs 33% random baseline)
- Home win precision: 53%, Away win precision: 53%
- Draws remain difficult to predict — a known challenge in sports analytics

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

```python
predict_match("Brazil", "Argentina")

# Output:
# Brazil win probability: 46.0%
# Argentina win probability: 24.0%
# Draw probability: 30.0%
```

## Project Structure

```
fifa-worldcup-predictor/
    Ball data/
        results.csv
        fifa_rankings.csv
        fifa_matches.csv
        fifa_teams.csv
        goalscorers.csv
        shootouts.csv
        former_names.csv
    worldcup.ipynb
    README.md
```

## Author

Om Raut  
GitHub: github.com/Omraut18
