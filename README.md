# Multi-Source HRMS Workforce Analytics Dashboard | Power BI + Power Query + SQL

## Project Overview

This Multi-Source HRMS Workforce Analytics Dashboard was created using Power BI, Power Query, and SQL to analyze workforce headcount, attrition, hiring trends, and budget performance across multiple HRMS data sources.

The project combines two sample HRMS files into one cleaned master dataset. Power Query was used to clean and standardize the data, SQL was used to build the analysis layer, and Power BI was used to create a four-page HR analytics dashboard.

The goal of this project is to demonstrate how HR data from different systems can be cleaned, merged, and transformed into actionable workforce insights for HR leaders and business stakeholders.

## Dashboard Pages

## Page 1: Workforce Overview

![Workforce Overview](https://raw.githubusercontent.com/joyceleehy/hrms-workforce-analytics/main/images/dashboard.png)

This page provides a high-level snapshot of workforce size, employee status, department headcount, and hiring movement.

Key visuals:

- Total employees
- Active employees
- Terminated employees
- Attrition rate
- Active vs terminated employees
- Headcount by department
- Hiring trend over time

## Page 2: Attrition Analysis

![Attrition Analysis](https://raw.githubusercontent.com/joyceleehy/hrms-workforce-analytics/main/images/Attrition.png)

This page focuses on employee exits and attrition risk.

Key visuals:

- Terminated employees
- Attrition rate
- Attrition by department
- Voluntary vs involuntary exits
- Exit trend over time
- Attrition insight summary

## Page 3: Budget vs Actual

![Budget vs Actual](https://raw.githubusercontent.com/joyceleehy/hrms-workforce-analytics/main/images/Budget.png)

This page compares actual workforce cost against planned budget.

Key visuals:

- Total monthly cost
- Total budget cost
- Budget variance
- Budget variance percentage
- Budget variance by department
- Actual vs budget cost by department
- Overspending vs underspending status

## Page 4: Forecast Insights

![Forecast Insights](https://raw.githubusercontent.com/joyceleehy/hrms-workforce-analytics/main/images/forecast.png)

This page supports workforce planning by showing hiring movement and future workforce signals.

Key visuals:

- Current headcount
- 2025 hires
- 2025 exits
- Hiring trend by year
- 2025 hiring by department
- Forecast insight summary

## Key Highlights

- Total employees: 16
- Active employees: 12
- Terminated employees: 4
- Attrition rate: 25.0%
- Workforce cost and budget variance tracking
- Department-level headcount analysis
- Voluntary vs involuntary exit analysis
- Hiring trend and workforce planning view
- Budget overspending and underspending analysis


## Dashboard Insights

- Headcount increased in 2025, but several new hires were junior-level employees, which may reduce short-term productivity while employees are still onboarding.
- Sales shows elevated attrition because both voluntary and involuntary exits occurred in the department.
- Information Technology has the highest salary concentration, driven by senior technical roles.
- Budget overspend is concentrated in teams where actual monthly workforce cost is above planned budget.
- Hiring activity increased in 2025, but exits also occurred in the same year, showing the need to track net workforce movement instead of hiring volume only.

## Business Impact

This dashboard helps HR leaders, People Analytics teams, and business stakeholders:

- Monitor workforce headcount in one centralized view
- Identify departments with higher attrition risk
- Track hiring and exit movement over time
- Compare actual workforce cost against planned budget
- Understand which departments are overspending or underspending
- Support workforce planning and leadership reporting
- Move from manual HR reporting to structured workforce analytics

## Recommendations

- Monitor attrition monthly by department and exit type.
- Review departments with repeated hiring and exit activity.
- Compare headcount growth with productivity, tenure, and job level mix.
- Track budget variance by department to identify cost pressure early.
- Review teams with high attrition and high hiring activity to understand whether growth is sustainable.
- Add forecasting logic to support future workforce planning.

## Suggested Actions

- Create a monthly HR workforce review using the dashboard.
- Use attrition by department to prioritize retention discussions.
- Review voluntary exits with manager feedback, workload, and compensation data.
- Track new-hire ramp-up time, especially for junior employees.
- Monitor departments with positive budget variance and validate budget assumptions.
- Add monthly net headcount movement to separate real growth from replacement hiring.

## Tools Used

- Power BI Desktop
- Power Query
- DAX
- SQL
- Excel / CSV
- Data Cleaning
- Data Visualization
- HR Analytics
- Workforce Analytics
- Business Intelligence

## Data Sources

This project uses two sample HRMS source files:

- `hrms_a.csv`
- `hrms_b.csv`

Both files contain employee information such as employee ID, employee name, department, job level, hire date, termination date, termination type, salary, monthly cost, budget cost, and source system.

The final cleaned dataset is:

- `cleaned_master_data.csv`

## Power Query Data Cleaning

Power Query was used to clean and prepare the HRMS data before analysis.

Main cleaning steps included:

- Loaded `hrms_a.csv` and `hrms_b.csv` into Power Query.
- Standardized column names so both HRMS files followed the same structure.
- Cleaned employee ID format into one standard format, such as `EMP0001`.
- Converted hire date and termination date into proper date format.
- Standardized department names, for example:
  - `HR` to `Human Resources`
  - `IT` to `Information Technology`
  - `Ops` to `Operations`
- Removed currency symbols from salary and cost columns.
- Converted salary, monthly cost, and budget cost into numeric format.
- Removed duplicate employee records.
- Appended both HRMS files into one master workforce table.
- Created a new `employee_status` column:
  - `Active` if termination date is blank
  - `Terminated` if termination date is available

## SQL Analysis Layer

SQL was used to create the analysis layer for workforce reporting.

SQL analysis included:

- Attrition rate calculation
- Total employees and terminated employees
- Attrition by department
- Voluntary vs involuntary exits
- Monthly headcount snapshot
- Hiring vs exit trend
- Budget vs actual workforce cost
- Budget variance calculation
- Salary ranking within department
- Running headcount trend
- 3-month moving attrition average

## SQL Skills Demonstrated

- Window functions
- Time-series snapshots
- Cohort-style workforce analysis
- Salary ranking by department
- Running totals
- Moving averages
- Budget variance analysis
- Department-level workforce analysis

## Note

This project uses sample HRMS data created for portfolio purposes. The dataset does not contain real employee information.

## About This Project

This project was created as part of my data analytics portfolio to demonstrate skills in Power BI dashboard design, Power Query data cleaning, SQL analysis, HR analytics, workforce reporting, budget variance analysis, and business intelligence storytelling.
