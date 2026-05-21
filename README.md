# Multi-Source HRMS Workforce Analytics Dashboard

## Problem

HR data is scattered across multiple HRMS systems, making it difficult to track headcount, attrition, hiring trends, and workforce cost efficiency from one reliable view.

## Solution

Built a unified analytics pipeline using Power Query, SQL, and Power BI. The project cleans and merges two HRMS datasets, creates a standardized master workforce table, analyzes workforce trends with SQL, and presents business insights in a Power BI dashboard.

## Tools

- Power Query
- SQL
- Power BI
- Excel / CSV
- GitHub

## Project Structure

```text
hrms-workforce-analytics/
+-- data/
+-- power_query/
+-- sql/
+-- powerbi/
+-- images/
+-- README.md
```

## Features

- Attrition analysis
- Headcount tracking
- Hiring vs exit trends
- Budget vs actual workforce cost
- Department-level workforce insights

## SQL Skills Demonstrated

- Window functions
- Cohort-style workforce analysis
- Time-series snapshots
- Ranking and moving averages
- Variance analysis

## Dashboard Pages

### Page 1: Workforce Overview

- Total headcount
- Active vs terminated employees
- Hiring trend
- Department headcount breakdown

### Page 2: Attrition Analysis

- Attrition rate
- Voluntary vs involuntary exits
- Attrition by department

### Page 3: Budget vs Actual

- Workforce cost variance by department
- Overspending vs underspending status
- Actual monthly cost compared with planned budget

### Page 4: Forecast Insights

- Headcount trend
- Hiring gap estimation
- Workforce planning indicators

## Dashboard Images

Add screenshots after building the Power BI report:

## Dashboard Images

![Workforce Overview](images/dashboard.png)
![Attrition Analysis](images/attrition.png)
![Budget vs Actual](images/budget.png)
![Forecast Insights](images/forecast.png)

## Key Insights

| Insight | Business Impact | Recommendation | Suggested Action |
| --- | --- | --- | --- |
| Headcount increased in 2025, but several new hires were junior-level employees. | Short-term productivity may drop while new employees are still onboarding and building role proficiency. | Balance workforce growth with capability planning, not just headcount targets. | Track new-hire ramp-up time, assign mentors, and review productivity metrics by tenure group. |
| Sales shows elevated attrition because both voluntary and involuntary exits occurred in the department. | High attrition can increase hiring cost, disrupt customer relationships, and reduce sales pipeline continuity. | Prioritize Sales for deeper attrition diagnosis and retention planning. | Review exit reasons, manager feedback, compensation competitiveness, and workload indicators for the Sales team. |
| Information Technology has the highest salary concentration, driven by senior technical roles. | Workforce cost risk is higher in IT because a small number of senior roles can significantly affect total cost. | Monitor critical-role cost and succession risk separately from general headcount. | Build an IT role-cost dashboard showing salary rank, critical roles, replacement risk, and budget variance. |
| Budget overspend is concentrated in teams where actual monthly workforce cost is above planned budget. | Persistent overspending can reduce budget flexibility and affect future hiring approvals. | Separate planned hiring overspend from unplanned compensation or staffing cost increases. | Review departments with positive variance, validate budget assumptions, and flag teams exceeding tolerance thresholds. |
| Hiring activity increased in 2025, but exits in the same year show the need for stronger retention planning. | The organization may be replacing employees instead of achieving sustainable growth. | Track net headcount growth alongside hires and exits. | Add monthly net movement, attrition rate, and replacement hiring indicators to the dashboard. |

## Future Improvements

- Build a predictive attrition model.
- Automate the data refresh pipeline.
- Add employee engagement and performance data.
- Create department-level hiring forecasts.
- Add Power BI row-level security for HR business partners.

## LinkedIn Post Draft

I built an end-to-end HR analytics system using Power Query, SQL, and Power BI.

In this project, I cleaned multi-source HRMS data, merged two HR systems into one master workforce dataset, built a SQL analysis layer, and created dashboard pages for workforce decision-making.

Key features:
- Attrition analysis
- Headcount tracking
- Hiring vs exit trends
- Budget vs actual workforce cost
- Forecast insights

One key insight: headcount increase does not always mean productivity increase. If growth is driven mainly by junior hires, productivity may temporarily drop while new employees ramp up.

GitHub project: [Add your GitHub link here]

Open to feedback from HR analytics, data analytics, and Power BI professionals.
