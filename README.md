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

**1. Attrition Count**
```tableau
IF [Attrition] = 'Yes' THEN 1 ELSE 0 END

2. Attrition Rate

tableau
Copy
Edit
SUM([Attrition Count]) / SUM([Employee Count])
3. Active Employees

tableau
Copy
Edit
SUM([Employee Count]) - SUM([Attrition Count])
4. Average Age

tableau
Copy
Edit
AVG([Age])
🔍 EDA (Exploratory Data Analysis) Steps
Distribution of employee age and gender

Correlation between job satisfaction and attrition

Attrition rates by department, education field, and age group

Job roles with high attrition rates

Gender distribution across departments

🧠 Data Modeling (in Tableau)
Calculated Fields for KPIs

Grouping age into bins (e.g., 20-30, 30-40, etc.)

Data filters by gender, department, and age group

Data blending not required (single dataset)

📊 Visualizations Used
KPI Cards: Employees Count, Attrition Count, Attrition Rate, Avg. Age

Pie Chart: Department-wise Attrition

Bar Chart: Employees by Age Group

Line/Bar: Attrition by Gender for Age Groups

Bar Chart: Education Field vs Attrition

Job Satisfaction Rating: Distribution (Histogram or Bar)

🔑 Key Findings
Higher attrition rates in younger age groups (20-30)

Specific departments show elevated attrition

Lower job satisfaction is directly tied to increased attrition

Gender-based differences in attrition for specific age bands

💼 Business Impact
Strategic retention initiatives for departments with high attrition

Policy changes to address dissatisfaction in early-career employees

Focused efforts on gender equity and workplace engagement

📌 Insights & Inference
Attrition is not evenly distributed—age, department, and job satisfaction are strong drivers.

Intervening early with targeted employee programs could reduce attrition rates.

Dashboards help stakeholders monitor and react to workforce dynamics in real-time.

✅ Conclusion
This HR Analyst Dashboard provides a powerful tool for identifying and addressing factors related to employee attrition. Using Tableau’s interactivity, HR teams can drill down into key dimensions and implement strategies based on data-driven insights.

📷 Dashboard Preview
<img width="1157" height="652" alt="Image" src="https://github.com/user-attachments/assets/0d6c7a4c-9084-4d38-9f15-6ed6d066d519" />

📜 License
This project is licensed under the MIT License.


## 🔗 Author
 
📧 Gmail:[jayeshpardeshi161@gmail.com]  
📌 LinkedIn:[] 
📌 Portfolio:[]

---

