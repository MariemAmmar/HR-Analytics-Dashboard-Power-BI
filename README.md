# 👥 HR Analytics Dashboard — Power BI

An interactive Power BI dashboard analyzing 1,480 employee records across demographics, performance, compensation, and attrition to help HR teams identify workforce trends, reduce turnover, and make data-driven people decisions.

---

## 📌 Project Overview

This project builds a comprehensive **HR Analytics Dashboard** in Power BI using real employee data. The dashboard enables HR managers and business leaders to monitor workforce composition, track attrition patterns across departments and demographics, and identify the key factors driving employee turnover — from overtime and salary levels to age groups and job roles. The goal is to transform raw HR data into actionable insights that support smarter hiring, retention, and compensation strategies.

---

## 📁 Repository Structure

```
├── HR_Data.xlsx                  # Raw employee dataset (1,480 records)
└── HR_Analytics_Dashboard.pbix  # Power BI dashboard file
```

---

## 🗄️ Dataset

**1,480 employees × 38 columns**

### Demographics
| Field | Description |
|---|---|
| `EmpID` | Unique employee identifier |
| `Age` / `AgeGroup` | Age (18–60) and age band (18-25, 26-35, 36-45, 46-55, 55+) |
| `Gender` | Employee gender |
| `MaritalStatus` | Married, Single, or Divorced |
| `Education` | Education level (encoded) |
| `DistanceFromHome` | Commute distance |

### Employment
| Field | Description |
|---|---|
| `Department` | Department (3 departments) |
| `JobRole` | Job role (9 distinct roles) |
| `JobLevel` | Seniority level (1–5) |
| `BusinessTravel` | Travel frequency (Non-Travel, Travel_Rarely, Travel_Frequently) |
| `OverTime` | Whether employee works overtime (Yes/No) |
| `YearsAtCompany` | Total tenure at company |
| `YearsInCurrentRole` | Years in current position |
| `YearsSinceLastPromotion` | Years since last promotion |
| `YearsWithCurrManager` | Years working under current manager |
| `TotalWorkingYears` | Total career experience |
| `NumCompaniesWorked` | Number of previous employers |
| `TrainingTimesLastYear` | Training sessions attended last year |

### Compensation
| Field | Description |
|---|---|
| `MonthlyIncome` | Monthly salary ($1,009 – $19,999) |
| `SalarySlab` | Salary band (Upto 5k, 5k-10k, 10k-15k, 15k+) |
| `DailyRate` / `HourlyRate` / `MonthlyRate` | Rate metrics |
| `PercentSalaryHike` | Last salary increase % |
| `StockOptionLevel` | Stock option tier |

### Satisfaction & Performance
| Field | Description |
|---|---|
| `JobSatisfaction` | Job satisfaction score (1–4) |
| `EnvironmentSatisfaction` | Work environment satisfaction (1–4) |
| `RelationshipSatisfaction` | Relationship satisfaction (1–4) |
| `WorkLifeBalance` | Work-life balance score (1–4) |
| `JobInvolvement` | Level of job involvement (1–4) |
| `PerformanceRating` | Performance rating (1–4) |

### Attrition
| Field | Description |
|---|---|
| `Attrition` | Whether employee left (Yes = 238, No = 1,242) |
| `Complain` | Filed a complaint in last 2 years |

---

## 📊 Dashboard Features & Step-by-Step Documentation

### KPI Cards
- **Total Employees:** 1,480
- **Attrition Count:** 238 employees
- **Attrition Rate:** 16.1%
- **Active Employees:** 1,242
- **Average Age** across workforce

### Attrition by Department
- Visualized attrition rate across 3 departments
- Department 1002 has the highest attrition at **20.7%**, followed by Department 1003 at **19.0%** and Department 1001 at **13.8%**

### Attrition by Age Group
- Breakdown of attrition across 5 age bands
- Largest employee segment: **26-35 years (611 employees)**
- Youngest group (18-25) and oldest (55+) are smallest cohorts

### Attrition by Salary Slab
- Compared attrition rates across 4 salary bands
- Majority of employees (753) earn **Upto $5K/month**
- Higher salary bands (10k-15k, 15k+) have significantly fewer employees

### Attrition by Gender
- Compared male vs. female attrition rates
- Workforce is predominantly male (889 vs. 591 female employees)

### Attrition by Job Role
- Tracked attrition across **9 distinct job roles**
- Enables identification of high-turnover positions for targeted retention

### Attrition by Years at Company
- Line/bar chart tracking attrition by tenure
- Identifies whether early-career or long-tenured employees leave more

### Overtime Impact on Attrition
- 418 employees (28.2%) work overtime
- Filtered analysis comparing attrition rates for overtime vs. non-overtime employees

### Marital Status Analysis
- Workforce breakdown: Married (679), Single (473), Divorced (328)
- Attrition segmented by marital status to identify at-risk groups

### Education Level Filter
- Interactive slicer enabling drill-down by education level
- 6 education categories encoded in the dataset

---

## 💡 Key Findings

| Metric | Value |
|---|---|
| Overall Attrition Rate | **16.1%** |
| Highest-Attrition Department | **Dept 1002 — 20.7%** |
| Employees on Overtime | **418 (28.2%)** |
| Lowest Salary Band (most employees) | **Upto $5K — 753 employees** |
| Largest Age Group | **26–35 years — 611 employees** |
| Total Active Employees | **1,242** |

- Employees earning **under $5K/month** represent the largest group and are most at risk of attrition
- **Overtime workers** show disproportionately higher attrition — a key retention lever
- The **26-35 age group** dominates the workforce and drives the most attrition volume
- **Department 1002** has the highest attrition rate at 20.7%, signaling a management or culture concern

---

## 🛠️ Tools & Technologies

- **Visualization:** Power BI Desktop
- **Data Source:** Microsoft Excel (.xlsx)
- **Techniques:** DAX measures, KPI cards, slicers and filters, bar/column charts, donut charts, matrix visuals, conditional formatting, drill-through, interactive cross-filtering

---

## 🚀 Getting Started

1. Clone this repository
2. Open `HR_Analytics_Dashboard.pbix` in **Power BI Desktop**
3. If prompted, update the data source path to point to `HR_Data.xlsx` in your local directory
4. Refresh the data and interact with the dashboard using slicers and filters

> Requires **Power BI Desktop** (free download from Microsoft). Compatible with Power BI Desktop June 2023 or later.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
