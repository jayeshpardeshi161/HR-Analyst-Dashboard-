# HR Analyst Dashboard (Tableau Project)

## 📊 Project Summary
This project involves the creation of an interactive Tableau dashboard to analyze HR-related metrics from a sample HR dataset. The goal is to assist HR departments in understanding employee attrition patterns and workforce demographics, enabling data-driven decisions to improve employee retention and satisfaction.

---

## 🎯 Project Goals
- Analyze employee attrition across multiple dimensions (age, gender, department, education, etc.)
- Provide visual insights into employee satisfaction and attrition trends
- Build a self-service dashboard for HR teams to track KPIs in real time

---

## 📂 Dataset Overview
- **File**: `HR Data.csv`
- **Rows**: 1,470
- **Columns**: 39
- **Key Columns**: `Age`, `Attrition`, `Department`, `Gender`, `JobSatisfaction`, `EducationField`, `EmployeeCount`

---

## ❓ Problem Statement
Employee attrition is costly and disruptive. This dashboard aims to uncover the key factors that contribute to attrition and present actionable insights for HR management to improve employee retention and engagement.

---

## 🧮 KPIs & Tableau Calculated Fields

To build the core metrics, I created custom calculated fields within Tableau to derive the following KPIs:

| **Metric Name**      | **Tableau Calculated Field**                     | **Purpose**                                                                 |
| -------------------- | ------------------------------------------------ | --------------------------------------------------------------------------- |
| **Attrition Count**  | `IF [Attrition] = 'Yes' THEN 1 ELSE 0 END`       | To quantify the number of employees who have left the organization.         |
| **Attrition Rate**   | `SUM([Attrition Count]) / SUM([Employee Count])` | To measure the proportion of employees who left out of the total workforce. |
| **Active Employees** | `SUM([Employee Count]) - SUM([Attrition Count])` | To calculate the number of employees currently active within the company.   |
| **Average Age**      | `AVG([Age])`                                     | To determine the average age of the workforce, helping identify age trends. |


---

## 🔍 EDA (Exploratory Data Analysis) Steps
Distribution of employee age and gender

Correlation between job satisfaction and attrition

Attrition rates by department, education field, and age group

Job roles with high attrition rates

Gender distribution across departments

---

## 🧠 Data Modeling (in Tableau)
Calculated Fields for KPIs

Grouping age into bins (e.g., 20-30, 30-40, etc.)

Data filters by gender, department, and age group

Data blending not required (single dataset)

---

## 📊 Visualizations Used
KPI Cards: Employees Count, Attrition Count, Attrition Rate, Avg. Age

Pie Chart: Department-wise Attrition

Bar Chart: Employees by Age Group

Line/Bar: Attrition by Gender for Age Groups

Bar Chart: Education Field vs Attrition

Job Satisfaction Rating: Distribution (Histogram or Bar)

---

## 🔑 Key Findings
Higher attrition rates in younger age groups (20-30)

Specific departments show elevated attrition

Lower job satisfaction is directly tied to increased attrition

Gender-based differences in attrition for specific age bands

---

## 💼 Business Impact
Strategic retention initiatives for departments with high attrition

Policy changes to address dissatisfaction in early-career employees

Focused efforts on gender equity and workplace engagement

## 📌 Insights & Inference
Attrition is not evenly distributed—age, department, and job satisfaction are strong drivers.

Intervening early with targeted employee programs could reduce attrition rates.

Dashboards help stakeholders monitor and react to workforce dynamics in real-time.

---

## ✅ Conclusion
This HR Analyst Dashboard provides a powerful tool for identifying and addressing factors related to employee attrition. Using Tableau’s interactivity, HR teams can drill down into key dimensions and implement strategies based on data-driven insights.

## 📷 Dashboard Preview

<img width="1157" height="652" alt="HR-Analyst-Dashboard" src="https://github.com/user-attachments/assets/daf90be8-fd45-4858-ae91-b51102fba9d3" />


---


## ✅ PROJECT REVIEW: 

### 🔍 1. Exploratory Data Analysis (EDA) Review

You effectively explored key dimensions of attrition:

Age Distribution: Clear histogram visualization showing employee distribution by age.

