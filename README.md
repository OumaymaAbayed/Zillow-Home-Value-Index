# 🏠 Zillow Home Value Index (ZHVI) Analysis & Forecasting

This project analyzes the historical trends of the Zillow Home Value Index (ZHVI) across U.S. states, forecasts future values, and applies clustering techniques to discover patterns and similarities in housing markets.

---

## 📊 Overview

The ZHVI is a smoothed, seasonally adjusted measure of the typical home value within the 35th to 65th percentile range. It is designed to reflect the full housing stock, not just homes sold in a given period.

This project focuses on:
- Cleaning and visualizing historical ZHVI data
- Forecasting home values for the next 5 years using linear regression
- Clustering U.S. states based on their ZHVI trends using PCA and K-Means

---

## 📁 Dataset

- **Source**: [Kaggle](https://www.kaggle.com/datasets/robikscube/zillow-home-value-index/data)
- **Format**: CSV
- **Columns**: Monthly data from January 2000 onward for all 50 U.S. states + D.C.
- **Target**: `ZHVI` per state (float values)
- **Date Index**: Monthly datetime index in the format YYYY-MM-DD

---

## 🧹 Data Preprocessing

- Handled missing values using forward and backward fill
- Converted the "Month" column to datetime and set it as the index
- Renamed columns for consistency
- Normalized and cleaned string data

---

## 📈 Forecasting

- Used `LinearRegression` from `scikit-learn` to predict future home values over the next **60 months** (5 years)
- Visualized both historical and predicted trends for each state
- Calculated and compared:
  - Current growth rate
  - Forecasted growth rate
- Identified states with the **highest** and **lowest** projected changes

---

## 🔍 Clustering

- Used **Principal Component Analysis (PCA)** to reduce dimensions
- Applied **K-Means Clustering** to group states based on similar ZHVI trends
- Visualized clusters in 2D PCA space, annotated by state name

---

## 💡 Insights

- Overall increasing trend in home values across all states
- States like **California, Hawaii, and D.C.** form a distinct cluster due to extremely high and accelerating values
- Midwestern and Southern states show more stable or slower growth patterns
- Clustering helps categorize housing markets into strategic groups for policymakers or investors

---

## 📦 Dependencies

```bash
pandas
numpy
matplotlib
seaborn
scikit-learn
````
## 👩‍💻 Author
Oumaima Abaied

Contact: abaiedoumaima@gmail.com

