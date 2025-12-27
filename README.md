# Adecco-Analytics

<div align="center">

<img src="https://logos-world.net/wp-content/uploads/2023/08/Adecco-Logo.png" alt="drawing" width="300"/>

</div>

<!--![Adecco](https://logos-world.net/wp-content/uploads/2023/08/Adecco-Logo.png)
![Adecco](https://raw.githubusercontent.com/PratyushPuri/Adecco-Analytics/refs/heads/main/Adecco%20Dash.png)-->

<br>

## Overview

Employee turnover at Adecco India is rising, particularly among junior sales employees. This attrition raises the cost of hiring and training new employees and affects productivity.

In order to determine the main causes of employee departures, this project examines HR data. Finding trends in departmental difficulties, demographics, and job satisfaction is the main goal. The objective is to offer practical insights to boost engagement, lower turnover, and improve retention tactics.


The result will be data-driven suggestions to assist management in cultivating a more stable and contented workforce, which will directly support the expansion and ongoing operations of the business.

## Dataset

This analysis uses a synthetic HR analytics dataset from [Kaggle: HR Analytics Case Study](https://www.kaggle.com/datasets/bhanupratapbiswas/hr-analytics-case-study). It is designed to mimic real-world employee attrition scenarios in a mid-sized organization. The dataset contains **1,470 employee records** across **35 columns**, which include demographic, job-related, and satisfaction-related variables.

- **Source**: Publicly available Kaggle dataset that simulates employee data for attrition modeling.
- **Time Coverage**: Cross-sectional (snapshot of employee status at a single time).
- **Key Variables**:
  - **Target**: `Attrition` (binary: "Yes" or "No") which indicates whether an employee left the company.
  - **Demographics**: `Age`, `Gender`, `MaritalStatus`, `DistanceFromHome`.
  - **Job Details**: `Department`, `JobRole`, `JobLevel`, `YearsAtCompany`, `BusinessTravel`.
  - **Compensation**: `MonthlyIncome`, `HourlyRate`, `DailyRate`, `PercentSalaryHike`.
  - **Satisfaction Metrics**: `JobSatisfaction`, `EnvironmentSatisfaction`, `WorkLifeBalance`, `RelationshipSatisfaction` (all on a scale from 1 to 4).
  - **Work History**: `TotalWorkingYears`, `NumCompaniesWorked`, `YearsSinceLastPromotion`.
- **Notes**: 
  - `EmployeeCount` and `StandardHours` are constants (1 and 80, respectively) and were excluded from the analysis.
  - `Over18` is consistently "Y" and therefore redundant.
  - All data is anonymized and synthetic, meant for educational and analytical practice.

## Analysis

> File for Analytics is `Adecco.xlsx`

### **Data Analysis Process in Excel**

I analyzed Adecco India's HR data using Microsoft Excel to find insights into employee attrition. The process went step-by-step from data preparation to visualization.

#### **Data Cleaning & Preparation**
* **Initial Assessment:** I loaded the raw HR dataset into Excel to understand its structure, column names, and data types.
* **Standardization & Deduplication:** I removed duplicates and ensured consistency in categorical data, such as department names and attrition status.
* **Handling Missing Values:** I identified and addressed missing or inconsistent entries using filters and logical checks to ensure data integrity for calculations.

#### **Exploratory Data Analysis (EDA) Using Core Excel Functions**
* **Insights:** I used essential functions to answer key questions:
    * **Overall Attrition Rate:** I used `COUNTIF` and `COUNTA` to find the overall turnover rate.
    * **Departmental Trends:** I created **PivotTables** to calculate and compare attrition rates across Engineering, Sales, Marketing, and more, identifying Sales as a critical area.
    * **Demographic Analysis:** I applied **AVERAGE**, **FILTER**, and **PivotTables** to analyze the profiles of departing employees, including average age, income, and gender split.
    * **Key Metrics:** I calculated average employee tenure, overtime prevalence, and satisfaction scores by role using **PivotTables** and `AVERAGEIF`.
    * **Factor Correlation:** I used the `CORREL` function to find top attrition drivers like job satisfaction, monthly income, and distance from home.
    * **Trend Analysis:** I created **scatter plots** with **Trendlines** to show relationships between variables like Age vs. Job Satisfaction and Work-Life Balance vs. Performance.
    * **Segmented Analysis:** I used **PivotTables** to break down attrition by factors like marital status, training frequency, and stock option levels to uncover hidden patterns.

#### **Dashboard Development**
* **Visual Synthesis:** I compiled key findings into a single, interactive **Excel Dashboard**.
* **Key Components:** The dashboard includes:
    * A high-level **summary metrics card** showing the overall attrition rate.
    * **Interactive charts** (bar, pie, line) that visualize department-wise attrition, demographic breakdowns, and satisfaction trends.
    * **Dynamic slicers** for filtering data by Department, Job Role, and Age Group to enable user exploration.
    * Clear **insight callouts** highlighting the main drivers of attrition and actionable recommendations for management.
* **Purpose:** This dashboard acts as a centralized tool for stakeholders to monitor attrition trends, understand root causes, and track the impact of future changes.

## **Dashboard Summary: Key Insights & Findings**

The **Adecco Employee Attrition Analysis Dashboard** brings together the analysis into a single, useful visual tool. Built entirely in Excel, it helps management quickly understand the size and main causes of employee turnover.

The dashboard shows an **overall attrition rate of 16.12%**, which means **237 employees** have left. A main visual, like a bar chart for **Attrition by Department**, quickly points out high-risk areas, confirming concerns about the **Sales department**. Interactive filters let users break down the data further, uncovering trends by **Job Role, Age Group, and Tenure**.

Additional charts offer important context:
*   **Attrition by Demographics** (e.g., gender, age group) shows if turnover affects certain groups more.
*   **Trends in Job Satisfaction & Income** for employees who left compared to those who stayed.
*   **Correlation visuals** connect factors such as **Distance from Home** and **Years Since Last Promotion** to the chances of leaving.

This dashboard turns raw data into clear, strategic information. It not only measures the problem but also shows where and why it happens, providing a solid basis for targeted HR actions and policy reviews to improve retention.



![Adecco](https://raw.githubusercontent.com/PratyushPuri/Adecco-Analytics/refs/heads/main/Adecco%20Dash.png)

<br>

## **How to Use the Dashboard**

This interactive Excel dashboard is designed for easy exploration. Follow these steps to gain insights:

1.  **Open the File:** Launch the `Adecco.xlsx` file in Microsoft Excel.

2.  **Navigate & Interact:**
    *   **Key Metrics:** View the summary at the top, which includes the Overall Attrition Rate and Count.
    *   **Explore with Slicers:** Use the interactive slicers, usually found on the side or top, to filter the entire dashboard. You can filter by **Department, Job Role, Age Group, or Marital Status** to see how attrition trends change for specific segments.
    *   **Analyze Charts:** Hover over any chart element, like bars or pie slices, to see detailed tooltips with exact numbers and percentages.

3.  **Refresh Data (If Applicable):**
    *   If the dashboard is connected to a live data source, update it by going to the **Data** tab in the Excel ribbon and clicking **"Refresh All."**
    *   **Security Note:** If asked about enabling macros or external links, select "Enable Content" only if you trust the source of this file.


## Author & Contact
- Name: `Pratyush Puri`
- Contact: pratyushpuri17@gmail / [LinkedIn](https://www.linkedin.com/in/pratyushpuri)


 