Job Satisfaction: Nicely summarized by job role and satisfaction level (1–4 scale), which helps uncover dissatisfaction patterns.

Gender Analysis: Gender-based attrition is cleanly segmented by age group.

Department & Education Field Insights: Pie and bar charts concisely illustrate department and education-wise attrition trends.

- The data is visualized in a business-friendly way for decision-makers.

---

### 📐 2. Data Modeling & Calculations Review

You applied essential Tableau calculations effectively:

Attrition Count using IF condition

Attrition Rate, Active Employees, and Avg. Age computed via appropriate Tableau formulas

Grouping by Age bins and Education Field

👍 Efficient use of calculated fields—helps maintain data integrity and dynamic KPIs.

👍 Age binning adds more interpretability to trends.

---

### 📊 3. Visualization Review
You used a variety of visual tools:

KPI Cards: Clear and prominent for leadership.

Pie Chart: Department-wise attrition is visual and easy to digest.

Bar Charts: Strong use for education, age groups, and satisfaction ratings.

Donut Charts: Effective for gender-based attrition by age group.

👍 Consistent design theme and good use of colors for categorical comparisons.

👍 Good interactivity with slicers like the Education filter.

👍 “Bin Size” slider adds analytical flexibility.

---

### 🔍 4. Insights & Inferences

surfaced several impactful insights:

Higher attrition in age group 25-34

Life Sciences and Medical fields have the highest attrition

Sales Executive role shows dissatisfaction (many score 1 or 2)

Gender differences are notable in early-career attrition
 
👍 These insights are actionable and align with strategic HR planning.

👍 Excellent alignment between visual data and business narratives.

---

### 💼 5. Business Impact & Strategic Value
Clearly identified:

Where attrition is concentrated (age, job role, education)

What drives it (low job satisfaction, early career phase)

Who it affects (departments, genders)

### 📈 Based on this, I developed:

###### My Retention Strategy
→ The insights guide me in developing targeted retention plans focused on the areas and groups at greatest risk.

###### Targeted Engagement Programs
→ I can implement specific initiatives to improve engagement among the affected groups, such as mentorship, feedback loops, or manager development.

###### Career Development Paths for Younger Employees
→ I use these findings to create structured growth opportunities that support younger employees and reduce early-career turnover.

---

### 📝 SUMMARY REPORT

###### Project Title: HR Analyst Dashboard (Tableau)

###### Objective: To analyze employee attrition patterns and workforce dynamics, enabling HR leaders to take strategic, data-driven actions.

Key Metrics Tracked:
Total Employees: 1,470

Attrition Count: 237

Attrition Rate: 16.12%

Active Employees: 1,233

Average Age: 37

###### Key Findings:

Highest attrition in age 25–34 group (29.11%)

Life Sciences and Medical education fields show highest attrition

Sales Executives have lowest satisfaction levels

Male attrition slightly higher than female across all age groups

###### 🧠 Key Features & Insights

Real-Time KPI Monitoring: Tracks Employee Count, Attrition Count, Attrition Rate, Active Employees, and Average Age.

Attrition Breakdown:

By Age Groups: Highest in 25–34 age range (29.11%)

By Gender: Slightly higher among males across all age groups

By Department & Education Field: Life Sciences and Sales show elevated attrition

Job Satisfaction Analysis:

Role-specific satisfaction levels highlight areas for improvement (e.g., Sales Executives)

Strong correlation observed between low satisfaction and higher attrition

Education Field vs Attrition: Life Sciences, Medical, and Marketing fields show higher turnover rates.

###### Visualizations Used:

KPI Cards for high-level tracking

Pie chart for department attrition

Bar and histogram charts for age, education, and job satisfaction

Gender and age group analysis via donut charts

###### Business Impact:

Identify and retain high-risk employee groups

Improve job satisfaction in roles with high dissatisfaction

Craft policies for early-career employee development

Track KPIs in real-time via dashboard interactivity

---

## 📜 License
This project is licensed under the MIT License.


## 🔗 Author
 
📧 Gmail:[jayeshpardeshi161@gmail.com]  
📌 LinkedIn:[] 
📌 Portfolio:[]

---

