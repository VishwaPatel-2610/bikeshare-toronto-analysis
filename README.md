# bikeshare-toronto-analysis
End-to-end ridership trend analysis of 5M+ Bike Share Toronto trips using Power BI, MySQL, and Python
# 🚲 Bike Share Toronto — Ridership Trend Analysis

## Project Overview
End-to-end analytics project analyzing **5.1 million bike-share trips** from 
Toronto (January–September 2024) to uncover ridership trends, peak demand 
periods, station utilization patterns, and behavioral differences between 
Annual Members and Casual Riders.

## Tools Used
- **Data Cleaning**: Power BI, Power Query
- **Database**: MySQL 8.0 (5.3M records)
- **SQL Analysis**: 6 query files with window functions (LAG, RANK, CTEs)
- **Visualization**: Power BI (5-page interactive dashboard)
- **Python**: pandas, matplotlib, seaborn, scipy, Prophet
- **Version Control**: GitHub

## Key Findings
- 📈 Ridership grew **321%** from January to July 2024
- ⏰ Peak hours confirmed at **8AM and 5PM** on weekdays (commuter pattern)
- 🚉 York St / Queens Quay W has utilization index of **6.99** (7x network average)
- 👤 Casual Members take **52% longer trips** than Annual Members (17.60 vs 11.62 min)
- 🔴 Anomaly days align with Canadian public holidays (Canada Day, Labour Day)
- 📅 90-day forecast projects seasonal demand decline through Q4 2024

## Dashboard Preview
![Overview Page](![Overview Page](powerbi/Screenshots/page1_overview.png)")

## Project Structure
```
bikeshare-toronto-analysis/
├── data/raw/          # Original monthly CSV files (not tracked)
├── sql/               # 6 SQL analytical query files
├── python/            # 4 Jupyter notebooks
├── powerbi/           # Power BI file + dashboard screenshots
└── docs/              # Assignment report
```

## SQL Highlights
- Window functions: LAG, RANK, SUM OVER, PARTITION BY
- Station imbalance analysis (departure vs return net flow)
- Month-over-Month growth with LAG()
- Peak hour elasticity by user type

## Python Notebooks
| Notebook | Purpose |
|---|---|
| 00_data_loading.ipynb | MySQL data pipeline (5.3M rows) |
| 01_eda.ipynb | Exploratory data analysis + statistical testing |
| 02_anomaly_detection.ipynb | Z-score anomaly detection |
| 03_forecasting.ipynb | Facebook Prophet 90-day forecast |

## Dataset
Source: [City of Toronto Open Data Portal](https://open.toronto.ca/dataset/bike-share-toronto-ridership-data/)

## Business Recommendations
1. Pre-position bikes at York St / Queens Quay W before 7:30AM weekdays
2. Create Summer Pass ($35 for June–August) to convert Casual riders
3. Implement dynamic pricing at high-imbalance stations
4. Reduce winter operations based on seasonal forecast
5. Review 423 underutilized stations for relocation opportunities
6. Create formal holiday operations policy for 7 anomaly dates

## Team
Group 5 — BIA-5440 Capstone | Humber College
- Vishwa Patel (Project Manager)
- Hasti Chandarana (Data Engineer)
- Parth Chauhan (Data Analyst)
- Lorencia Monteiro (Modelling Lead)
- Vedant Sharma (QA Specialist)
```

---

## Step 5 — Push to GitHub

Once your folder is organized open **Command Prompt** and run these commands one by one:
```
cd Desktop\bikeshare-toronto-analysis
```
```
git init
```
```
git add .
```
```
git commit -m "Initial commit — Bike Share Toronto Analysis Project"
```
```
git branch -M main
```
```
git remote add origin https://github.com/VishwaPatel-2610/bikeshare-toronto-analysis.git
```
```
git push -u origin main
