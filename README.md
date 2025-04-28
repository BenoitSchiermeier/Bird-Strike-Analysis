# FAA Wildlife Strike Data Analysis (1990–2023)

## Overview
This project analyzes the Federal Aviation Administration (FAA) dataset on wildlife strikes to civil aircraft in the United States from 1990 to 2023. It explores key trends, statistical relationships, and predictive modeling approaches to better understand the risk factors and impacts associated with wildlife strikes.

---

## Objectives
- Clean and prepare the dataset for analysis
- Conduct Exploratory Data Analysis (EDA)
- Perform hypothesis testing on important aviation variables
- Develop basic statistical models to predict bird strike occurrences
- Visualize geospatial distributions of wildlife strikes

---

## Key Steps

### 1. Data Cleaning and Preparation
- Handled missing and inconsistent data
- Converted date fields to proper datetime format
- Imputed missing continuous values (e.g., Speed, Height, Distance) using medians
- Removed duplicate entries to maintain data quality

### 2. Exploratory Data Analysis (EDA)
- Proportional trend of bird strikes by year
- State-by-state analysis of strike frequency
- Most common bird species involved in strikes
- Bird strikes by phase of flight and time of day
- Seasonal trends over the last 10 years

### 3. Hypothesis Testing
- Pearson correlation between aircraft height and speed
- Two-sample t-test comparing speed during "Approach" vs "Landing Roll" phases
- Chi-squared test between phase of flight and level of damage
- Additional t-test on height differences between damaged vs undamaged incidents

### 4. Statistical Modeling
- Built a Linear Regression model to predict bird strike incidents in the AWP FAA region (West Coast) from 1990 to 2015
- Achieved an R² of 0.95, indicating excellent model fit
- Predicted future incident counts for 2016, 2017, and beyond

### 5. Geospatial Modeling
- Created heatmaps to visualize concentration of bird strikes across the U.S.
- Generated region-specific maps for high-activity areas like California (AWP region) and the Northeast (AEA region)

---

## Major Findings
- **Temporal Trends**: Bird strike incidents have generally increased over time, peaking around 2019 and declining slightly in 2023.
- **Seasonality**: Incidents are most common during spring and summer months (especially July and August), likely related to bird migration patterns.
- **Risk Factors**:
  - Most strikes occur at lower altitudes, particularly during takeoff and landing phases.
  - Damage severity is strongly associated with phase of flight and aircraft height.
- **Geographic Hotspots**:
  - High incident concentration in metropolitan regions like California (Sacramento, San Jose, Los Angeles) and the Northeast Corridor (New York, Philadelphia, D.C.).

---

## Technologies Used
- Python (Pandas, NumPy, Matplotlib, Seaborn, Scipy, Scikit-learn, Folium)
- Jupyter Notebook (Google Colab)
- Git/GitHub for version control and collaboration
