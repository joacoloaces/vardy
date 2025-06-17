# ⚽ Analysing Jamie Vardy’s 2015–16 Leicester City Season

This project is a data-driven analysis of Jamie Vardy’s remarkable 2015–16 Premier League season with Leicester City, using event data from StatsBomb. The aim is to uncover performance trends, goal-scoring patterns, and key factors behind his historic goal surge.

## 🧩 Project Overview

- **Player**: Jamie Vardy  
- **Season**: 2015–16  
- **Team**: Leicester City (Premier League Champions)  
- **Focus**: Shot efficiency, goal timing, movement, and contextual features influencing Vardy’s goals during that season.

## 🔍 Objectives

1. Quantify Vardy’s goal-scoring efficiency and how it compared within Leicester and across the Premier League.
2. Analyze spatial and contextual shot features (e.g., distance, angle, build-up context).
3. Detect patterns such as high-scoring streaks and underappreciated goal types.
4. Perform a time series analysis of his goals over the season.
5. Derive actionable insights into the playing style that drove Leicester's title-winning campaign.

## 📊 Data & Tools

- **Data source**: StatsBomb event data (Premier League 2015–16) via `statsbombpy`.
- **Key events**: shots, carries, passes, positional data tied to Vardy.
- **Python libraries**: pandas, numpy, matplotlib/seaborn, scikit-learn, statsbombpy.

## 🧠 Methodology

1. **Data Extraction**  
   - Pulled all match events involving Leicester.
   - Filtered to Vardy’s shots (filtered by player name/ID).

2. **Feature Engineering**  
   - Computed shot angle & distance to goal.
   - Included contextual flags: open play, counter-attack, press intensity.

3. **Shot Performance Analysis**  
   - Shot map visualization across matches.
   - Distribution of shot distances, angles.
   - Time-based exploration (e.g., streaks of scoring games).
  
4. **Pressure Performance Analysis**  
   - Pressure map visualization across matches.
   - Influence in ball recovery
