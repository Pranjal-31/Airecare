# 🌤️ AireCare — Weather-Driven Health Risk Prediction

Predicts daily flare-up risk for Migraine, Allergy, and Joint Pain
based on Indian weather and air quality data.

## What it does
- Takes daily weather inputs (temperature, humidity, AQI,
  barometric pressure, pollen count etc.)
- Predicts risk probability for 3 health conditions
- In a real app: user selects their conditions and receives
  a morning weather-based health alert

## Tech Stack
Python · Pandas · Scikit-learn · Matplotlib · Seaborn · SQLite · SQL
## Models
- KNN, Random Forest, Gradient Boosting — one set per condition
- SMOTE for class imbalance
- GridSearchCV with StratifiedKFold for hyperparameter tuning
- Evaluated using ROC-AUC and confusion matrices

## Dataset
Synthetic dataset of 730 days built using Indian seasonal weather
patterns and known medical triggers for each condition
(AQI, barometric pressure change, temperature range, humidity)
## How to run
1. Clone the repo
2. Install requirements: pip install -r requirements.txt
3. Open AireCare_v3.ipynb in Jupyter and run all cells
## SQL Analysis
Dataset stored in SQLite — includes aggregation queries to find
seasonal risk patterns and high-risk weather combinations
