# 🏢 HR Data Analysis & Attrition Dashboard  

## 📌 Project Overview  
This **HR Data Analysis** project explores **employee attrition trends, job satisfaction, and work-life balance** using **SQL for analysis** and **Power BI for visualization**.  
The goal is to:  
✔ Identify **factors influencing employee attrition**.  
✔ Analyze **job roles, departments, and age groups** for retention insights.  
✔ Provide **data-driven solutions** for HR decision-making.  

---

## 📂 **Dataset Overview**  
The dataset includes **key HR attributes** such as:  
✔ **Demographics**: Age, Gender, Marital Status  
✔ **Employment Details**: Job Role, Department, Business Travel  
✔ **Compensation & Benefits**: Salary Hike, Stock Option Level  
✔ **Performance Metrics**: Job Satisfaction, Performance Rating  
✔ **Attrition Factors**: Over Time, Distance From Home, Work-Life Balance  

---

## 🔍 **SQL Data Analysis**  

### **Basic Queries:**  
✔ **Retrieve Employee Attrition Data**  
```sql
SELECT * FROM HR_Data WHERE Attrition = 'Yes';
```
✔ **Count Employees by Department**
```
SELECT Department, COUNT(*) AS EmployeeCount FROM HR_Data GROUP BY Department;
```
✔ **Find Average Monthly Income by Job Role**
```
SELECT Job_Role, AVG(Monthly_Income) AS AvgSalary FROM HR_Data GROUP BY Job_Role;
```

### **Basic Queries:**
✔ **Attrition Rate Calculation**
```
SELECT 
    Department, 
    COUNT(CASE WHEN Attrition = 'Yes' THEN 1 END) * 100.0 / COUNT(*) AS Attrition_Rate 
FROM HR_Data 
GROUP BY Department;
```
✔ **Impact of Work-Life Balance on Attrition**
```
SELECT Work_Life_Balance, COUNT(*) AS EmployeeCount 
FROM HR_Data 
WHERE Attrition = 'Yes' 
GROUP BY Work_Life_Balance;
```

---

# 📊 Power BI HR Dashboard  

## 📌 Project Overview  
This project involves **HR Data Analysis** using **SQL and Power BI**, focusing on **employee attrition, job satisfaction, and compensation trends**. The dashboard provides **interactive insights** for HR decision-making, helping organizations reduce attrition and improve employee satisfaction.  

---

## 🛠️ **Project Objectives**  
✔ **Analyze employee attrition patterns** to identify key risk factors.  
✔ **Evaluate job satisfaction and work-life balance** to enhance retention.  
✔ **Assess the impact of compensation, promotions, and overtime on attrition.**  
✔ **Provide interactive visualizations for actionable HR insights.**  

---

## 🛠️ **Dashboard Development Process**  

### **Step 1: Data Preprocessing & Cleaning**  
✔ **Handled missing values** by imputing or removing inconsistencies.  
✔ **Converted data types** for numerical and categorical attributes.  
✔ **Removed duplicates** for accurate reporting.  
✔ **Created calculated fields** for advanced analysis.  

---

### **Step 2: Dashboard Layout & Features**  

#### 📌 **Key Metrics (KPIs)**  
✔ **Total Employees**  
✔ **Attrition Rate**  
✔ **Average Age of Employees**  
✔ **Average Monthly Income**  

#### 📊 **Visuals Included in the Dashboard**  
✅ **Attrition Rate by Department** – Identifies departments with the highest attrition.  
✅ **Employee Count by Age Band** – Helps HR understand the age distribution.  
✅ **Attrition Trends by Gender & Marital Status** – Shows gender-based trends.  
✅ **Salary vs. Attrition Analysis** – Determines if salary impacts retention.  
✅ **Work-Life Balance vs. Attrition** – Evaluates how balance affects attrition.  
✅ **Overtime Impact on Attrition** – Highlights how working overtime influences employee retention.  

---

## 📊 **Key Insights from the Dashboard**  
✅ **The highest attrition rates are in the Sales and R&D departments.**  
✅ **Employees with poor work-life balance have a higher attrition risk.**  
✅ **Overtime significantly increases the chances of attrition.**  
✅ **Higher salary hikes and stock options improve employee retention.**  
✅ **Younger employees (under 30) tend to leave more often than older employees.**  

---

## 📩 **Connect with Me for Key Insights & Collaboration**  
📌 **LinkedIn:** [www.linkedin.com/in/ravirathod-me]  
🚀 **GitHub:** [https://github.com/imraviiiii]  
🌍 **Portfolio:** [https://www.notion.so/Ravi-Rathod-CV-Portfolio-1b047a47205980f09801d1d14dbf180f]  
