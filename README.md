# Global Climate Warming Analysis with Berkeley Earth Temperature Dataset
Data-driven analysis of 265-year global surface temperature records (1750–2015) from Berkeley Earth, hosted on Kaggle.
![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)
![Python](https://img.shields.io/badge/Python-3.8+-green.svg)
![Libraries](https://img.shields.io/badge/Libraries-pandas%20%7C%20numpy%20%7C%20matplotlib%20%7C%20seaborn%20%7C%20plotly-orange)
![Last Commit](https://img.shields.io/github/last-commit/sight-link/Global-Climate-Warming-Analysis)

## Dataset Source
Kaggle Dataset Link: https://www.kaggle.com/datasets/berkeleyearth/climate-change-earth-surface-temperature-data
Target File: `GlobalTemperatures.csv`
Data coverage: Monthly global land & combined land-ocean temperature measurements, including max/min land temperature and 95% uncertainty intervals.

## Project Goals
1. Visualize long-term global warming trends from 1850 to 2015
2. Calculate temperature anomalies using the standard 1951–1980 climate baseline
3. Compare divergent warming rates of land maximum and minimum temperatures
4. Explore seasonal warming differences across winter, spring, summer, autumn
5. Analyze decade-by-decade shifts in monthly temperature anomaly distributions
6. Quantify correlation between raw temperature values and measurement uncertainty
7. Build interactive Plotly dashboards for dynamic trend exploration

## Repository File Structure
├── Climate_Warming_Analysis.ipynb # Full Kaggle/GitHub runnable notebook
├── README.md # Project introduction & documentation
└── climate-change-earth-surface-temperature-data/ # Local downloaded dataset folder
└── GlobalTemperatures.csv

## Environment Dependencies
Install required packages before execution:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn scipy plotly




## How to Run

Option 1: Kaggle Notebook (Recommended)
Create a new Kaggle Notebook
Add dataset: climate-change-earth-surface-temperature-data via Kaggle sidebar "Add data"
Copy all code from Climate_Warming_Analysis.ipynb into notebook cells
Execute sequentially (dataset path is pre-configured for Kaggle cloud environment)

Option 2: Local Machine / GitHub
Download and unzip the Kaggle dataset into your project folder
Switch dataset loading code to the local file path (comment/uncomment path block)
Run the notebook or Python script locally

Key Visual Outputs
Global land vs land-ocean temperature trend line chart
Annual temperature curve with 10-year rolling mean & 95% uncertainty shade band
5-year rolling max/min land temperature comparison
Climate warming stripes (temperature anomaly horizontal heatmap)
Boxplot of monthly temperature anomalies grouped by decade
Seasonal warming trend multi-line plot
Correlation heatmap for temperature and measurement uncertainty
Static scatter plot of historical temperature anomalies
Two interactive Plotly time-series dashboards

Data Preprocessing Steps
Datetime parsing & year/month feature extraction
Linear interpolation to fill missing temperature records
Filter reliable post-1850 instrumental temperature data
Annual/monthly temperature aggregation
Temperature anomaly calculation (remove seasonal bias with 1951–1980 baseline)
Z-score extreme temperature detection
Min-Max normalization for standardized temperature values
Decade categorical feature creation for grouped analysis

License
Dataset: CC BY-NC-SA 4.0 (Berkeley Earth)
Project Code: MIT License
plaintext
