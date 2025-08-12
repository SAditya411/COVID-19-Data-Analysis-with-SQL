# 📊 COVID-19 Data Analysis with SQL

## 📌 Project Overview
This project demonstrates **data cleaning, descriptive statistics, percentiles, correlation analysis, and a simple linear regression model** using COVID-19 time-series data.  
The dataset is stored in an Excel file and imported into a SQL Server database for analysis.

The analysis covers:
- Data preprocessing (handling NULL values)
- Basic statistics (min, max, sum, mean, median, mode)
- Dispersion metrics (variance, standard deviation)
- Percentiles (discrete & continuous)
- Correlation between confirmed, deaths, and recovered cases
- Ranking and ordering
- Simple linear regression to estimate deaths based on confirmed cases

---

## 📂 Files in Repository
- **`data_time_series_covid19.xlsx`** → Raw COVID-19 dataset.
- **`SQL for analysing Covid data.sql`** → SQL script for data cleaning, statistical analysis, and modeling.

---

## 🛠️ Tools & Technologies
- **SQL Server** (T-SQL)
- **Excel** (data source)
- **Data Analysis Concepts**:  
  - Descriptive Statistics  
  - Percentiles  
  - Correlation  
  - Linear Regression

---

## 🔍 Key SQL Analysis Steps
1. **Data Cleaning**
   - Check for NULL values.
   - Replace missing values with appropriate defaults (`0` for numerical values).

2. **Descriptive Statistics**
   - Calculate **min**, **max**, **sum**, **mean**, **median**, and **mode** for each month.

3. **Dispersion Analysis**
   - Compute **variance** and **standard deviation** for confirmed, deaths, and recovered cases.

4. **Percentiles**
   - Use `PERCENTILE_DISC` and `PERCENTILE_CONT` to understand case distribution.

5. **Correlation Analysis**
   - Evaluate relationships between confirmed, deaths, and recovered cases.

6. **Ranking & Ordering**
   - Identify top countries/months based on confirmed, deaths, and recovered cases.

7. **Linear Regression**
   - Estimate the relationship between confirmed cases (X) and deaths (Y):
     ```
     y = 0.0136x + 9.9926
     ```
     Meaning: Every 100 additional confirmed cases predict ~1 more death.

---

## 📊 Example Insights
- **High correlation** between confirmed cases and deaths (~0.79).
- **India in April–May 2021** recorded the highest confirmed and death cases.
- **50th percentile** of confirmed cases is much lower than the average, showing a skewed distribution.

---

## 🚀 How to Use
1. **Import Data**  
   - Load `data_time_series_covid19.xlsx` into your SQL Server database table (`dbo.Data`).

2. **Run SQL Script**  
   - Execute `SQL for analysing Covid data.sql` in SQL Server Management Studio (SSMS).

3. **View Results**  
   - Check statistical summaries, percentiles, correlations, and regression outputs.

---


