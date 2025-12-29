
# 🏥Patient Readmission Analysis

This repository contains SQL queries and visualizations for analyzing **patient readmission patterns** using a healthcare dataset.  
The goal is to classify patients into meaningful groups (diagnoses severity, age group, admissions history, blood pressure stage, blood sugar status, length of stay) and generate insights that can guide hospital management and clinical decision-making.

---

## 📊 Dataset
**Source:** `PATIENT.DATA.INFORMATION` 
Contains patient-level information including:
- `PATIENT_ID`
- `GENDER`
- `AGE`
- `READMISSION`
- `NUMBER_OF_DIAGNOSES`
- `PREVIOUS_ADMISSIONS`
- `BLOOD_PRESSURE`
- `BLOOD_SUGAR_LEVELS`
- `LENGTH_OF_STAY`

---

## 🎯 Objective
To classify patients into meaningful groups (diagnoses severity, age group, admissions history, blood pressure stage, blood sugar status, length of stay) and analyze readmission patterns for actionable healthcare insights.

## 📝 Analysis Logic

### Classification Columns
🧾 NUMBER_OF_DIAGNOSES_GROUP**  
  - 0–2 → Minor  
  - 3–5 → Normal  
  - 6–8 → High  
  - 9+ → Severe  

  👥 AGE_GROUP**  
  - 0–18 → Teenager  
  - 19–30 → Young Adult  
  - 31–49 → Adult  
  - 50–64 → Elder  
  - 65+ → Senior  

  🕒 PREVIOUS_ADMISSIONS_DURATION**  
  - 0–2 → Low  
  - 3–5 → High  
  - 6+ → Critical  

  💓 BLOOD_PRESSURE_STAGE**  
  - 0–120 → Normal  
  - 121–129 → Elevated  
  - 130–139 → High  
  - 140–180 → Very High  
  - 181+ → Critical  

  🩸 BLOOD_SUGAR_LEVELS_STATUS**  
  - 3.0–4.0 → Low  
  - 5.0–7.0 → Excellent  
  - 8.0–11.0 → Good  
  - 12.0+ → Very High  

  🏥 LENGTH_OF_STAY_DURATION**  
  - 0–2 → Short Stay  
  - 3–7 → Long Stay  
  - 8+ → Over Stay  

## 🎯 Key Insights:
 - Elderly patients with multiple diagnoses, longer stays, and abnormal vitals are at the highest risk of readmission.

 - Preventive care strategies should focus on critical-risk groups: seniors, patients with 3+ prior admissions, and those with severe diagnoses.

 - Monitoring blood pressure and sugar levels can help reduce readmission rates

## 🛠️ Tools Used:
🧠 Miro — Used for workflow design

📊 Excel — Used for data cleaning, exploration, and preliminary analysis

❄️ Snowflake — Used for data storage, querying, and analytical processing

🎨 Canva — Used for presentation materials
