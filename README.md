# HR Attrition Analysis — Exploratory Data Analysis & Dashboard

---

## Overview

Employee attrition is one of the most expensive and least understood problems in HR. Which roles are actually losing people the fastest? Is attrition a tenure problem, a workload problem, or both? And where should retention efforts actually be focused?

This project explores IBM's public HR Analytics dataset covering 1,470 employees across 35 attributes, using Python, SQL, and Tableau to identify where attrition concentrates and what drives it.

---

## Key Findings

- Overall attrition rate is 16.1%, the baseline every department, role, and segment is measured against
- Sales (20.6%) and HR (19.0%) run above that baseline; Research & Development, the largest department, runs below it at 13.8%
- Department-level numbers hide the real problem: Sales Representatives leave at 39.8%, nearly 2.5x the company average and the single highest-risk role in the dataset
- Attrition is heavily front-loaded by tenure — employees in their first 0-2 years leave at 29.8%, compared to just 8.1% for employees with 10+ years
- OverTime is the strongest behavioral signal in the dataset — employees working overtime leave at 30.5%, nearly triple the rate of those who don't (10.4%)
- No single numeric factor dominates in a full correlation pass; tenure-related measures cluster together as the next-strongest signals, but attrition here is best explained by overlapping factors rather than one root cause

---

## Charts

| Chart | Description |
|-------|-------------|
| 01_overall_attrition.png | Company-wide attrition split, the baseline for every comparison below |
| 02_department_role_attrition.png | Attrition rate by department and by job role, side by side |
| 03_tenure_attrition.png | Attrition rate across tenure bands (0-2, 3-5, 6-10, 10+ years) |
| 04_overtime_attrition.png | Attrition rate comparison between employees working overtime and those who aren't |

---

## Live Dashboard

Interactive 4-view Tableau dashboard covering department, job role, tenure, and overtime breakdowns, all benchmarked against the company-wide attrition rate.

[Live Dashboard →](https://public.tableau.com/app/profile/kesheka.edupuganti8192/viz/HRAttritionAnalysisKPIDashboard/HRAttritionOverview)

---

## Data Source

All data is sourced from IBM's public **HR Analytics Employee Attrition & Performance** dataset, a fictional but realistic dataset created by IBM data scientists for HR analytics practice.

Dataset: [IBM HR Analytics Attrition Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)

Download the CSV file and place it in the `data/` folder before running:

| Filename to use | File to download from Kaggle |
|-----------------|-------------------------------|
| `hr_attrition_raw.csv` | WA_Fn-UseC_-HR-Employee-Attrition.csv |

---

## Tools

Python, Pandas, Matplotlib, Seaborn, SQLite, Tableau

---

## How to Run

```bash
git clone https://github.com/KeshekaE/hr-attrition-analysis
cd hr-attrition-analysis
pip install pandas matplotlib seaborn
# Download the CSV from Kaggle and place in data/ as hr_attrition_raw.csv
jupyter notebook notebook/hr_attrition_analysis.ipynb
```

---

*This project is part of my data analytics portfolio.*

## Portfolio

[Portfolio Link →](https://keportfolio.vercel.app)

## Author
**Kesheka Edupuganti**  
Data Analyst & BI Specialist | Loma Linda, CA  
ekesheka1010@gmail.com  
[LinkedIn](https://www.linkedin.com/in/kesheka-edupuganti-b53a96293/)
