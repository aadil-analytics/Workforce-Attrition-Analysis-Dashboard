# Workforce Attrition Analysis Dashboard

## 📌 Project Overview

This project analyzes employee attrition using **Power BI** to identify
patterns and factors associated with employees leaving an organization.

The analysis is based on **4,653 employee records** and focuses on
attrition across employee demographics, joining year, city, education,
payment tier, bench status, and experience in the current domain.

The goal of the project is to turn raw HR data into an interactive
dashboard that can help HR teams identify areas with higher attrition
and investigate potential retention issues.

------------------------------------------------------------------------

## 🖼️ Dashboard Preview

![Workforce Attrition
Dashboard](dashboard/Workforce%20Attrition%20Dashboard.png)

------------------------------------------------------------------------

## 🎯 Business Objectives

The dashboard is designed to answer questions such as:

-   What is the overall employee attrition rate?
-   How many employees have left the organization?
-   Does attrition differ by gender?
-   Which city has the highest attrition rate?
-   Which education group has the highest attrition rate?
-   How does attrition vary by joining year?
-   How does experience in the current domain relate to attrition?
-   Does payment tier show differences in attrition?
-   Does having been benched relate to a higher attrition rate?

------------------------------------------------------------------------

## 🛠️ Tools & Technologies

  Tool              Purpose
  ----------------- ----------------------------------------------
  **Power BI**      Interactive dashboard and data visualization
  **DAX**           KPI and attrition-rate calculations
  **Power Query**   Data preparation and transformation
  **CSV**           Source dataset

------------------------------------------------------------------------

## 📂 Project Files

``` text
Workforce-Attrition-Analysis/
│
├── data/
│   └── Employee.csv
│
├── powerbi/
│   └── workforce.pbix
│
├── dashboard/
│   └── Workforce Attrition Dashboard.png
│
└── README.md
```

------------------------------------------------------------------------

## 📊 Dataset Overview

The dataset contains **4,653 records** and **9 attributes**:

-   `Education`
-   `JoiningYear`
-   `City`
-   `PaymentTier`
-   `Age`
-   `Gender`
-   `EverBenched`
-   `ExperienceInCurrentDomain`
-   `LeaveOrNot`

### Data Quality

-   Rows: **4,653**
-   Columns: **9**
-   Missing values: **0**
-   Exact duplicate rows: **1,889**

> **Note:** The dataset does not contain a unique employee ID.
> Therefore, exact duplicate rows cannot automatically be treated as
> erroneous duplicate employees. They may represent different employees
> with identical attribute combinations. For this analysis, the records
> are retained unless a unique employee identifier is available to
> validate duplication.

------------------------------------------------------------------------

# 📈 Key KPIs

  KPI                             Value
  -------------------- ----------------
  Total Employees             **4,653**
  Employees Left              **1,600**
  Employees Stayed            **3,053**
  Attrition Rate             **34.39%**
  Average Age            **29.4 years**
  Average Experience     **2.91 years**

------------------------------------------------------------------------

# 📊 Dashboard Overview

The Power BI dashboard contains:

### KPI Cards

-   Total Employees
-   Employees Left
-   Employees Stayed
-   Attrition Rate
-   Average Age
-   Average Experience

### Interactive Slicers

-   Gender
-   Ever Benched
-   Payment Tier

### Analytical Visuals

-   Attrition Rate by Joining Year
-   Attrition Rate by Experience
-   Attrition Rate by Gender
-   Attrition Rate by City
-   Attrition Rate by Education

------------------------------------------------------------------------

# 🔍 Key Insights

## 1. Overall Attrition

The dataset contains **4,653 employees**, of whom **1,600 have left**,
resulting in an overall attrition rate of **34.39%**.

This indicates that roughly one out of every three employees in the
dataset has left the organization.

------------------------------------------------------------------------

## 2. Gender-wise Attrition

  Gender     Employees   Employees Left   Attrition Rate
  -------- ----------- ---------------- ----------------
  Female         1,875              884       **47.15%**
  Male           2,778              716       **25.77%**

Female employees have a substantially higher observed attrition rate
than male employees in this dataset.

> This is an observed association, not proof that gender itself causes
> attrition. HR should investigate underlying factors such as role,
> compensation, location, tenure, and career opportunities.

