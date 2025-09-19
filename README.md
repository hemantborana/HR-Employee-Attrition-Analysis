# HR Employee Attrition Analytics
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Excel](https://img.shields.io/badge/Excel-217346?style=flat&logo=microsoft-excel&logoColor=white)](https://www.microsoft.com/en-us/microsoft-365/excel)
[![Data Analysis](https://img.shields.io/badge/Data%20Analysis-4285F4?style=flat&logo=google-analytics&logoColor=white)](https://analytics.google.com/)

A comprehensive data analytics project focused on understanding employee attrition patterns and predicting workforce turnover using advanced Excel techniques including pivot tables, regression analysis, and interactive dashboards.

![Dashboard Preview](screenshots/Dashboard_overview.png)

## 🎯 Project Overview

This project analyzes employee attrition data to identify key factors contributing to workforce turnover and provides actionable insights for HR decision-making. The analysis employs multiple statistical and visualization techniques to create a comprehensive view of employee retention patterns.

### 🔍 Key Objectives
- **Identify Attrition Drivers**: Analyze factors leading to employee turnover
- **Predict Turnover Risk**: Develop models to forecast attrition likelihood  
- **Create Actionable Insights**: Provide data-driven recommendations for HR strategy
- **Build Interactive Dashboard**: Design user-friendly visualization tools

## 📊 Dataset Information

**Source**: HR Employee Attrition Dataset  
**Records**: 1,470 employee records  
**Features**: 36 variables including demographics, job characteristics, and satisfaction metrics

### Key Variables Analyzed:
- **Demographics**: Age, Gender, Marital Status
- **Education**: Education, EducationField
- **Job Characteristics**: Department, JobRole
- **Satisfaction Metrics**: JobSatisfaction, EnvironmentSatisfaction, RelationshipSatisfaction
- **Compensation**: MonthlyIncome, HourlyRate
- **Career Progression**: YearsAtCompany, YearsInCurrentRole, YearsSinceLastPromotion
- **Performance**: PerformanceRating, JobInvolvement, WorkLifeBalance

## 🛠️ Methodology & Tools

### Technology Stack
- **Primary Tool**: Microsoft Excel (Pivot Tables, Charts, What-If Analysis, Regression Tools)
- **Dataset**: HR Employee Attrition Data (1,470 records, 36 variables)

### Analysis Framework
1. **Data Transformation**: VLOOKUP formulas to convert numeric values into descriptive labels
2. **Pivot Table Reports**: Six comprehensive analytical reports with charts
3. **Interactive Dashboard**: Consolidated dashboard with dynamic slicers
4. **What-If Analysis**: Scenario modeling using Data Tables
5. **Regression Analysis**: Statistical modeling using Excel's Data Analysis ToolPak

## 📈 Key Findings & Results

### Report 1: Monthly Income and Job Satisfaction by Job Role and Education Field
- **Chart Type**: Clustered Column Chart
- **Key Finding**: Managers and Research Directors generally earn the highest. Job satisfaction is higher for employees with advanced education (Master's and Doctoral levels) in roles like Healthcare Representative and Research Scientist.

### Report 2: Gender and Job Role-wise Job & Environment Satisfaction
- **Chart Type**: Stacked Column
- **Key Finding**: Females in R&D have slightly higher satisfaction than males. Sales roles show slightly lower environment satisfaction across both genders.

### Report 3: Hourly Rate, Monthly Income, and Job Satisfaction by Education Field and Job Role
- **Chart Type**: Line Chart
- **Key Finding**: Medical and Technical roles have comparatively higher hourly rates. Satisfaction is correlated with higher earnings.

### Report 4: Job Satisfaction by Department and Gender
- **Chart Type**: Clustered Bar
- **Key Finding**: In Human Resources, females show higher satisfaction. Research & Development shows near equal satisfaction levels across genders.

### Report 5: Distance from Home by Gender, Department, and Job Role
- **Key Finding**: Employees in Sales and Human Resources tend to live further from work than those in R&D. There's a slight gender difference, with males averaging slightly longer commute distances.

### Report 6: Monthly Income by Education and Attrition
- **Chart Type**: Side-by-Side Column Chart
- **Key Finding**: Employees with lower education levels and lower income show higher attrition rates, suggesting compensation may influence turnover.

## 🎛️ Interactive Dashboard

**Worksheet**: Q9_Dashboard

A consolidated, interactive dashboard using Slicers for filtering by:
- Job Role
- Department
- Gender
- Education Field
- Attrition

Contains linked charts and pivot tables that update dynamically based on slicer selection.

## 🔮 What-If Analysis

**Worksheet**: Q10_WhatIfAnalysis

Scenario modeling performed using Data Tables to test impact on attrition by adjusting:
- Monthly Income
- Distance From Home
- Percent Salary Hike
- Job Satisfaction

**Key Insights**:
- Attrition probability decreases significantly when job satisfaction is high and commute is low
- Salary increases have diminishing returns beyond a certain level

## 📊 Regression Analysis

**Worksheet**: Q11_Regression

**Method**: Excel's Data Analysis ToolPak (Regression)

**Target Variable**: Attrition (encoded as 1 = Yes, 0 = No)

**Predictor Variables**:
- YearsAtCompany
- YearsInCurrentRole
- YearsSinceLastPromotion
- YearsWithCurrManager
- JobSatisfaction

### Regression Results:
- **Adjusted R²**: ~0.20 (typical for HR datasets)
- **Significant Predictors**:
  - JobSatisfaction (negative coefficient – higher satisfaction lowers attrition)
  - YearsSinceLastPromotion (positive coefficient – longer without promotion increases attrition)

**Interpretation**: Attrition is moderately predicted by lack of promotion, low satisfaction, and fewer years with the current manager.

## 📁 Project Structure

```
HR-Attrition-Analytics/
│
├── Q1_RefTables/           # Reference mappings for data transformation
├── Q2_FormattedData/       # Cleaned dataset with descriptive labels
├── Q3_Report1/             # Monthly Income & Job Satisfaction Analysis
├── Q4_Report2/             # Gender & Job Role Satisfaction Analysis
├── Q5_Report3/             # Hourly Rate, Income & Satisfaction Analysis
├── Q6_Report4/             # Job Satisfaction by Department & Gender
├── Q7_Report5/             # Distance from Home Analysis
├── Q8_Report6/             # Monthly Income by Education & Attrition
├── Q9_Dashboard/           # Interactive Dashboard with Slicers
├── Q10_WhatIfAnalysis/     # Scenario Modeling & Data Tables
└── Q11_Regression/         # Statistical Regression Analysis
```

## 🎯 Conclusion

This project provides a multi-faceted analysis of employee satisfaction and attrition using real HR data. Key takeaways include:

- **Satisfaction and compensation are key predictors of attrition**
- **Distance from home has a modest but real impact**
- **Regression analysis confirms that promotion cycles and management support influence retention**
- **An interactive dashboard enables dynamic exploration of attrition patterns**

The analysis demonstrates how advanced Excel techniques can deliver comprehensive HR analytics, providing actionable insights for workforce management and retention strategies.
