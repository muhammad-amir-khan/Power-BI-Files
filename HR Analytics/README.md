# HR Analysis Dashboard

> A comprehensive Power BI dashboard for exploring employee attrition, workforce demographics, salary distribution, and engagement risk across an organisation of 1,480 employees.

![HR Analysis Dashboard](HR%20Analytics.jpeg)

---

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Key Metrics](#key-metrics)
- [Dashboard Sections](#dashboard-sections)
- [Filters & Slicers](#filters--slicers)
- [Key Insights](#key-insights)
- [Files](#files)
- [Tools Used](#tools-used)

---

## Overview

This dashboard was built to help HR teams and business leaders understand workforce dynamics at a glance. It covers four core areas:

1. **Attrition** — who is leaving, from which department, and what risk factors drive it
2. **Workspace Composition** — salary bands, gender & marital status distribution, and income by job level
3. **Engagement & Risk** — satisfaction scores across multiple dimensions and a segment-level attrition risk table
4. **Tenure & Development** — years at company, training frequency, time since last promotion, and salary hike trends

Data shown spans **January 2025 to December 2025**.

---

## Dataset

**File:** `HR_Analytics.csv`  
**Rows:** 1,480 employees  
**Columns:** 39 features

| Column | Description |
|---|---|
| `EmpID` | Unique employee identifier |
| `Age` / `AgeGroup` | Employee age and banded age group |
| `Attrition` | Whether the employee left (Yes / No) |
| `Department` | HR, R&D, or Sales |
| `JobRole` | One of 9 roles (e.g., Sales Representative, Research Scientist) |
| `MonthlyIncome` / `SalarySlab` | Actual income and banded salary tier |
| `OverTime` | Whether the employee works overtime |
| `JobSatisfaction` | Score 1–4 |
| `WorkLifeBalance` | Score 1–4 |
| `JobInvolvement` | Score 1–4 |
| `EnvironmentSatisfaction` | Score 1–4 |
| `YearsAtCompany` | Tenure at the organisation |
| `YearsSinceLastPromotion` | Recency of last promotion |
| `TrainingTimesLastYear` | Number of training sessions attended |
| `PercentSalaryHike` | Salary hike % at last appraisal |
| `Gender` | Male / Female |
| `MaritalStatus` | Single / Married / Divorced |
| `BusinessTravel` | Non-Travel / Travel Rarely / Travel Frequently |

---

## Key Metrics

| Metric | Value |
|---|---|
| Total Employees | **1,480** |
| Active Employees | **1,242** |
| Attrited Employees | **238** |
| Overall Attrition Rate | **16.1%** |
| Average Monthly Income | **$6.5K** |
| Average Age | **36.9 years** |
| Average Tenure | **7.0 years** |
| Overtime Prevalence | **28.2%** |
| Average Salary Hike | **15.2%** |

---

## Dashboard Sections

### 1 · Attrition Overview
- Total headcount with department-level breakdown (R&D 65%, Sales 30%, HR 5%)
- Active vs attrited employee counts
- Attrition by department: R&D **133**, Sales **93**, HR **12**

### 2 · Attrition Deep-Dive
- **Attrition % by Job Role** — Sales Representatives lead at **39.3%**, followed by Laboratory Technicians (23.8%) and Human Resources (23.1%)
- **Category % donut chart** — Sales accounts for 38.7% of total attrition, HR 35.6%, R&D 25.7%
- **Overtime → Attrition** — employees with overtime have a **30.6%** attrition rate vs **10.4%** for those without
- **Age Distribution** — clustered bar comparing active vs attrited by age group; 26–35 is the largest cohort (495 active, 116 attrited)

### 3 · Workspace Composition
- **Salary Bands** — majority of employees (753) earn below $5K/month; 133 earn $15K+
- **Gender split** — Female 40%, Male 60%
- **Marital Status** — Married 46%, Single 32%, Divorced 22%
- **Avg Monthly Income by Job Level (1–5)** — ranges from $2.8K at Level 1 to $19.2K at Level 5

### 4 · Engagement & Risk
- **Satisfaction scores** (scale 1–4): Work-Life Balance 2.76 · Job Involvement 2.73 · Job Satisfaction 2.73 · Environment 2.72 · Relationships 2.71
- **Segment-level attrition risk table** — highest-risk segments are Sales Rep role (39.3%), Overtime workers (30.6%), and Single employees (25.4%)

### 5 · Tenure & Development
- Avg years at company: **7.0** | Total experience: **11.3 years**
- Years since last promotion: **2.2** | Trainings per year: **2.8**
- Years in current role: **4.1** | Avg salary hike since promotion: **15.2%**

---

## Filters & Slicers

The dashboard includes two sets of interactive filters in the top bar:

| Filter Group | Options |
|---|---|
| Department | Select All · HR · R&D · Sales |
| Gender | Select All · Female · Male |

All visuals respond dynamically to slicer selections, enabling focused analysis by department or gender.

---

## Key Insights

- **Overtime is the single strongest attrition driver** — employees on overtime are 3× more likely to leave (30.6% vs 10.4%).
- **Sales Representatives are the highest-risk role** with a 39.3% attrition rate — nearly 1 in 2 employees in this role leaves.
- **Low earners churn most** — the sub-$5K salary band has a 21.6% attrition rate; addressing compensation at entry level could reduce overall attrition meaningfully.
- **The 26–35 age group** represents both the largest active cohort and the largest attrited cohort — engagement strategies targeting early-career employees are critical.
- **Satisfaction scores are uniformly low** (all between 2.71–2.76 on a 4-point scale), suggesting systemic engagement issues rather than role-specific ones.
- **Promotion cadence is slow** — employees wait an average of 2.2 years between promotions despite receiving adequate training (2.8 sessions/year), which may be contributing to dissatisfaction.

---

## Files

| File | Description |
|---|---|
| `HR Dashboard.pbix` | Power BI Desktop file — open to explore or modify the dashboard |
| `HR_Analytics.csv` | Raw dataset (1,480 rows × 39 columns) used as the data source |
| `HR Analytics.jpeg` | Dashboard screenshot |
| `README.md` | This file |

---

## Tools Used

- **Power BI Desktop** — data modelling, DAX measures, and report visualisation
- **Microsoft Excel / CSV** — data source
- **DAX** — custom measures for attrition rate, satisfaction averages, salary band distributions, and segment-level risk scoring
