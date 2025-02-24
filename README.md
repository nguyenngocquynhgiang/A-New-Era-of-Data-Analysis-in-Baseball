
---

# The Statcast Revolution

## Introduction
This project explores the impact of Statcast, a cutting-edge baseball tracking system, by analyzing data from two of MLB's most prolific sluggers: **Aaron Judge** and **Giancarlo Stanton**. Using **pandas**, **matplotlib**, and **seaborn**, we will wrangle, visualize, and compare their hitting statistics.

## About Statcast
Statcast is a high-tech system that utilizes cameras and radar to measure baseball and player movements with extreme precision. Since its introduction in 2015, it has revolutionized how teams analyze performance, leading to a data-driven approach to the game.

## Data Description
The dataset contains Statcast records from **2015 to 2017** for:
- **Aaron Judge** (`judge.csv`)
- **Giancarlo Stanton** (`stanton.csv`)

Each row in the dataset represents a pitch thrown to a batter, with information on:
- **Pitch data**: velocity, spin rate, movement
- **Hit data**: exit velocity, launch angle, distance
- **Game context**: inning, score, runners on base

## Analysis Overview
1. **Data Wrangling & Exploration**  
   - Load the dataset using `pandas`
   - Inspect key features

2. **Comparing Batted Ball Events**  
   - Analyze event counts (home runs, strikeouts, walks, etc.)  
   - Compare Judge’s and Stanton’s tendencies at the plate  

3. **Home Run Analysis**  
   - **Launch Angle vs. Exit Velocity**  
     - Scatter and density plots for home runs  
   - **Pitch Velocity Distribution**  
     - Box plots comparing how fast pitches were when homers were hit  
   - **Pitch Location & Heatmaps**  
     - 2D strike zone analysis  

## Key Findings
- **Judge vs. Stanton Differences**: Judge strikes out and walks more, while Stanton puts more balls in play.
- **Home Run Profiles**: Judge hits home runs off faster pitches, while Stanton's power is more evenly distributed.
- **Launch Angles & Exit Velocities**: Slight differences suggest unique approaches at the plate.

## Dependencies
Ensure you have the following Python libraries installed:
```bash
pip install pandas matplotlib seaborn
```

## Running the Analysis
To execute the analysis, run the following script in a Jupyter Notebook:
```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load datasets
judge = pd.read_csv('datasets/judge.csv')
stanton = pd.read_csv('datasets/stanton.csv')

# Display last 5 rows
print(judge.tail())
```
For full visualizations, follow the notebook’s step-by-step analysis.

## Conclusion
Statcast has transformed baseball analytics by providing unprecedented insight into player performance. This project showcases how data science can reveal intricate details about elite hitters like Aaron Judge and Giancarlo Stanton.

---

This README gives a clear, structured overview of your project. Let me know if you'd like any refinements! 🚀
