# Multi-Source HRMS Workforce Analytics Dashboard | Power BI + Power Query + SQL

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-SQLite-003B57?style=flat&logo=sqlite&logoColor=white)
![Power Query](https://img.shields.io/badge/Power%20Query-217346?style=flat&logo=microsoft&logoColor=white)
![DAX](https://img.shields.io/badge/DAX-F2C811?style=flat&logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat)

Most HR teams manage workforce data across multiple systems — and no single source tells the full story. This project simulates that real-world challenge: two separate HRMS files, cleaned and merged into one master dataset, then analysed across headcount, attrition, budget, and workforce planning.

---

## Dashboard Preview

**Page 1 — Workforce Overview**
![Workforce Overview](https://raw.githubusercontent.com/joyceleehy/hrms-workforce-analytics/main/images/dashboard.png)

**Page 2 — Attrition Analysis**
![Attrition Analysis](https://raw.githubusercontent.com/joyceleehy/hrms-workforce-analytics/main/images/Attrition.png)

**Page 3 — Budget vs Actual**
![Budget vs Actual](https://raw.githubusercontent.com/joyceleehy/hrms-workforce-analytics/main/images/Budget.png)

**Page 4 — Forecast Insights**
![Forecast Insights](https://raw.githubusercontent.com/joyceleehy/hrms-workforce-analytics/main/images/forecast.png)

---

## How It Was Built

    hrms_a.csv + hrms_b.csv (two separate HRMS sources)
            ↓
    Power Query — standardise columns, clean dates, fix dept names,
                  remove duplicates, append into master table
            ↓
    SQL — attrition rate, budget variance, salary ranking,
          window functions, moving averages, running totals
            ↓
    DAX — KPI measures, status flags, variance calculations
            ↓
    Power BI — 4-page dashboard across workforce, attrition,
               budget, and forecast views
            ↓
    cleaned_master_data.csv — final output dataset

---

## Dashboard Pages

| Page | Focus |
|---|---|
| Workforce Overview | Headcount, active vs terminated, hiring trend, dept breakdown |
| Attrition Analysis | Exit rate, voluntary vs involuntary, dept-level attrition |
| Budget vs Actual | Workforce cost vs planned budget, variance by department |
| Forecast Insights | 2025 hiring movement, exits, hiring trend by year |

---

## Power Query — Data Cleaning Steps

- Loaded and standardised columns across both HRMS source files
- Cleaned employee ID format → `EMP0001` standard
- Converted hire and termination dates to proper date format
- Standardised department names (`HR` → `Human Resources`, `IT` → `Information Technology`, `Ops` → `Operations`)
- Removed currency symbols, converted salary and cost columns to numeric
- Removed duplicate records
- Appended both files into one master workforce table
- Created `employee_status` column: `Active` (no termination date) / `Terminated`

---

## SQL Analysis Layer

| Technique | Applied To |
|---|---|
| Window functions | Salary ranking within department, running headcount |
| Time-series snapshots | Monthly headcount movement |
| Moving averages | 3-month rolling attrition |
| Running totals | Cumulative hire and exit trends |
| Budget variance | Actual vs planned cost by department |
| Cohort-style analysis | Hiring vs exit by year and department |

---

## Tools Used

`Power BI Desktop` `Power Query` `DAX` `SQL` `Excel / CSV`

---

## Data Sources

Two sample HRMS files created for portfolio purposes — no real employee data used.

    hrms_a.csv               HRMS source file A
    hrms_b.csv               HRMS source file B
    cleaned_master_data.csv  Final merged and cleaned dataset

---

📄 [Full Analysis & Insights](insights.md)

> 📎 [LinkedIn](https://www.linkedin.com/in/joyceleehowyee/) · [More Projects](https://github.com/joyceleehy)