------------------------------------------------------------------------

## 3. City-wise Attrition

  City          Attrition Rate
  ----------- ----------------
  Pune              **50.39%**
  New Delhi         **31.63%**
  Bangalore         **26.71%**

Pune has the highest attrition rate among the three cities, at
approximately **50.39%**.

This makes Pune a strong area for further HR investigation.

------------------------------------------------------------------------

## 4. Education-wise Attrition

  Education     Attrition Rate
  ----------- ----------------
  Masters           **48.80%**
  Bachelors         **31.35%**
  PHD               **25.14%**

Employees with a Master's degree have the highest observed attrition
rate in the dataset.

A possible business question for HR would be whether highly qualified
employees have different career expectations, compensation gaps, or
external opportunities.

------------------------------------------------------------------------

## 5. Attrition by Joining Year

The dashboard shows substantial variation across joining years.

The most notable observation is **2018**, where the attrition rate is
approximately **98.64%**.

This is an unusually extreme value and should be investigated before
using it as a business conclusion. It may reflect the way the dataset
was collected or the relationship between joining year and the
observation period rather than a normal employee-retention pattern.

------------------------------------------------------------------------

## 6. Attrition by Experience

Attrition varies across employees with different levels of experience in
their current domain.

The highest observed rate is around **38% for employees with 3 years of
experience**, while employees with 6--7 years show lower rates, although
those groups contain very few records.

Therefore, experience should be interpreted together with sample size
rather than using the percentage alone.

------------------------------------------------------------------------

## 7. Bench Status

Employees who have been benched show a higher observed attrition rate:

  Ever Benched     Attrition Rate
  -------------- ----------------
  Yes                  **45.40%**
  No                   **33.13%**

This suggests that benching may be associated with increased attrition
and could be worth investigating from a workforce-utilization and
employee-engagement perspective.

------------------------------------------------------------------------

## 8. Payment Tier

The dataset also shows substantial variation in attrition by payment
tier:

  Payment Tier     Attrition Rate
  -------------- ----------------
  Tier 1               **36.63%**
  Tier 2               **59.91%**
  Tier 3               **27.52%**

Payment Tier 2 has the highest observed attrition rate at approximately
**59.91%**.

This is a strong segment for further investigation into compensation,
job roles, location, and employee demographics.

------------------------------------------------------------------------

# 💡 Business Recommendations

Based on the analysis, HR could consider the following actions:

### 1. Investigate High-Attrition Locations

Pune shows an attrition rate above 50%. HR should investigate
location-specific factors such as management, workload, compensation,
commuting, and career opportunities.

### 2. Investigate Payment Tier 2

Tier 2 employees show the highest attrition rate. Compensation
structure, role distribution, and career progression should be analyzed
for this group.

### 3. Reduce Bench-Related Attrition

Employees who have been benched show higher attrition. Improving project
allocation, internal mobility, and communication during bench periods
may help retention.

### 4. Investigate Master's-Level Attrition

The high attrition rate among Master's employees may indicate
career-growth or compensation concerns and deserves deeper analysis.

### 5. Validate the 2018 Cohort

The extremely high 2018 attrition rate should be validated against the
source data before making any operational decision.

------------------------------------------------------------------------

# 🔄 Project Workflow

``` text
Raw Employee Data
        ↓
Data Preparation
        ↓
Power Query
        ↓
DAX Measures
        ↓
Interactive Power BI Dashboard
        ↓
Attrition Analysis
        ↓
Business Insights
        ↓
Recommendations
```

------------------------------------------------------------------------

# 🧠 Skills Demonstrated

-   Power BI
-   DAX
-   Power Query
-   Data Cleaning
-   Exploratory Data Analysis
-   KPI Development
-   Data Visualization
-   Business Analysis
-   Dashboard Design
-   Insight Generation
-   HR Analytics

------------------------------------------------------------------------

# 🎯 Project Outcome

This project demonstrates how raw employee data can be transformed into
an interactive HR analytics solution.

The dashboard allows users to explore attrition patterns through
demographic and workforce dimensions and helps identify employee groups
and business areas that may require further investigation.

------------------------------------------------------------------------

## 👨‍💻 Author

**Aadil**

Data Analytics Project \| Power BI
