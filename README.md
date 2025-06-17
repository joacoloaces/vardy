# ⚽ Expected Goals (xG) Model with StatsBomb Data

This project explores the development of an Expected Goals (xG) model using open event data provided by [StatsBomb](https://statsbomb.com/). The goal is to estimate the probability of a shot resulting in a goal based on multiple contextual and spatial features.

## 🔍 Objective

Build a logistic regression model that predicts the probability of scoring for every shot taken in a match, considering factors like:

- Shot location (x, y coordinates)
- Shot type (e.g., open play, set piece)
- Body part used
- Pressure from defenders
- Shot angle and distance

## 📊 Data

The data comes from StatsBomb's publicly available datasets, accessed using the [`statsbombpy`](https://github.com/statsbomb/statsbombpy) Python package. The main dataset used includes shot-level event data from multiple matches.

## 🧠 Methodology

1. **Data Collection**  
   Downloaded and combined event-level data for several matches.

2. **Feature Engineering**  
   Created custom variables such as:
   - Shot angle and distance to goal
   - Game state (winning/losing/drawing)
   - Shot pressure
   - Goalkeeper position (if available)

3. **Modeling**  
   Trained a **logistic regression model** using scikit-learn to estimate xG values for each shot.

4. **Evaluation**  
   - Used AUC-ROC and Brier Score to evaluate model performance.
   - Visualized xG distribution, calibration curves, and residuals.

5. **Insights**  
   - Identified which features are most predictive.
   - Highlighted players and teams that over/under-perform their xG.

## 📎 Dependencies

- Python 3.8+
- pandas
- numpy
- matplotlib / seaborn
- scikit-learn
- statsbombpy
- shap (optional, for feature importance)

Install them using:

```bash
pip install -r requirements.txt
