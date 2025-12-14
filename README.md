# 👥 HR Analytics & Employee Performance Dashboard (Power BI)

## 📊 Dashboard Overview

This Power BI dashboard helps organizations understand **employee performance, attrition, salary trends, training effectiveness, and workforce distribution**. It provides actionable insights to HR teams for improving employee retention, performance, and decision-making.

---

## 🧩 Problem Statement

The objective of this dashboard is to analyze **HR data** and identify:

* Employee attrition patterns
* Department-wise workforce distribution
* Salary trends across job roles
* Performance ratings and training impact
* Demographic insights (Gender, Education, Experience)

📌 **Why this matters:**
Understanding these factors helps HR teams reduce attrition, improve employee engagement, and optimize compensation and training strategies.

---

## 🔄 Steps Followed

### Step 1: Data Loading

* Loaded HR dataset into **Power BI Desktop** (CSV file).

### Step 2: Data Profiling (Power Query)

* Opened **Power Query Editor**
* Enabled:

  * Column Distribution
  * Column Quality
  * Column Profile
* Selected **Column profiling based on entire dataset**

### Step 3: Data Cleaning

* Checked for nulls and errors across columns
* Converted Yes/No fields into **Boolean (True/False)**
* Verified numeric fields like Salary, Experience, and Ratings

### Step 4: Data Modeling

* Ensured correct data types
* Created relationships (if applicable)
* Renamed columns for clarity

### Step 5: KPI Creation (DAX Measures)

Created key HR metrics:

* Total Employees
* Attrition Rate
* Average Salary
* Average Performance Rating

### Step 6: Dashboard Design

* Selected theme from **View → Themes**
* Designed a **single-page dashboard** with clean layout

### Step 7: Filters (Slicers)

Added slicers for:

* Department
* Gender
* Education

### Step 8: Visuals Used

* KPI Cards (Top section)
* Donut Chart – Employee Count by Gender
* Column Chart – Total Employees by Department
* Bar Chart – Average Training Hours by Department
* Column Chart – Average Salary by Job Role
* Scatter Plot – Experience vs Promotion Rate

---

## 🧮 DAX Measures Used

### Total Employees

```DAX
Total Employees = COUNT(Employee[Employee_ID])
```

### Attrition Rate

```DAX
Attrition Rate = 
DIVIDE(
    CALCULATE(COUNT(Employee[Employee_ID]), Employee[Attrition] = 1),
    COUNT(Employee[Employee_ID])
)
```

### Average Salary

```DAX
Average Salary = AVERAGE(Employee[Monthly_Salary])
```

### Average Performance Rating

```DAX
Average Performance Rating = AVERAGE(Employee[Performance_Rating])
```

---

## 📸 Dashboard Snapshot

📌 **Power BI Desktop / Service View**
https://github.com/Surajkanekar3797/HR-Analytics-Employee-Performance/blob/main/Dashboard.png.png

---

## 🔍 Insights & Findings

### 1️⃣ Workforce Overview

* **Total Employees:** 10,000
* Employees distributed almost evenly across departments

### 2️⃣ Attrition Analysis

* Attrition Rate highlights departments requiring retention strategies
* Helps HR identify risk-prone employee groups

### 3️⃣ Salary Analysis

* Salary varies significantly by **Job Role**
* Senior roles show higher average compensation

### 4️⃣ Training & Performance

* Departments with higher training hours tend to show better performance
* Training investment impacts employee productivity

### 5️⃣ Demographic Insights

* Gender distribution is balanced
* Education and experience influence salary and promotion rate

---

## 🚀 Conclusion

This HR Analytics dashboard enables data-driven HR decisions by providing clear insights into employee performance, compensation, training, and attrition. It can be used by HR managers to:

* Reduce employee attrition
* Improve performance management
* Optimize salary structures
* Enhance training programs

---

## 🛠 Tools & Technologies

* Power BI Desktop
* Power Query
* DAX
* CSV Dataset
* GitHub

---

## 👤 Author

**Suraj Kanekar**
Aspiring Data Analyst | Power BI | SQL | Excel | Python

⭐ *If you like this project, please star the repository!*
he repository!*

