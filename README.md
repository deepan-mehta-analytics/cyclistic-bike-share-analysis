# 🚲 Cyclistic Bike-Share Analysis

### Strategic Analysis of User Behaviour for Membership Conversion

---

## 📌 Project Overview

This project analyzes historical bike-share data from Cyclistic (Divvy Bikes) to understand behavioral differences between **casual riders** and **annual members**.

The primary objective is to identify data-driven insights that can support **marketing strategies aimed at converting casual riders into long-term members**.

This case study follows a structured data analytics workflow including **data extraction, transformation, exploratory analysis, and visualization**.

---

## 🎯 Business Objective

Cyclistic aims to increase profitability by converting casual users into members.

This analysis answers the key question:

> **How do casual riders and members use Cyclistic bikes differently, and how can this inform conversion strategies?**

---

## 📊 Dataset Description

* **Source:** Divvy Bike Share
* **Time Period:** 2019 Q1 & 2020 Q1
* **Records:** ~791,000 rides (cleaned to ~778,000 after processing)
* **Format:** CSV

### Key Fields:

* Ride ID
* Start & End Time
* Start & End Stations
* Ride Duration
* User Type (Member / Casual)

---

## ⚙️ ETL Process (Python Pipeline)

A complete ETL pipeline was developed using Python (Pandas) to ensure clean and consistent data for analysis.

### 🔹 Data Extraction

* Loaded multiple CSV datasets (2019 & 2020)
* Verified schema differences between datasets

### 🔹 Data Transformation

* Standardized column names across datasets
* Converted datetime fields into consistent format
* Merged datasets into a unified dataframe
* Created new analytical features:

  * `ride_length` (minutes)
  * `day_of_week`
  * `hour`
  * `time_period` (Morning / Afternoon / Evening / Night)
  * `ride_category` (Short / Medium / Long)

### 🔹 Data Cleaning

* Removed invalid and negative ride durations
* Filtered extreme outliers (> 90 minutes)
* Standardized user types:

  * Subscriber / Member → **Member**
  * Customer / Casual → **Casual**

---

## 📈 Exploratory Data Analysis (EDA)

The dataset was analyzed to uncover behavioral patterns across multiple dimensions:

* Ride volume distribution
* Average ride duration
* Weekly usage patterns
* Hourly ride trends
* Time-of-day segmentation
* Ride length categorization

---

## 🔍 Key Insights

### 1. Ride Distribution

Members account for approximately **92% of total rides**, indicating strong adoption among regular users.

### 2. Ride Duration

Casual users take significantly longer rides (~26 minutes) compared to members (~11 minutes), suggesting **leisure-oriented usage**.

### 3. Weekly Patterns

* Members: Consistent weekday usage
* Casual users: Peak usage on weekends

### 4. Hourly Trends

* Members: Peak during commuting hours
* Casual users: Peak during midday

### 5. Time-Based Behaviour

Casual riders show strong afternoon usage, while members demonstrate structured daily patterns.

### 6. Ride Category

* Members: Predominantly short rides
* Casual users: Higher proportion of medium and long rides

---

## 💡 Business Recommendations

Based on the analysis:

* 🎯 Target casual users during **weekends and afternoons**
* 🎯 Introduce **membership discounts for frequent long rides**
* 🎯 Offer **ride bundles or trial memberships**
* 🎯 Promote **conversion campaigns focused on leisure users**

---

## 🛠 Tools & Technologies

* **Python (Pandas, NumPy)** — ETL & Data Processing
* **Excel** — Pivot Tables & Dashboarding
* **Tableau** — Interactive Visualization
* **Jupyter Notebook** — Analysis Workflow

---

## 📁 Repository Structure

```
Google-Data-Analytics-Capstone-Cyclistic/
├── README.md
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   └── 01_cyclistic_etl_eda.ipynb
├── src/
├── results/
│   ├── excel_dashboard.xlsx
│   ├── tableau_dashboard.twbx
│   ├── presentation.pptx
├── reports/
│   └── cyclistic_case_study.pdf
└── .gitignore
```
### 📊 Excel Dashboard

Due to file size limitations, the full Excel dashboard is available here:

👉 [View Excel Dashboard](https://docs.google.com/spreadsheets/d/1FFkyD4qh74p4Z9GKBIELzyRPFqUm7nsd/edit?usp=sharing&ouid=105860754497024281787&rtpof=true&sd=true)
---

## 📊 Visualizations

Key visualizations include:

* Ride count distribution by user type
* Average ride duration comparison
* Weekly and hourly usage trends
* Time period segmentation
* Ride category distribution

(See `/results/` folder for full dashboards and charts)



## 📌 Project Outcome

This project demonstrates:

* End-to-end data analytics workflow
* Real-world ETL pipeline design
* Behavioral segmentation analysis
* Multi-tool data visualization
* Business-driven insight generation

---

## 🚀 Future Improvements

* Integration with cloud platforms (GCP / BigQuery)
* Automation of ETL pipeline
* Real-time data streaming analysis
* Predictive modeling for user conversion

---

## 👤 Author

**Deepan Mehta**
Data Analytics | Future Data Engineer

---
