# 📊 Global Literacy & Education Trends: An Analytical Study

## 📌 Project Overview

**Global Literacy & Education Trends** is a data analytics project that explores literacy, education, illiteracy, GDP, and schooling patterns across countries and years.

The project combines multiple datasets to identify global education trends, relationships between economic development and literacy, and disparities in educational outcomes.

### 🎯 Objectives

* Analyze adult and youth literacy rates across countries.
* Study illiteracy population trends over time.
* Examine the relationship between GDP per capita and education.
* Analyze average years of schooling.
* Identify countries with significant literacy and education disparities.
* Perform exploratory data analysis using visualizations.
* Store and analyze the cleaned data using SQL.
* Answer real-world analytical questions using SQL queries.

---

## 📂 Datasets

The project uses three main datasets:

| Dataset            | Description                                   |
| ------------------ | --------------------------------------------- |
| `df_literacy`      | Adult and youth literacy rates                |
| `df_illiteracy`    | Illiterate population data                    |
| `df_gdp_schooling` | GDP per capita and average years of schooling |

The datasets are merged using common identifiers such as:

* Country
* Year

---

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Plotly**
* **SQL**
* **Jupyter Notebook / Google Colab**

---

## 🔍 Data Understanding

Each dataset is loaded into a separate Pandas DataFrame:

```text
df_literacy
df_illiteracy
df_gdp_schooling
```

The datasets are explored to understand:

* Number of rows and columns
* Data types
* Missing values
* Duplicate records
* Country and year coverage
* Numerical statistics
* Common columns available for merging

---

## 🧹 Data Cleaning

The following data-cleaning steps are performed:

* Handled missing values using appropriate methods.
* Removed duplicate records.
* Standardized country names for successful merging.
* Renamed columns for better readability.
* Checked the shape and structure of each dataset.
* Identified unusual or inconsistent values.
* Converted columns to appropriate data types.
* Filtered the data for the period **1990–2023**, or the latest available year in the dataset.

---

## ⚙️ Feature Engineering

Additional features are created where useful to improve the analysis and generate deeper insights.

Possible engineered features include:

* Literacy rate difference between male and female populations.
* Literacy rate difference between adult and youth populations.
* GDP growth rate.
* Literacy growth rate.
* Illiteracy percentage change.
* Schooling-to-GDP comparisons.
* Male–female youth literacy gap.
* Literacy improvement over time.

Additional meaningful features may be created based on the available data.

---

# 📊 Exploratory Data Analysis (EDA)

EDA is performed using **Pandas, Matplotlib, Seaborn, and Plotly**.

## 1. Univariate Analysis

Individual variables are analyzed using:

* Histograms
* Box plots
* Bar charts
* Distribution plots

Variables explored include:

* Adult literacy rate
* Youth literacy rate
* Illiteracy percentage
* Illiterate population
* GDP per capita
* Average years of schooling

## 2. Bivariate Analysis

Relationships between variables are explored using:

* Scatter plots
* Line plots
* Bar charts
* Correlation heatmaps

Examples:

* GDP per capita vs Adult Literacy
* GDP per capita vs Years of Schooling
* Adult Literacy vs Youth Literacy
* Male vs Female Youth Literacy
* Illiteracy vs Years of Schooling

## 3. Time-Series Analysis

Changes over time are analyzed to identify:

* Literacy trends
* Illiteracy trends
* GDP growth
* Changes in years of schooling
* Country-level education improvements

## 📌 Key Insights

The EDA section summarizes important findings from the visualizations, including:

* Countries with high and low literacy rates.
* Countries experiencing significant improvements in literacy.
* Relationship between economic development and education.
* Gender differences in literacy.
* Countries with high schooling but persistent illiteracy.
* Global changes in education indicators over time.

---

# 🗄️ Data Storage in SQL

The cleaned datasets are stored in a SQL database using three tables:

### 1. `literacy_rates`

Contains:

* Country
* Year
* Adult literacy rates
* Youth literacy rates
* Male youth literacy
* Female youth literacy
* Other relevant literacy indicators

### 2. `illiteracy_population`

Contains:

* Country
* Year
* Illiteracy percentage
* Illiterate population
* Other relevant indicators

### 3. `gdp_schooling`

Contains:

* Country
* Year
* GDP per capita
* Average years of schooling
* Other relevant economic/education indicators

### 🔑 Composite Key

Each table uses:

```text
(country, year)
```

as the composite key to uniquely identify country-year observations.

---

# 🧮 SQL Analysis

The following analytical queries are performed on the database.

## Literacy Rates

### 1. Top 5 Countries by Adult Literacy

Find the top 5 countries with the highest adult literacy rate in **2020**.

### 2. Female Youth Literacy

Find countries where **female youth literacy is below 80%**.

### 3. Average Adult Literacy by Region

Calculate the average adult literacy rate for each **OWID region/continent**.

---

## Illiteracy Population

### 4. Countries with High Illiteracy

Find countries where **illiteracy exceeds 20% in 2000**.

### 5. India Illiteracy Trend

Analyze the trend of illiteracy percentage in **India from 2000–2020**.

### 6. Countries with the Largest Illiterate Population

Find the **top 10 countries** with the largest illiterate population in the latest available year.

---

## GDP & Schooling

### 7. GDP and Schooling Comparison

Find countries where:

```text
Average Years of Schooling > 7
AND
GDP per Capita < 5000
```

### 8. GDP per Schooling Ranking

Rank countries based on:

```text
GDP per Capita / Average Years of Schooling
```

for the year **2020**.

### 9. Global Average Schooling

Calculate the global average number of schooling years for each year.

---

# 🔗 Join Queries

The three datasets are joined to perform more advanced analysis.

### 10. High GDP but Low Schooling

Find the top 10 countries in **2020** with:

* High GDP per capita
* Average years of schooling below 6

### 11. High Schooling but High Illiteracy

Identify countries where:

* Average years of schooling is greater than 10
* Illiterate population remains high

This helps identify potential disparities between schooling levels and literacy outcomes.

### 12. Literacy and GDP Growth

For a selected country, compare:

* Literacy rate growth
* GDP per capita growth

over the last 20 years.

### 13. Gender Literacy Gap

Calculate the difference between male and female youth literacy rates:

```text
Youth Literacy Gap =
Male Youth Literacy Rate - Female Youth Literacy Rate
```

Identify countries with significant gender gaps in youth literacy.
