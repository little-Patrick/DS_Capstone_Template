# Traffic Accident Analysis Project

![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)
![pandas](https://img.shields.io/badge/pandas-Data%20Analysis-yellow.svg)
![numpy](https://img.shields.io/badge/numpy-Numerical%20Computing-orange.svg)
![matplotlib](https://img.shields.io/badge/matplotlib-Visualization-green.svg)
![seaborn](https://img.shields.io/badge/seaborn-Statistical%20Plots-blueviolet.svg)
![statsmodels](https://img.shields.io/badge/statsmodels-Statistical%20Modeling-lightgrey.svg)

## Overview
This project analyzes US traffic accident data to identify key factors influencing accident frequency and severity. The insights aim to inform safety interventions, infrastructure improvements, and policy recommendations to reduce accidents and improve public safety.

## Business Understanding
### Goals
- **Economic Impact**: Reduce costs associated with medical expenses, property damage, and lost productivity.
- **Public Safety**: Mitigate accident-prone conditions to improve citizen safety and reduce fatalities.
- **Infrastructure Prioritization**: Allocate budgets effectively to high-risk areas.
- **Policy Development**: Inform new safety regulations and evaluate existing programs.

### Stakeholders
- **Primary Stakeholders**: Department of Transportation (DOT), Congress, Local Governments.
- **Secondary Stakeholders**: Law Enforcement Agencies, Emergency Services, Public.

## Analytical Questions
1. What environmental factors are most strongly correlated with traffic accidents?
2. Which geographic regions experience the highest frequency and severity of accidents?
3. How do accident trends vary by time of day, day of the week, and season?
4. What infrastructure or road conditions contribute to accident severity?
5. Can derived features like accident duration or time of occurrence help predict accident severity?

## Data Understanding
The dataset includes detailed records of traffic accidents across the United States, with features such as:
- **Environmental Factors**: Weather, visibility, precipitation.
- **Geographic Data**: State, city, latitude, longitude.
- **Temporal Data**: Start time, end time, day of the week.
- **Severity Levels**: Accident severity ranging from minor to severe.

## Methodology
1. **Data Cleaning**:
   - Dropped columns with excessive missing values.
   - Imputed missing values for numerical and categorical columns.
   - Removed outliers using the IQR method.
   - Converted date columns to datetime and categorical columns to category type.
2. **Feature Engineering**:
   - Created derived features such as accident duration and day of the week.
3. **Exploratory Data Analysis (EDA)**:
   - Visualized accident patterns across dimensions like time, geography, and severity.
   - Analyzed correlations between variables.
4. **Statistical Analysis**:
   - Conducted Chi-Square tests, ANOVA, and regression analysis to validate patterns.

## Key Findings
1. **Day of the Week**: Accident severity is slightly higher on weekends.
2. **Environmental Factors**: Weak correlations suggest human behavior and infrastructure play larger roles.
3. **Geographic Trends**: States like California, Texas, and Florida have the highest accident frequencies.
4. **Rush Hours**: Accident frequency peaks during morning and evening rush hours.
5. **Severity Patterns**: Longer distances traveled are associated with higher accident severity.

## Recommendations
1. **Targeted Safety Measures**:
   - Increase enforcement and public awareness campaigns during weekends.
2. **Infrastructure Improvements**:
   - Prioritize funding for high-accident states and address localized issues.
3. **Rush Hour Management**:
   - Implement staggered work hours and adaptive traffic signals.

## Next Steps
1. **Expand the Dataset**:
   - Analyze the full dataset and include additional variables like vehicle types and road conditions.
2. **Advanced Modeling**:
   - Use machine learning models to predict accident severity and identify influential factors.
3. **Policy Recommendations**:
   - Collaborate with stakeholders to implement and monitor interventions.

## Tableau Dashboard
The cleaned dataset has been exported for use in Tableau to create an interactive dashboard. The dashboard allows users to:
- Explore accident patterns across dimensions.
- Filter data by state, severity, and time.
- Visualize key insights and recommendations.

## How to Run the Notebook
1. Install the required Python libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn statsmodels
   ```
2. Open the Jupyter Notebook `DS_Capstone_Notebook.ipynb`.
3. Run all cells sequentially to reproduce the analysis.