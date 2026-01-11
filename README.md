# Hospital Emergency Room Dashboard Analysis

##  Project Overview
This project focuses on building an end-to-end **Hospital Emergency Room Analysis Dashboard** to improve operational efficiency and support data-driven decision-making.  
The dashboard helps hospital stakeholders monitor patient flow, wait times, admissions, and department referrals.

---

##  Objective
- Analyze emergency room patient data
- Track key performance indicators (KPIs)
- Identify bottlenecks in patient wait times
- Provide insights to improve emergency services

---

##  Dataset
- **Source:** Hospital Emergency Room Data
- **Format:** CSV
- **Key Attributes:** Patient age, gender, admission status, wait time, department referrals

---

##  Tools & Technologies
- Microsoft Excel
- Power BI
- Pivot Tables
- DAX
- Data Visualization

---

##  KPIs Tracked
- Patient Admission Status (Admitted vs Not Admitted)
- Percentage of patients seen within 30 minutes
- Patient Age Group Distribution
- Gender-wise Patient Analysis
- Department Referral Analysis

---

##  Dashboard Visualizations
- Admission status comparison
- Age group segmentation
- Timeliness analysis (Within time vs Delayed)
- Gender distribution
- Department-wise referral trends

---

##  Key DAX Calculations
**Age Group Classification**
```DAX
Age Group = 
IF([Patient Age]>=70,"70-79",
IF([Patient Age]>=60,"60-69",
IF([Patient Age]>=45,"45-59",
IF([Patient Age]>=30,"30-44",
IF([Patient Age]>=15,"15-29",
IF([Patient Age]>=5,"05-14","0-4"))))))
