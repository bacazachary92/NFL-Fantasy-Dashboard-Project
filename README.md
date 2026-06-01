# NFL Fantasy Football Dashboard

An interactive web application built with Dash and Plotly to analyze and evaluate NFL skill position players based on their fantasy football output. The tool includes volume metrics, fantasy football scoring outputs to help users identify high-value performers, track career trajectories, and benchmark team outputs to prepare for the upcoming season or go back in time to remember the old days on the grid-iron.

## Known Weaknesses of the App
- Two players named Adrian Peterson exist in the dataset
- Ignored as of 6/1/26 since it is so niche 
  (CHI 2002, MIN 2007). Known edge case, acceptable for this use case.

## Features

* **Dynamic Filters**: Select specific skill positions (`QB`, `RB`, `WR`, `TE`), statistical metrics, and individual tracking years.
* **Dynamic Cross-Filtering & Highlighting**: Selecting specific players within the scatterplot in the dropdown updates their color and size profile across all secondary visualization layers automatically.
* **Volume vs. Production Evaluation**: A scatterplot visualization mapping touches per game vs half-PPR fantasy points per game, complete with an automated Ordinary Least Squares trendline to easily flag high-efficiency values. Great for your draft! 
* **Individual Trajectory Line Graph**: Multi-player comparison line graphs which map career fantasy metrics based on the age of the selected players. Specific stats in the hover data.
* **Aggregated Team Fantasy Leaderboards**: Bar chart distributions tracking the average fantasy points output generated per position for all 32 NFL franchises and traded players (2TM, 3TM). 

## Technology Stack

* **Data Processing**: Python, Pandas, NumPy
* **Visualization Canvas**: Plotly Express
* **Application Framework**: Dash (HTML, Core Components)
* **Statistical Modeling Engine**: Statsmodels (OLS Linear Regression)

## Data Source
NFL Fantasy Football statistics dataset sourced from Kaggle.
Dataset covers seasons from 1970-2024 with half-PPR scoring.


## Getting Started
### Prerequisites
Ensure you have the required dependencies installed in your Python environment:
```bash
pip install pandas numpy plotly dash statsmodels
```

### Installation & Execution
1. Clone this repository to your local directory.
2. Ensure your cleaned player data (`nfl_clean` DataFrame source) is accessible within the application workspace.
3. Run the dashboard framework:
```bash
python app.py
```
4. Navigate to `http://127.0.0.1:505` in your web browser to open the dashboard.

Play around with the app! Pleae give feedback on what else you would like to see. Thank you! 
