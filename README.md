# HR-ATTRITION-ANALYSIS-PROJECT

<img width="1316" height="738" alt="PROJECT" src="https://github.com/user-attachments/assets/9f866135-11c8-44f1-9abb-a775efc022ed" />


 HR ANALYSIS OF ATTRITION – Power BI Project Explanation
 
**Project Overview**

The **HR Attrition Analysis Dashboard** is designed to analyze employee turnover patterns within an organization.

The objective of this project is to:

* Identify key factors contributing to employee attrition
* Analyze attrition by department, age group, gender, marital status, and salary
* Provide data-driven insights to reduce employee turnover

This dashboard helps HR managers and business leaders make strategic workforce decisions.

 Dataset Description

The dataset contains employee-related information such as:

* Employee ID
* Age
* Gender
* Department
* Job Role
* Marital Status
* Education Field
* Salary
* Hourly Rate
* Job Satisfaction
* Overtime
* Attrition (Yes/No)

**Data Preparation (Power Query)**

Steps performed in Power BI:

1. Imported HR dataset (CSV/Excel/SQL)
2. Cleaned null values
3. Created calculated columns:

   * **Age Group** (26–35, 36–45, 46–55, 55+)
   * Salary Slab (10k–15k, 15k+)
4. Converted data types properly
5. Removed duplicates


  **DAX Measures Used**

Some important DAX measures created:

 Attrition Count

DAX
Attrition_Count = CALCULATE(COUNT(Employee[EmployeeID]), Employee[Attrition] = "Yes")


 Total Income

```DAX
Total_Income = SUM(Employee[MonthlyIncome])
```

 **Average Salary**

```DAX
Avg_Salary = AVERAGE(Employee[MonthlyIncome])
```

** Overtime Count**

```DAX
Over_Time = CALCULATE(COUNT(Employee[EmployeeID]), Employee[OverTime] = "Yes")
```

---

** Dashboard KPI Cards (Top Section)
**
Your dashboard includes key performance indicators:

* **Attrition Count → 102**
* **Total Income → 2M**
* **Sum of Over Time → 27**
* **Max Salary → 20K**
* **Average Salary → 17.18K**

These KPIs give a quick summary of workforce metrics.

---

**Visual Analysis Explanation* Job Role by Attrition & Age Group (Clustered Column Chart)

Shows:

* Most attrition happens in **26–35 age group**
* Mid-career employees are more likely to leave
* Younger workforce has higher mobility



**Job Satisfaction by Salary Slab (Donut Chart)**

Insight:

* Majority of employees fall in **15K+ salary slab**
* Higher salary correlates with better satisfaction



 **Sum of Hourly Rate (Gauge Chart)**

* Displays total hourly compensation (6817)
* Helps track workforce cost efficiency



 **Attrition by Department (Pie Chart)**

* **Research & Development** has highest attrition
* Sales is second
* HR has lowest attrition

This helps management focus retention strategies on specific departments.



** Attrition by Marital Status (Bar Chart)
**
* Married employees show highest attrition count
* Divorced and Single follow

This may indicate work-life balance factors.



 **Department by Attrition & Marital Status**

* Married employees in R&D show significant attrition
* Helps combine demographic and department-level insights


**Slicers Used**

Left panel includes filters for:

* Education Field
* Gender
* Department
* Marital Status
* Job Role

These slicers allow dynamic filtering and interactive analysis.



** Key Business Insights**

✔ Highest attrition occurs in 26–35 age group
✔ Research & Development department needs retention strategies
✔ Overtime employees may be more prone to attrition
✔ Salary and job satisfaction are related
✔ Married employees show higher attrition trend



 **Business Recommendations**

1. Improve work-life balance policies
2. Reduce excessive overtime
3. Offer career growth programs for mid-age employees
4. Provide performance-based salary increments
5. Conduct satisfaction surveys in R&D department



 ** Tools & Technologies Used
**
* Power BI Desktop
* Power Query
* DAX
* Data Modeling
* Interactive Visualizations


** Conclusion
**
This HR Attrition Analysis dashboard helps the organization:

* Understand why employees leave
* Identify high-risk departments
* Improve employee retention strategies
* Make informed HR decisions

It transforms raw HR data into actionable business intelligence.


