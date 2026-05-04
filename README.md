# COVID-19-ANALYSIS
End-to-end COVID-19 global data analysis using Python, SQL &amp; Power BI — 1M+ rows, 50+ countries, interactive dashboards, automated data pipeline.
# 🦠 COVID-19 Global Data Analysis

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi)
![SQL](https://img.shields.io/badge/SQL-MySQL-orange?logo=mysql)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Wrangling-lightblue?logo=pandas)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

> **An end-to-end data analysis project** analyzing 1M+ rows of global COVID-19 data
> across 50+ countries — covering infection trends, recovery rates, and mortality ratios —
> using Python, SQL, and Power BI.

---

## 📌 Project Overview

This project was developed as part of a **45-day Data Analyst Internship at ThinkNext
Technologies Pvt. Ltd., Mohali**. The goal was to build a complete analytics pipeline —
from raw data ingestion to interactive dashboards — that could surface meaningful public
health insights for stakeholder reporting.

### 🎯 Objectives
- Analyze global COVID-19 spread patterns across time and geography
- Identify infection peaks, recovery trends, and mortality ratios by country and region
- Automate the data cleaning and transformation pipeline
- Build interactive dashboards for non-technical stakeholders

---

## 📊 Dataset

| Detail | Info |
|--------|------|
| **Source** | [Our World in Data — COVID-19 Dataset](https://github.com/owid/covid-19-data) |
| **Size** | 1,000,000+ rows |
| **Coverage** | 50+ countries, Jan 2020 – Dec 2023 |
| **Format** | CSV |
| **Key Columns** | `date`, `location`, `total_cases`, `new_cases`, `total_deaths`, `new_deaths`, `total_vaccinations`, `population` |

---

## 🛠️ Tools & Technologies

| Category | Tools Used |
|----------|-----------|
| **Language** | Python 3.10 |
| **Data Wrangling** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **Database** | MySQL |
| **BI Dashboard** | Microsoft Power BI |
| **IDE** | Jupyter Notebook |
| **Version Control** | Git & GitHub |

---

## 🗂️ Project Structure

---

## ⚙️ Methodology

### Step 1 — Data Collection & Loading
- Downloaded global COVID-19 dataset from Our World in Data
- Loaded 1M+ rows into Pandas DataFrame
- Initial inspection: shape, dtypes, missing value audit

### Step 2 — Data Cleaning & Transformation
- Handled missing values using forward-fill and column-mean imputation
- Standardized date formats and country name inconsistencies
- Removed duplicate records and irrelevant columns
- Engineered new features: `mortality_rate`, `recovery_rate`, `case_growth_rate`
- **Automated the full cleaning pipeline — reducing manual preparation effort by ~70%**

### Step 3 — SQL Analysis
- Loaded cleaned data into MySQL database
- Wrote optimized SQL queries using:
  - `JOIN` across country and date dimension tables
  - `Window functions` (ROW_NUMBER, RANK, LAG) for rolling averages
  - `GROUP BY` aggregations for regional summaries
  - `CTEs` for multi-step analytical logic

### Step 4 — Exploratory Data Analysis (EDA)
- Time-series analysis of infection waves (Wave 1, Wave 2, Delta, Omicron)
- Country-wise case fatality rate (CFR) comparison
- Correlation analysis between vaccination rates and case reduction
- Heatmaps showing regional outbreak intensity by month

### Step 5 — Power BI Dashboard
- Connected Power BI to cleaned CSV exports
- Built interactive dashboard with:
  - Global case map with country-level drill-down
  - Timeline slicers for outbreak wave analysis
  - KPI cards: Total Cases, Deaths, Recoveries, Vaccination Rate
  - Bar charts for top 10 affected countries
  - Trend lines comparing waves across regions

---

## 📈 Key Insights

1. **Peak outbreak periods** aligned with Winter 2020–21 and Dec 2021 (Omicron) globally
2. **India, USA, and Brazil** consistently ranked in the top 3 by total cases
3. Countries with **higher vaccination rates** showed a clear reduction in mortality ratios post-2021
4. **Mortality rate declined** from ~3.5% (early 2020) to ~0.8% (late 2022) as healthcare response improved
5. Regional analysis revealed **Europe had the most synchronized outbreak waves**, while Asia showed more fragmented patterns

---

## 🖥️ Dashboard Screenshots

> *(Add your Power BI screenshots to the `screenshots/` folder and they will appear here)*

| Dashboard Overview | Country Comparison |
|---|---|
| ![Overview](screenshots/dashboard_overview.png) | ![Comparison](screenshots/country_comparison.png) |

---

## 🚀 How to Run This Project

### 1. Clone the Repository
```bash
git clone https://github.com/rinkle-YADAV/covid19-data-analysis.git
cd covid19-data-analysis
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Download the Dataset
```bash
# Download directly from Our World in Data
wget https://covid.ourworldindata.org/data/owid-covid-data.csv -P data/raw/
```

### 4. Run Notebooks in Order

### 5. Open Power BI Dashboard
- Open `dashboard/COVID19_Dashboard.pbix` in Microsoft Power BI Desktop
- Refresh data source to point to your local `data/processed/` folder

---

## 📦 Requirements

---

## 🎓 Project Context

| Field | Detail |
|-------|--------|
| **Developed during** | Data Analyst Internship at ThinkNext Technologies Pvt. Ltd., Mohali |
| **Duration** | June 22 – Aug 6, 2025 (45 Days) |
| **Role** | Data Analyst Intern |
| **Certificate** | Grade A — Industrial Training Certificate (Cert ID: 251486) |

---

## 👩‍💻 Author

**Rinkle Yadav**
MSc Statistics & Operational Research — Kurukshetra University

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://linkedin.com/in/rinkle-yadav-402a67304)
[![GitHub](https://img.shields.io/badge/GitHub-Profile-black?logo=github)](https://github.com/rinkle-YADAV)
[![Email](https://img.shields.io/badge/Email-Contact-red?logo=gmail)](mailto:rinkleyadav91@gmail.com)

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

⭐ **If you found this project helpful, please give it a star!**
