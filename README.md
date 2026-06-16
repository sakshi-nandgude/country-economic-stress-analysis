# Country-Level Economic Stress Monitoring and Predictive Analytics System

> End-to-end analytics project that analyzes global economic vulnerability using macroeconomic and food security indicators to identify high-stress countries, uncover key drivers of economic stress, segment countries into meaningful groups, and support data-driven decision-making.

## Problem Statement

Economic stress is influenced by multiple interconnected factors including inflation, unemployment, economic growth, income levels, and food security conditions. Governments, development organizations, and policy makers require reliable methods to identify economically vulnerable countries and understand the factors contributing to economic stress.

This project addresses the following business question:

**Which countries exhibit higher levels of economic stress based on inflation, GDP growth, unemployment, income level, population characteristics, and food and agricultural indicators?**

## Approach

### 1. Data Sourcing and Integration

Data was collected from:

* World Bank

  * GDP Growth
  * Inflation
  * Unemployment
  * GDP Per Capita
  * Population
  * Food Production Index
  * Region and Income Group

* FAOSTAT

  * Cereal Yield
  * Cereal Production
  * Agricultural Land Percentage
  * Dietary Energy Supply Adequacy

### 2. Data Understanding and Quality Assessment

* Data Profiling
* Missing Value Analysis
* Duplicate Validation
* Primary Key Validation
* Range Validation
* Outlier Assessment

### 3. Exploratory Data Analysis

* Economic Stress Distribution
* Country-Level Stress Rankings
* Regional Analysis
* Income Group Analysis
* Inflation, GDP Growth, and Unemployment Analysis
* Food Security Analysis
* Economic Stress Driver Analysis

### 4. Country Segmentation

K-Means Clustering was used to group countries with similar economic and agricultural characteristics.

Clusters identified:

* Economically Vulnerable Countries
* Economically Stable High-Income Countries
* Emerging Growth Economies
* Economic Crisis Economies

### 5. Predictive Analytics

A Random Forest Regression model was developed to estimate Economic Stress Scores using macroeconomic and food security indicators.

### 6. Dashboard Design

A Power BI dashboard framework was designed to support:

* Economic Stress Monitoring
* Regional Comparisons
* Food Security Analysis
* Country Clustering
* Predictive Analytics Insights

## Results

### Model Performance

* R² Score: 0.89
* MAE: 3.74
* RMSE: 5.40

### Highest Economic Stress Countries (2020–2025)

* Haiti
* Sudan
* Yemen
* Somalia
* Syrian Arab Republic
* Lebanon
* Eswatini
* Angola
* Sao Tome and Principe

### Key Business Insights

* Sub-Saharan Africa recorded the highest average Economic Stress Score (58.02).
* Low-income countries exhibited significantly higher economic stress than high-income economies.
* Unemployment was identified as the strongest positive driver of economic stress.
* GDP Growth, GDP Per Capita, Dietary Energy Supply Adequacy, and Cereal Yield were associated with lower economic stress.
* Food security indicators demonstrated a meaningful relationship with economic resilience.

## Tech Stack

| Layer                 | Tools               |
| --------------------- | ------------------- |
| Language              | Python 3.x          |
| Data Processing       | Pandas, NumPy       |
| Data Visualization    | Matplotlib, Seaborn |
| Machine Learning      | Scikit-Learn        |
| Business Intelligence | Power BI            |
| Environment           | Jupyter Notebook    |
| Version Control       | Git, GitHub         |

## Project Structure

```text
country-economic-stress-analysis/

├── data/
│   ├── country_metadata.csv
│   ├── country_year_indicators.csv
│   ├── country_year_indicators.xlsx
│   ├── economic_stress_score.csv
│   └── indicator_dictionary.csv
│
├── docs/
│   ├── Business Recommendations.docx
│   ├── Business Requirements Document.docx
│   ├── Data Dictionary and Metadata.docx
│   ├── Data Understanding Document.docx
│   ├── Executive Summary.docx
│   ├── Final Report.docx
│   └── Project Charter.docx
│
├── notebooks/
│   ├── 01_data_understanding.ipynb
│   ├── 02_data_quality_assessment.ipynb
│   ├── 03_data_preparation.ipynb
│   ├── 04_exploratory_data_analysis.ipynb
│   ├── 05_country_clustering.ipynb
│   └── 06_predictive_analytics.ipynb
│
├── dashboard/
│   └── Dashboard.pbix
│
├── validation_report.json
├── LICENSE
├── .gitignore
└── README.md
```

## How to Run

```bash
git clone https://github.com/sakshi-nandgude/country-economic-stress-analysis.git

cd country-economic-stress-analysis

pip install pandas numpy matplotlib seaborn scikit-learn jupyter

jupyter notebook
```

Open notebooks in the following order:

```text
01_data_understanding.ipynb

02_data_quality_assessment.ipynb

03_data_preparation.ipynb

04_exploratory_data_analysis.ipynb

05_country_clustering.ipynb

06_predictive_analytics.ipynb
```

## Key Findings

1. Haiti, Sudan, Yemen, Somalia, and Syria exhibited the highest levels of economic stress during the 2020–2025 period.

2. Sub-Saharan Africa recorded the highest average Economic Stress Score (58.02), while North America recorded the lowest (35.59).

3. Unemployment showed the strongest positive relationship with Economic Stress Score (0.53), indicating that labor market conditions are a major contributor to economic vulnerability.

4. GDP Growth (-0.40), Dietary Energy Supply Adequacy (-0.39), GDP Per Capita (-0.37), and Cereal Yield (-0.36) demonstrated meaningful negative relationships with economic stress.

5. Country clustering identified four distinct economic profiles, including a crisis cluster consisting of Lebanon, Sudan, and Zimbabwe.

---

*by Sakshi Nandgude*
*MSc Business Analytics, University of Limerick*
