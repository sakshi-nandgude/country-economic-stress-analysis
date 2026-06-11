# Country-Level Economic Stress Monitoring and Predictive Analytics System

## Project Overview

This project analyzes global economic stress patterns using macroeconomic, demographic, and food security indicators sourced from the World Bank and FAOSTAT.

The objective is to identify countries experiencing elevated economic stress, understand the factors driving economic vulnerability, segment countries into meaningful economic groups, and evaluate whether Economic Stress Scores can be estimated using economic and agricultural indicators.

The project follows an end-to-end analytics lifecycle including business analysis, data quality assessment, exploratory data analysis, machine learning, dashboard design, and business recommendations.

---

## Business Problem

Economic stress is influenced by multiple interconnected factors including inflation, unemployment, economic growth, income levels, and food security conditions.

The primary analytical question addressed in this project is:

**Which countries exhibit higher levels of economic stress based on inflation, GDP growth, unemployment, income level, population characteristics, and food and agricultural indicators?**

---

## Project Objectives

* Identify countries with the highest economic stress levels.
* Analyze economic stress across regions and income groups.
* Investigate relationships among inflation, GDP growth, and unemployment.
* Evaluate the impact of food security indicators on economic stress.
* Segment countries into meaningful economic profiles.
* Develop a machine learning model to estimate Economic Stress Scores.
* Design an interactive Power BI dashboard for economic stress monitoring.

---

## Dataset Information

### Data Sources

#### World Bank

* GDP Growth
* Inflation
* Unemployment
* GDP Per Capita
* Population
* Food Production Index
* Region
* Income Group

#### FAOSTAT

* Cereal Yield
* Cereal Production
* Agricultural Land Percentage
* Dietary Energy Supply Adequacy

### Dataset Files

| File                        | Description                                 |
| --------------------------- | ------------------------------------------- |
| country_year_indicators.csv | Primary analytical dataset                  |
| country_metadata.csv        | Country metadata and geospatial information |
| economic_stress_score.csv   | Economic stress score components            |
| indicator_dictionary.csv    | Data dictionary and metadata                |

---

## Repository Structure

```text
country-economic-stress-analysis/

│
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
│   └── Economic_Stress_Dashboard.pbix
│
├── validation_report.json
├── .gitignore
├── LICENSE
└── README.md
```

---

## Methodology

### Phase 1: Business Analysis

* Project Charter
* Business Requirements Document (BRD)
* Data Dictionary
* Metadata Documentation

### Phase 2: Data Understanding & Data Quality Assessment

* Dataset Exploration
* Data Profiling
* Missing Value Analysis
* Duplicate Validation
* Range Validation
* Outlier Assessment

### Phase 3: Exploratory Data Analysis

* Economic Stress Distribution
* Country Rankings
* Regional Analysis
* Income Group Analysis
* Inflation, GDP Growth and Unemployment Analysis
* Food Security Analysis
* Economic Stress Driver Analysis

### Phase 4: Country Clustering

* Missing Value Treatment
* Feature Scaling
* K-Means Clustering
* Cluster Profiling
* Country Segmentation

### Phase 5: Predictive Analytics

* Random Forest Regression
* Model Evaluation
* Feature Importance Analysis

### Phase 6: Dashboard Design

* KPI Framework
* Dashboard Requirements
* Power BI Dashboard

---

## Key Findings

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

### Regional Insights

**Highest Stress Region:** Sub-Saharan Africa (58.02)

**Lowest Stress Region:** North America (35.59)

### Income Group Insights

* Low-income countries exhibited the highest economic stress.
* High-income countries exhibited the lowest economic stress.

### Strongest Drivers of Economic Stress

| Indicator                      | Relationship with Stress |
| ------------------------------ | ------------------------ |
| Unemployment                   | Strong Positive          |
| GDP Growth                     | Moderate Negative        |
| GDP Per Capita                 | Moderate Negative        |
| Dietary Energy Supply Adequacy | Moderate Negative        |
| Cereal Yield                   | Moderate Negative        |

### Food Security Insights

Countries with stronger food security and agricultural productivity generally exhibited lower levels of economic stress.

---

## Country Clustering Results

Four country segments were identified.

### Cluster 0 – Economically Vulnerable Countries

* High unemployment
* Lower GDP growth
* Lower income levels

### Cluster 1 – Economically Stable High-Income Countries

* High GDP per capita
* Low unemployment
* Strong food security

### Cluster 2 – Emerging Growth Economies

* Strong GDP growth
* Low unemployment
* Strong agricultural performance

### Cluster 3 – Economic Crisis Economies

Representative countries:

* Lebanon
* Sudan
* Zimbabwe

---

## Predictive Analytics Results

### Model

Random Forest Regressor

### Performance

| Metric   | Value |
| -------- | ----: |
| R² Score |  0.89 |
| MAE      |  3.74 |
| RMSE     |  5.40 |

### Most Important Predictors

1. GDP Growth
2. GDP Per Capita
3. Inflation
4. Unemployment
5. Food Production Index

---

## Dashboard Features

### Executive Overview

* Economic Stress Distribution
* Country Rankings
* Stress Category Analysis
* Global Economic Stress Mapping

### Regional Analysis

* Regional Comparisons
* Income Group Comparisons

### Economic Drivers

* GDP Growth Analysis
* Inflation Analysis
* Unemployment Analysis
* Correlation Analysis

### Food Security Analysis

* Food Production Analysis
* Dietary Energy Analysis
* Agricultural Productivity Analysis

### Country Clustering

* Cluster Profiles
* Country Segmentation
* Cluster Membership Analysis

### Predictive Analytics

* Model Performance
* Feature Importance
* Actual vs Predicted Results

---

## Business Recommendations

* Prioritize employment generation initiatives.
* Promote sustainable economic growth.
* Strengthen food security systems.
* Focus interventions on high-stress regions.
* Implement economic stress monitoring frameworks.
* Apply cluster-specific economic development strategies.

---

## Project Limitation

The Economic Stress Score is a derived index that incorporates several indicators used as model inputs. Therefore, predictive analytics results should be interpreted as demonstrating explanatory relationships rather than providing a pure forecasting framework.

---

## Author

Sakshi Nandgude

University of Limerick

Data Analytics Portfolio Project

2026
