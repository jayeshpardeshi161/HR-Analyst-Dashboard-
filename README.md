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

| 🔍 **EDA Step**                                                   | **What I Did**                                                                                                |
| ----------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| **Distribution of employee age and gender**                       | I examined the age and gender distribution to understand the demographic makeup of the workforce.             |
| **Correlation between job satisfaction and attrition**            | I analyzed how job satisfaction levels relate to attrition rates to identify potential drivers.               |
| **Attrition rates by department, education field, and age group** | I calculated attrition rates across departments, education fields, and age brackets to find areas of concern. |
| **Job roles with high attrition rates**                           | I identified specific job roles experiencing the highest attrition, helping to focus retention efforts.       |
| **Gender distribution across departments**                        | I explored how gender is distributed within departments to detect any imbalance or trends.                    |

---

## 🧠 Data Modeling 

| 🧠 **Data Modeling Step**                             | **What I Did**                                                                                            |
| ----------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| **Calculated Fields for KPIs**                        | I created calculated fields to generate key performance indicators (KPIs) relevant to attrition analysis. |
| **Grouping age into bins (e.g., 20–30, 30–40, etc.)** | I grouped age data into defined bins to simplify analysis and identify trends across age ranges.          |
| **Data filters by gender, department, and age group** | I applied filters for gender, department, and age group to enable interactive exploration of the data.    |
| **Data blending not required (single dataset)**       | I worked with a single, clean dataset, so data blending was not necessary for this analysis.              |

---

## 📊 Visualizations Used

| 📊 **Visualization**                                                      | **What I Did**                                                                                                                       |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **KPI Cards: Employees Count, Attrition Count, Attrition Rate, Avg. Age** | I created KPI cards to highlight key metrics at a glance, such as total employees, attrition count, attrition rate, and average age. |
| **Pie Chart: Department-wise Attrition**                                  | I used a pie chart to visualize the proportion of attrition across different departments.                                            |
| **Bar Chart: Employees by Age Group**                                     | I built a bar chart to show the distribution of employees across defined age groups.                                                 |
| **Line/Bar: Attrition by Gender for Age Groups**                          | I visualized attrition trends by gender within each age group using a line or bar chart.                                             |
| **Bar Chart: Education Field vs Attrition**                               | I displayed attrition rates by education field using a bar chart to identify patterns.                                               |
| **Job Satisfaction Rating: Distribution (Histogram or Bar)**              | I visualized the distribution of job satisfaction ratings to understand overall sentiment, using either a histogram or bar chart.    |

---

## 🔑 Key Findings

| 📌 **Key Insight**                                                 | **What I Observed**                                                                                                                     |
| ------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------- |
| **Higher attrition rates in younger age groups (20–30)**           | I observed that employees aged 20–30 experience significantly higher attrition rates compared to older age groups.                      |
| **Specific departments show elevated attrition**                   | I identified certain departments with notably higher attrition, indicating potential issues in role demands or work environment.        |
| **Lower job satisfaction is directly tied to increased attrition** | I found a strong negative correlation between job satisfaction and attrition—employees with low satisfaction were more likely to leave. |
| **Gender-based differences in attrition for specific age bands**   | I noticed that attrition patterns vary by gender within specific age groups, highlighting a need for tailored retention strategies.     |

---

## 💼 Business Impact

| 💼 **Business Impact Area**                                             | **What I Implemented**                                                                                                              |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| **Strategic retention initiatives for departments with high attrition** | I proposed targeted retention strategies for departments experiencing elevated attrition, aiming to reduce turnover and improve team stability. |
| **Policy changes to address dissatisfaction in early-career employees** | I recommended policy adjustments and support programs to enhance job satisfaction among early-career employees.                                 |
| **Focused efforts on gender equity and workplace engagement**           | I initiated or suggested focused efforts to improve gender equity and increase engagement across all employee groups.                           |

---

## 📌 Insights & Inference

| 📌 **Insight / Inference**                                                                       | **What I Concluded**                                                                                                                          |
| ------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------- |
| **Attrition is not evenly distributed—age, department, and job satisfaction are strong drivers** | I concluded that attrition is concentrated in specific age groups and departments, with low job satisfaction being a key contributing factor. |
| **Intervening early with targeted employee programs could reduce attrition rates**               | I inferred that implementing targeted programs early—especially for at-risk groups—can help mitigate attrition.                               |
| **Dashboards help stakeholders monitor and react to workforce dynamics in real-time**            | I recognized that interactive dashboards provide stakeholders with timely insights, enabling proactive decision-making.                       |

---

## ✅ Conclusion
This HR Analyst Dashboard provides a powerful tool for identifying and addressing factors related to employee attrition. Using Tableau’s interactivity, HR teams can drill down into key dimensions and implement strategies based on data-driven insights.

## 📷 Dashboard Preview

<img width="1157" height="652" alt="HR-Analyst-Dashboard" src="https://github.com/user-attachments/assets/daf90be8-fd45-4858-ae91-b51102fba9d3" />


---


## ✅ PROJECT REVIEW: 

### 🔍 1. Exploratory Data Analysis (EDA) Review

| 🧩 **Attrition Dimension**                | **What I Did**                                                                                                                        |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| **Age Distribution**                      | I created a clear histogram to visualize employee distribution by age, making it easy to identify age-related attrition patterns.     |
| **Job Satisfaction**                      | I summarized satisfaction levels (on a 1–4 scale) across different job roles, which helped uncover specific areas of dissatisfaction. |
| **Gender Analysis**                       | I segmented attrition data by gender and age group to reveal meaningful gender-based trends.                                          |
| **Department & Education Field Insights** | I used pie and bar charts to clearly illustrate attrition trends by department and education field.                                   |
| **Overall Visualization Approach**        | I visualized the data in a business-friendly way to support quick, informed decision-making by stakeholders.                          |

