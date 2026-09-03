# 🌾 Seasonal Agriculture Performance Analysis

## 📌 Project Overview

This project analyzes agricultural performance across different seasons, crops, irrigation methods and geographical regions.

The main objective is to use data analysis and visualization techniques to identify meaningful patterns in:

- Agricultural yield
- Farm profitability
- Water usage and efficiency
- Irrigation methods
- Rainfall and environmental conditions
- Crop performance
- Seasonal performance
- Regional variation
- Disease and pest risk

The analysis focuses mainly on the **Kharif, Rabi and Zaid** agricultural seasons.

---

## 🎯 Objectives

The major objectives of this project are:

1. Analyze the structure and characteristics of the agricultural dataset.
2. Clean and preprocess the data.
3. Identify and handle missing values.
4. Identify and handle duplicate records.
5. Investigate potential outliers.
6. Perform descriptive statistical analysis.
7. Perform univariate, bivariate and multivariate analysis.
8. Compare agricultural performance across seasons.
9. Analyze crop-wise performance.
10. Examine irrigation methods and water efficiency.
11. Study relationships between agricultural variables.
12. Identify meaningful insights from the data.
13. Provide evidence-based recommendations for agricultural planning.

---

## 📊 Dataset

The project uses a CSV dataset containing **4,000 agricultural records and 28 variables**.

The dataset includes information related to:

- Farm identification
- State and district
- Crop
- Agricultural season
- Farm area
- Rainfall
- Temperature
- Soil moisture
- Irrigation method
- Water usage
- Fertilizer usage
- Pesticide usage
- Yield
- Revenue
- Production cost
- Profit
- Water efficiency
- Disease and pest risk

### Seasons Analyzed

- Kharif
- Rabi
- Zaid

---

## 🧹 Data Cleaning

The following preprocessing steps were performed:

### Missing Values

Missing values were identified in:

- `Rainfall_mm`
- `Soil_Moisture_pct`
- `Yield_Tonnes_Ha`

The missing numerical values were handled using **median imputation**.

### Duplicate Records

The dataset was checked for duplicate records.

If duplicate records were identified, they were removed to avoid counting the same observation more than once.

### Outlier Investigation

Potential outliers were investigated using:

- Interquartile Range (IQR)
- Boxplots

Extreme observations were investigated rather than automatically deleted because unusually high or low agricultural values may represent genuine farming conditions.

---

## 🔎 Exploratory Data Analysis

The project includes several forms of exploratory analysis.

### 1. Univariate Analysis

Individual variables were analyzed independently.

Examples include:

- Distribution of agricultural yield
- Number of farms by season

The yield distribution shows a strong right-skewed pattern, with most observations concentrated at lower yield values and a smaller number of observations having much higher yields.

---

### 2. Bivariate Analysis

Relationships between two variables were examined.

Examples include:

- Season vs Yield
- Yield vs Water Efficiency

The Yield vs Water Efficiency analysis shows a strong positive relationship between the two variables.

---

### 3. Multivariate Analysis

Multiple agricultural performance indicators were analyzed together.

The project compares:

- Average Yield
- Average Profit
- Average Water Efficiency

across Kharif, Rabi and Zaid seasons.

Because these variables have different units and scales, normalized values were used for comparison.

---

## 📈 Key Analyses

### 🌱 Seasonal Yield Analysis

Average yield by season:

| Season | Average Yield |
|---|---:|
| Kharif | ~5.63 tonnes/ha |
| Rabi | ~5.04 tonnes/ha |
| Zaid | ~4.64 tonnes/ha |

Kharif recorded the highest average yield, while Zaid recorded the lowest.

---

### 💰 Seasonal Profitability Analysis

Approximate average profit:

| Season | Average Profit |
|---|---:|
| Kharif | ~₹1.79 lakh |
| Rabi | ~₹87,689 |
| Zaid | ~-₹24,805 |

Kharif showed the strongest average profitability, while Zaid recorded a negative average profit.

---

### 🌾 Crop Performance

Crop-wise yield analysis showed considerable differences between crops.

**Sugarcane recorded the highest average yield in tonnes/ha in the dataset.**

However, crop yield alone should not be used to determine overall agricultural performance because crops have different production requirements and economic characteristics.

---

### 💧 Irrigation Analysis

Different irrigation methods were compared using:

- Average yield
- Average profit
- Water usage
- Water efficiency

