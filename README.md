# Employee Attrition Analysis – Salifort Motors

## Project Overview

This project focuses on analyzing employee attrition at **Salifort Motors**. The primary goal is to uncover the key factors leading to employee turnover and provide actionable, data-driven recommendations to improve employee satisfaction and retention while reducing recruitment costs.

---

## Business Context

The HR department at Salifort Motors has collected employee data but lacks direction on how to leverage it. They have tasked a data analytics professional (you) to:

- Understand why employees are leaving.
- Identify trends and patterns in the data.
- Recommend strategic changes to boost retention.

Improving retention is crucial, as high attrition increases costs related to hiring and onboarding new employees.

---

## Work Summary

### Problem Statement

Why are employees leaving the company, and what can be done to prevent it?

### Initial Steps

- Data import and inspection
- Data cleaning (renaming columns, removing duplicates, handling outliers)
- Initial exploratory data analysis (EDA)

---

## Data Handling & Cleaning

### Step 1: Data Import

- Dataset loaded using Pandas
- Libraries used: NumPy, Pandas, Matplotlib, Seaborn

### Step 2: Data Cleaning

- Renamed inconsistent or misspelled columns to `snake_case`
- Checked for missing values (none found)
- Removed 3,008 duplicate rows (20% of dataset)
- Detected and assessed outliers in `tenure`

**Columns in cleaned dataset:**

['satisfaction_level', 'last_evaluation', 'number_project',
'average_monthly_hours', 'tenure', 'work_accident', 'left',
'promotion_last_5years', 'department', 'salary']


---

## Exploratory Data Analysis (EDA)

### Key Visualizations

- Boxplot of `average_monthly_hours` vs `number_project`, colored by `left`
- Scatterplot of `average_monthly_hours` versus `satisfaction_level`
- Histogram showing project count distribution across `left` vs `stayed`
- Correlation heatmap

### Important Insights

#### Overwork Indicator
- Employees with 6 or 7 projects worked the most hours and had the highest attrition.
- Every employee who worked on 7 projects left the company.

#### Workload vs Retention
- Optimal number of projects: **3–4** (lowest attrition rates)
- Employees with extreme workloads (too high or too low) were more likely to leave.

#### Hours Worked
- Most employees work **more than 166 hours/month**, indicating overwork across the board.

---

## Business Insights

- Attrition is highest among overworked employees (especially those with 6–7 projects).
- Employees might quit due to burnout or feeling undervalued.
- Low satisfaction and high workload are strong indicators of future attrition.

---

## Next Steps

- Correlation analysis to further understand drivers of attrition
- Build predictive model using logistic regression
- Provide HR department with actionable strategies:
  - Balanced project assignment (3–4 projects per employee)
  - Monitor work hours
  - Improve satisfaction for employees at risk

---

## Dataset Info

- **Filename:** `HR_capstone_dataset.csv`
- **Total records:** 14,999
- **Post-cleaning records:** 11,991

---

## Technologies Used

- Python 
- Pandas, NumPy for data manipulation
- Matplotlib, Seaborn for data visualization

---

## Reference

This project was developed based on knowledge and techniques learned from the  
[Google Advanced Data Analytics Professional Certificate](https://www.coursera.org/professional-certificates/google-advanced-data-analytics) on Coursera.


---

## Contact

For any queries or collaboration, feel free to connect!