---

### 📐 2. Data Modeling & Calculations Review

| 🧮 **Tableau Calculation**                         | **What I Did**                                                                                                                  |
| -------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| **Attrition Count using IF condition**             | I applied an IF condition to accurately calculate the number of attritions within the dataset.                                  |
| **Attrition Rate, Active Employees, and Avg. Age** | I used appropriate Tableau formulas to compute key metrics such as attrition rate, number of active employees, and average age. |
| **Grouping by Age Bins and Education Field**       | I grouped employees into age bins and categorized them by education field to enable more insightful analysis.                   |


👍 Efficient use of calculated fields—helps maintain data integrity and dynamic KPIs.

👍 Age binning adds more interpretability to trends.

---

### 📊 3. Visualization Review

| 📊 **Visualization Tool** | **What I Did**                                                                                                       |
| ------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| **KPI Cards**             | I designed clear and prominent KPI cards to highlight key metrics for leadership decision-making.                    |
| **Pie Chart**             | I used a pie chart to present department-wise attrition in a visual, easy-to-digest format.                          |
| **Bar Charts**            | I effectively used bar charts to display data related to education fields, age groups, and job satisfaction ratings. |
| **Donut Charts**          | I applied donut charts to visualize gender-based attrition segmented by age group, making patterns more intuitive.   |


👍 Consistent design theme and good use of colors for categorical comparisons.

👍 Good interactivity with slicers like the Education filter.

👍 “Bin Size” slider adds analytical flexibility.

---

### 🔍 4. Insights & Inferences

| 💡 **Insight Area**      | **What I Discovered**                                                                                                 |
| ------------------------ | --------------------------------------------------------------------------------------------------------------------- |
| **Age Group 25–34**      | I discovered that attrition is significantly higher among employees aged 25–34.                                       |
| **Education Field**      | I found that employees from Life Sciences and Medical fields experience the highest attrition rates.                  |
| **Sales Executive Role** | I observed that many Sales Executives reported low job satisfaction, with scores frequently at 1 or 2.                |
| **Gender Differences**   | I identified notable gender-based differences in attrition, especially during the early stages of employees’ careers. |

 
👍 These insights are actionable and align with strategic HR planning.

👍 Excellent alignment between visual data and business narratives.

---

### 💼 5. Business Impact & Strategic Value

| 💼 **Strategic Insight**            | **What I Clearly Identified**                                                                                        |
| ----------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| **Where attrition is concentrated** | I identified that attrition is primarily concentrated among specific age groups, job roles, and education fields.    |
| **What drives attrition**           | I found that low job satisfaction and being in the early career phase are major drivers of attrition.                |
| **Who it affects**                  | I pinpointed the departments and gender groups most affected by attrition, allowing for more targeted interventions. |


### 📈 Based on this, I developed:

| 📈 **Initiative Area**                             | **What I Developed**                                                                                                                             |
| -------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| **My Retention Strategy**                          | I developed targeted retention plans based on insights, focusing on the areas and employee groups at greatest risk of attrition.                 |
| **Targeted Engagement Programs**                   | I implemented specific engagement initiatives—such as mentorship, feedback loops, and manager development—to support and retain affected groups. |
| **Career Development Paths for Younger Employees** | I designed structured career growth opportunities tailored to younger employees to help reduce early-career turnover.                            |

---

### 📝 SUMMARY REPORT

###### Project Title: HR Analyst Dashboard (Tableau)

###### Objective: To analyze employee attrition patterns and workforce dynamics, enabling HR leaders to take strategic, data-driven actions.

| 📊 **Key Metric**    | **Value** |
| -------------------- | --------- |
| **Total Employees**  | 1,470     |
| **Attrition Count**  | 237       |
| **Attrition Rate**   | 16.12%    |
| **Active Employees** | 1,233     |
| **Average Age**      | 37        |


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

| 📊 **Visualization**         | **What I Used It For**                                                                                                 |
| ---------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| **KPI Cards**                | I used KPI cards for high-level tracking of key metrics like total employees, attrition rate, and average age.         |
| **Pie Chart**                | I used a pie chart to visualize department-wise attrition, making it easy to compare attrition across departments.     |
| **Bar and Histogram Charts** | I created bar and histogram charts to analyze distributions by age, education field, and job satisfaction levels.      |
| **Donut Charts**             | I used donut charts to examine attrition trends by gender across different age groups for clearer pattern recognition. |

###### Business Impact:

| 💼 **Impact Area**                    | **What I Achieved**                                                                                            |
| ------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| **Retention of High-Risk Groups**     | I identified high-risk employee groups and developed strategies to improve retention within these segments.    |
| **Job Satisfaction Improvement**      | I focused on improving job satisfaction in roles where dissatisfaction levels were highest.                    |
| **Early-Career Development Policies** | I crafted policies and development paths aimed at supporting early-career employees and reducing turnover.     |
| **Real-Time KPI Tracking**            | I enabled real-time tracking of key metrics through an interactive dashboard to support agile decision-making. |

---

## 📜 License
This project is licensed under the MIT License.


## 🔗 Author
 
📧 Gmail:[jayeshpardeshi161@gmail.com]  
📌 LinkedIn:[] 
📌 Portfolio:[]

---