**Drip irrigation recorded an average yield of approximately 6.58 tonnes/ha and an average profit of approximately ₹2.20 lakh.**

Rainfed farming recorded the highest water-efficiency metric at approximately **7.56 tonnes/1,000 m³**.

These results indicate that irrigation performance should be evaluated using multiple indicators rather than a single metric.

---

## 💦 Yield and Water Efficiency

A scatter plot was created to study the relationship between agricultural yield and water efficiency.

The correlation coefficient is approximately:

**0.91**

This indicates a **strong positive correlation** between yield and water efficiency in the dataset.

However, correlation does not prove causation. Other factors such as crop type, rainfall, soil conditions, irrigation method and farming practices may also affect yield.

---

## 🌧️ Environmental Analysis

Environmental conditions were compared across the three seasons.

Approximate average rainfall:

| Season | Average Rainfall |
|---|---:|
| Kharif | ~849 mm |
| Rabi | ~438 mm |
| Zaid | ~305 mm |

Kharif has the highest average rainfall, while Zaid has the lowest.

Rainfall, temperature and soil moisture provide useful context for understanding seasonal differences in agricultural performance.

---

## 🗺️ State × Season Analysis

A state-by-season analysis was performed to investigate geographical variation in agricultural yield.

Some important observations include:

- Punjab records a particularly high average yield during Rabi.
- Karnataka performs strongly during Zaid.
- Maharashtra shows comparatively low Zaid yield.
- Seasonal performance varies between states.

This indicates that agricultural planning may benefit from considering both **seasonal and regional conditions**.

---

## 📊 Statistical Analysis

Statistical tests were performed to examine seasonal yield differences.

The project includes:

- One-Way ANOVA
- Kruskal-Wallis test
- Correlation analysis
- Descriptive statistics

The ANOVA p-value is approximately **0.214**, which does not reject equal seasonal means at the 5% significance level.

The Kruskal-Wallis test indicates a statistically detectable difference in the seasonal distributions/ranks.

Because the tests provide different results, the project interprets the findings carefully and avoids making unsupported causal claims.

---

## 💡 Key Insights

The major insights identified from the analysis include:

1. Kharif has the highest average yield among the three seasons.
2. Zaid has the lowest average yield.
3. Kharif has the strongest average profitability.
4. Zaid records a negative average profit.
5. Sugarcane has the highest average yield among the crops analyzed.
6. Drip irrigation records strong average yield performance.
7. Drip irrigation also records strong average profitability.
8. Rainfed farming records the highest water-efficiency metric.
9. Yield and water efficiency have a strong positive correlation of approximately 0.91.
10. Agricultural performance varies across geographical regions and seasons.

---

## 💡 Recommendations

Based on the analysis, the following recommendations are proposed:

- Use season-specific agricultural planning.
- Investigate the causes of negative profitability during Zaid.
- Consider crop selection based on multiple performance indicators.
- Evaluate efficient irrigation methods based on local conditions.
- Monitor yield, profit and water efficiency together.
- Develop region-specific agricultural strategies.
- Incorporate historical weather information into future analysis.
- Include market prices and input costs in future profitability models.
- Use multi-year data for more reliable agricultural forecasting.
- Validate causal decisions through field studies or longitudinal data.

---

## ⚠️ Limitations

The project has several limitations:

- The analysis is based on the supplied dataset.
- The dataset may not represent all agricultural regions or farms.
- Missing numerical values were handled using median imputation.
- Outliers were investigated but retained because they may represent genuine observations.
- Different crops naturally have different yield ranges.
- The dataset is observational, so correlation should not be interpreted as causation.
- Weather and market conditions can change over time.
- Additional multi-year data would improve the reliability of the findings.

---

## 🛠️ Technologies Used

### Programming Language

- Python

### Development Environment

- Google Colab
- Jupyter Notebook

### Python Libraries

- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical computation
- **Matplotlib** — Data visualization
- **SciPy** — Statistical analysis

---

## 📁 Project Structure

```text
Seasonal-Agriculture-Performance-Analysis/
│
├── README.md
│
├── seasonal_agriculture_performance_dataset.csv
│
├── Seasonal_Agriculture_Performance_Analysis.ipynb
│
└── visualizations/
    ├── seasonal_yield.png
    ├── seasonal_profit.png
    ├── crop_yield.png
    ├── irrigation_efficiency.png
    ├── yield_water_efficiency.png
    └── state_season_analysis.png
