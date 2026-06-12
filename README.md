# Georgia County Obesity Risk Analysis
### Investigating the Impact of Socioeconomic and Behavioral Health Factors on Adult Obesity Rates

## Project Overview

Obesity remains one of the most significant public health challenges in the United States, contributing to increased risks of cardiovascular disease, diabetes, hypertension, and other chronic conditions.

This project analyzes county-level data across the state of Georgia to determine how socioeconomic and behavioral health factors influence adult obesity rates. By combining public health and socioeconomic datasets, this analysis identifies key drivers of obesity and highlights counties that may benefit from targeted public health interventions.

The project was completed as part of the WGU Master of Science in Data Analytics program.

---

## Research Question

**How do socioeconomic and behavioral health factors influence adult obesity rates across counties in Georgia, and which counties are at highest risk for elevated obesity rates?**

### Hypothesis

Counties with:

- Lower median household income
- Higher unemployment rates
- Higher smoking prevalence
- Higher levels of physical inactivity

will exhibit higher adult obesity rates.

---

## Objectives

- Analyze county-level obesity trends across Georgia.
- Evaluate relationships between socioeconomic conditions and obesity.
- Assess the impact of behavioral health indicators on obesity prevalence.
- Build predictive models to estimate obesity rates.
- Identify the most influential factors associated with obesity.

---

## Data Sources

### CDC PLACES Dataset
Provides county-level health indicators including:

- Adult obesity
- Smoking prevalence
- Physical inactivity
- Self-reported health measures

Source:
https://data.cdc.gov/

### USDA Economic Research Service

Provides county-level socioeconomic indicators including:

- Median household income
- Poverty rates
- Unemployment rates
- Population characteristics

Source:
https://www.ers.usda.gov/

---

## Tools & Technologies

| Category | Tools |
|-----------|--------|
| Programming | Python |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Modeling | Scikit-Learn |
| Environment | Jupyter Notebook |
| Version Control | Git & GitHub |

---

## Data Preparation

The project required extensive preprocessing and integration of multiple public datasets.

### Key Preparation Steps

- Imported raw CSV files
- Removed non-county observations
- Standardized county names
- Converted variables to appropriate numeric formats
- Reshaped long-format datasets into wide-format tables
- Merged CDC and USDA datasets using county identifiers
- Created a final analytical dataset for modeling

---

## Analytical Methods

### 1. Correlation Analysis

Evaluated relationships between predictor variables and obesity rates.

### 2. Multiple Linear Regression

Used to measure linear relationships between socioeconomic and behavioral health variables and obesity prevalence.

### 3. Random Forest Regression

Applied to capture nonlinear relationships and determine feature importance.

---

## Results

### Linear Regression

- R² = **0.79**
- RMSE = **1.61**

The model explained approximately 79% of the variation in county obesity rates.

### Random Forest Regression

- R² = **0.76**
- RMSE = **1.74**

The Random Forest model demonstrated comparable predictive performance while providing insights into variable importance.

---

## Key Findings

The strongest predictors of obesity rates were:

1. Physical Inactivity
2. Adult Smoking Rates
3. Median Household Income
4. Unemployment Rate

### Major Insight

Behavioral health factors—particularly physical inactivity and smoking prevalence—were more influential predictors of obesity than many socioeconomic variables.

---

## Business & Public Health Impact

The findings suggest that targeted interventions could help reduce obesity rates in high-risk counties.

Potential interventions include:

- Community fitness initiatives
- Smoking cessation programs
- Preventive health campaigns
- Expanded access to recreational facilities
- Improved healthcare accessibility

---

## Limitations

- Analysis used aggregated county-level data.
- Results identify associations rather than causation.
- Only a single year of observations was analyzed.
- Additional factors such as healthcare access and environmental conditions were not included.

---

## Future Enhancements

Future research could improve this project by:

### Longitudinal Analysis
Examining obesity trends across multiple years.

### Expanded Feature Set
Incorporating:

- Healthcare access metrics
- Educational attainment
- Environmental health indicators
- Food accessibility measures

### Advanced Modeling
Exploring:

- Gradient Boosting
- XGBoost
- Geographic clustering techniques
- Spatial analytics

---

## Repository Structure

```text
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── data_cleaning.ipynb
│   ├── exploratory_analysis.ipynb
│   └── modeling.ipynb
│
├── visuals/
│   ├── correlation_matrix.png
│   ├── regression_results.png
│   └── feature_importance.png
│
├── reports/
│   └── final_report.pdf
│
└── README.md
```

---

## Author

**Taylor Wilkerson**

Master of Science in Data Analytics (Data Engineering Concentration)  
Western Governors University

### Areas of Interest

- Healthcare Analytics
- Population Health
- Data Engineering
- Predictive Modeling
- Medical Research

---

## License

This project is intended for educational and portfolio purposes.
