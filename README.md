# 🚀 12-Week Data Cleaning & Feature Engineering Mastery Guide

> **From raw data → clean dataset → powerful features → reproducible pipelines.**  
> A hands-on, portfolio-ready roadmap based on *Python for Data Analysis (3e)*, extended to 12 weeks with testing, leakage checks, geospatial/time series options, and automation/MLOps.

---

## 📅 Program Overview

| Week | Theme | Status |
|------|-------|--------|
| 1 | 🧹 Data Familiarity & Baseline Cleaning | [ ] |
| 2 | ❓ Missing Values Mastery | [ ] |
| 3 | 🚦 Outliers, Anomalies & Transformations | [ ] |
| 4 | 🏷️ Categorical Encoding & Cardinality Control | [ ] |
| 5 | ➕ Numerical Feature Creation | [ ] |
| 6 | ⏳ Dates, Time Features & Text Basics | [ ] |
| 7 | 📏 Scaling, Normalization & Pipelines | [ ] |
| 8 | 🔗 Data Integration, Joins & Reshaping | [ ] |
| 9 | 🎯 Feature Selection & Dimensionality Reduction | [ ] |
| 10 | 🧪 Data Quality Testing & Automation | [ ] |
| 11 | 🛠️ Domain Tracks (TS/NLP/Geo) | [ ] |
| 12 | 🏆 Capstone: End-to-End Pipeline | [ ] |

*(Replace `[ ]` with `[x]` as you complete each week!)*

---

## 🗂️ How to Use This Guide
1. **Click the week title** to expand details.  
2. Follow **Objectives** → **Deliverables** → **Mini-project** → **Short course**.  
3. Track progress in the table above.  
4. **Celebrate** after every week — data cleaning is a *superpower*. 🦸‍♀️

---

<details>
<summary>📅 <strong>Week 1 – Data Familiarity & Baseline Cleaning</strong></summary>

### 🎯 Objectives
- Audit schema, dtypes, and value ranges
- Unify naming conventions
- Remove duplicates
- Build a data dictionary

### 📦 Deliverables
- `data_dictionary.md`
- Column naming map
- Type-fix script
- Initial EDA/profile report

### 🛠 Mini-project
> Audit the Titanic dataset for naming consistency, duplicates, and dtype fixes.

### 🎓 Short course
[Kaggle – Pandas](https://www.kaggle.com/learn/pandas)

📖 **PfDA 3e**: Ch5 §5.1–5.2, Ch6 §6.1, Ch7 §7.2, Ch3.3
</details>

---

<details>
<summary>📅 <strong>Week 2 – Missing Values Mastery</strong></summary>

### 🎯 Objectives
- Quantify missingness
- Visualize patterns of NA
- Choose imputation strategy per feature (drop, constant, KNN, MICE)

### 📦 Deliverables
- Missingness report
- Imputation plan
- Before/after data quality table

### 🛠 Mini-project
> Use Missingno on the Housing dataset; test 3 imputation methods and compare downstream model impact.

### 🎓 Short course
[DataCamp – Handling Missing Data](https://www.datacamp.com/courses/handling-missing-data-in-python)

📖 **PfDA 3e**: Ch7 §7.1, Ch6 §6.1
</details>

---

<details>
<summary>📅 <strong>Week 3 – Outliers, Anomalies & Transformations</strong></summary>

### 🎯 Objectives
- Detect outliers (IQR, Z-score, robust methods)
- Decide treat vs keep using domain context
- Apply transformations (e.g., Yeo-Johnson/Box-Cox)

### 📦 Deliverables
- Outlier policy
- Transformation notebook
- Before/after distribution plots

### 🛠 Mini-project
> Apply IQR capping on Boston Housing; compare RMSE before vs after.

### 🎓 Short course
[Kaggle – Data Cleaning](https://www.kaggle.com/learn/data-cleaning)

📖 **PfDA 3e**: Ch7 §7.2, Ch4 §4.3–4.4, Appendix A
</details>

---

<!-- Repeat for weeks 4–12 in the same expandable format -->

---

## 🧠 Key Notes & Pro Tips
💡 **Avoid leakage:**  
- Always fit transformers only on training folds.  
- For target encoding, wrap inside CV folds or use encoders with built-in CV.

🔍 **Data QA:**  
- Run schema, bounds, null %, and uniqueness tests before merges and at outputs.

🗝 **Join hygiene:**  
- Track match rates and orphan rows with anti-joins.

📦 **Persistence:**  
- Save artifacts with `joblib`, version datasets with DVC.

---

## 📜 License
MIT — free to learn, share, and adapt.

---

## 📣 Share Your Progress
If you complete a week, share your mini-project on GitHub with the tag:  
