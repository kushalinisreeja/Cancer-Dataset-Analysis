# 🔬 Cancer Patient Data Analysis

> Exploratory Data Analysis on a real-world oncology dataset to uncover survival patterns, treatment effectiveness, and clinical risk factors using Python.

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=flat-square&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=flat-square)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square)
![Status](https://img.shields.io/badge/Status-Complete-2ea043?style=flat-square)

---

## 📖 Overview

This project performs end-to-end **Exploratory Data Analysis (EDA)** on a cancer patient dataset spanning multiple countries. It covers data cleaning, feature engineering, statistical analysis, and visualization to extract meaningful clinical insights — following the same structured workflow used in real-world healthcare analytics.

---

## 📂 Dataset

| Property | Details |
|---|---|
| File | `dataset_med.csv` |
| Domain | Healthcare / Oncology |
| Target Variable | `survived` (0 = Deceased, 1 = Survived) |

**Features include:** `age`, `gender`, `country`, `cancer_stage`, `diagnosis_date`, `end_treatment_date`, `treatment_type`, `bmi`, `smoking_status`, `family_history`, `hypertension`, `asthma`, `cirrhosis`, `other_cancer`

---

## 🔄 Workflow

**Phase 1 — Data Cleaning**
- Removed duplicates and handled missing values
- Fixed data types: dates → `datetime`, age → `int`, categoricals → `category`
- Validated with `.info()`, `.describe()`, `.isnull()`

**Phase 2 — Feature Engineering**

| Feature | Description |
|---|---|
| `treatment_duration` | Days from diagnosis to end of treatment |
| `age_group` | Child / Adult / Senior-Citizen / Elder |
| `stage_group` | Early (Stage I–II) vs. Late (Stage III–IV) |
| `bmi_category` | Underweight / Normal / Overweight / Obese |
| `treatment_category` | Single vs. Combination therapy |
| `comorbidity_level` | None / 1 Condition / 2+ Conditions |

**Phase 3 — Exploratory Data Analysis**
- Demographics: age distribution, gender breakdown, country-wise stats
- Cancer stage: survival rate, death rate, age vs. stage
- Treatment: effectiveness by stage, single vs. combination therapy
- Survival factors: smoking, BMI, family history, comorbidities
- Country-level: survival rates, treatment duration comparison

**Phase 4 — Visualization**
- Histograms, count plots, box plots, heatmap, stacked bar charts

---

## 💡 Key Findings

- **Cancer stage at diagnosis** is the strongest predictor of survival
- **Combination therapy** outperforms single-mode treatment across most stages
- **Smokers** are more frequently diagnosed at advanced stages
- **2+ comorbidities** significantly reduce survival probability
- **Family history** patients tend to be diagnosed at a younger age
- Notable **country-level variation** in survival rates and treatment duration

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.8+ | Core language |
| Pandas | Data cleaning and feature engineering |
| Seaborn | Statistical visualization |
| Matplotlib | Custom charts and plots |
| Jupyter Notebook | Interactive analysis environment |


## 👩‍💻 Author

**Kushalini Sreeja**  
B.Tech CSE (Data Science) · Raghu Engineering College 

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin)](www.linkedin.com/in/kushalini-sreeja-mada)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=flat-square&logo=github)](https://github.com/kushalinisreeja)
