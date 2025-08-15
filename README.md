# PREDICTING STRUCTURAL BUILDING DAMAGE DURING EARTHQUAKE
This repository contains code for predicting building mean damage using an XGBoost regression model. The workflow includes data preprocessing, regression modeling, evaluation, and insightful data visualizations.
It cleans and processes raw building data, applies one-hot encoding to categorical features, trains a predictive model, and generates visualizations for correlations, predictions, and feature importance.

## Features
- Data Cleaning – Fixes invalid year_built values (> 2025 → 1925).
- One-Hot Encoding – Encodes categorical variables (struct_typ, occ_type).
- Model Training – Uses XGBoost for high-performance regression.
- Evaluation – Outputs Mean Absolute Error (MAE) and R² score.
- Visualizations:
  - Feature correlation heatmap
  - Actual vs Predicted damage scatter plot
  - Top 10 most important features

## Dataset
Expected CSV file:  
building_damage.csv
Columns:
- year_built – Year building was constructed  
- struct_typ – Structure type (categorical)  
- occ_type – Occupancy type (categorical)  
- meandamage – Target: mean building damage  
- Other structural/numerical features

## Requirements
pandas, numpy, seaborn, matplotlib, scikit-learn, xgboost

## How to Run
1. Open the notebook in Google Colab.
2. Install required Python packages (if running locally):
   ```bash
   pip install pandas numpy seaborn matplotlib scikit-learn xgboost

## Example Output

Sample Metrics:

Mean Absolute Error: 0.14
R-squared: 0.87


Generated Plots:

1. Correlation Heatmap
2. Actual vs Predicted Scatter Plot
3. Top 10 Feature Importances


Methodology

1. Data Cleaning – Remove extra columns and fix erroneous years
2. Preprocessing – One-hot encode categorical variables
3. Model Training – XGBoost regressor
4. Evaluation – MAE and R² metrics
5. Visualization – Heatmap, scatter plot, feature importance


Future Improvements

- Hyperparameter tuning  
- Cross-validation  
- Add seismic/geospatial features  
- Experiment with ensemble models 


# Earthquake Building Damage Prediction
# Author: https://github.com/Keerthi2427








