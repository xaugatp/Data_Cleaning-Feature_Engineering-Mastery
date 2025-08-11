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

<details>
<summary>📅 <strong>Week 4 – Categorical Encoding & Cardinality Control</strong></summary>

### 🎯 Objectives
- Clean categories (trim, unify, typo map)
- Group rare labels
- Apply safe encodings (OHE, ordinal, target/CatBoost, hashing) with CV

### 📦 Deliverables
- Encoding matrix per feature
- Leakage-safe encoding wrapper

### 🛠 Mini-project
> Encode categorical vars in Titanic; benchmark One-Hot vs Target encoding.

### 🎓 Short course
[Kaggle – Feature Engineering](https://www.kaggle.com/learn/feature-engineering)

📖 **PfDA 3e**: Ch7 §7.5, Ch7 §7.4, Ch12 §12.1–12.2
</details>

---

<details>
<summary>📅 <strong>Week 5 – Numerical Feature Creation</strong></summary>

### 🎯 Objectives
- Create groupby aggregations
- Engineer ratios/interactions
- Apply binning and transformations

### 📦 Deliverables
- Feature spec (name, formula, null policy, range)
- Top-k features by MI/Gini

### 🛠 Mini-project
> Create ride-duration and avg-speed features for NYC Taxi data; evaluate via CV.

### 🎓 Short course
[Kaggle – Feature Engineering](https://www.kaggle.com/learn/feature-engineering)

📖 **PfDA 3e**: Ch10 §10.1–10.4, Ch5 §5.3, Ch4 §4.3
</details>

---

<details>
<summary>📅 <strong>Week 6 – Dates, Time Features & Text Basics</strong></summary>

### 🎯 Objectives
- Extract date parts and cyclical encodings
- Add holiday flags and lags
- Text cleaning, counts, simple sentiment

### 📦 Deliverables
- Time-aware feature cookbook
- Text preprocessing pipeline

### 🛠 Mini-project
> Create lag features on retail sales; compute TF-IDF & sentiment on Tweets.

### 🎓 Short course
[Kaggle – Time Series](https://www.kaggle.com/learn/time-series) & NLP basics

📖 **PfDA 3e**: Ch11 §11.1–11.7, Ch6 §6.1, Ch7 §7.4
</details>

---

<details>
<summary>📅 <strong>Week 7 – Scaling, Normalization & Pipelines</strong></summary>

### 🎯 Objectives
- Apply scaling methods (Standard, Min-Max, Robust)
- Build scikit-learn Pipelines & ColumnTransformers
- Persist preprocessing with joblib

### 📦 Deliverables
- End-to-end preprocessing pipeline (fit/transform)
- Save/load demonstration

### 🛠 Mini-project
> Compare models with Min-Max vs StandardScaler on credit data within a Pipeline.

### 🎓 Short course
[scikit-learn – Preprocessing (User Guide)](https://scikit-learn.org/stable/modules/preprocessing.html)

📖 **PfDA 3e**: Ch12 §12.4, Ch12 §12.1
</details>

---

<details>
<summary>📅 <strong>Week 8 – Data Integration, Joins & Reshaping</strong></summary>

### 🎯 Objectives
- Perform safe merges with key audits
- Use anti-joins to find orphans
- Reshape with pivot/melt; use concat/append appropriately

### 📦 Deliverables
- Join QA checklist
- Keys coverage report (match rate, dupes, one-to-many audits)

### 🛠 Mini-project
> Merge ads spend with sales by date/region; quantify orphan rows and row inflation.

### 🎓 Short course
[Pandas merge/reshape documentation](https://pandas.pydata.org/docs/user_guide/merging.html)

📖 **PfDA 3e**: Ch8 §8.1–8.3, Ch6 §6.3–6.4
</details>

---

<details>
<summary>📅 <strong>Week 9 – Feature Selection & Dimensionality Reduction</strong></summary>

### 🎯 Objectives
- Apply filter (corr/MI), wrapper (RFE), and embedded (L1/trees) methods
- Explore PCA/UMAP for visualization
- Validate feature subsets without leakage

### 📦 Deliverables
- Feature selection report
- Compact, validated feature set

### 🛠 Mini-project
> Run RFE and L1 on churn data; compare baseline vs selected features.

### 🎓 Short course
[StatQuest – Feature Selection](https://www.youtube.com/watch?v=Q6f7m5Yb0P8)

📖 **PfDA 3e**: Ch12 §12.4, Ch10 (foundations)
</details>

---

<details>
<summary>📅 <strong>Week 10 – Data Quality Testing & Automation</strong></summary>

### 🎯 Objectives
- Create schema/range/null/uniqueness tests
- Add Pytest + (Pandera or Great Expectations)
- Wire basic CI to block failing data jobs

### 📦 Deliverables
- Pandera or GE suite
- pytest unit tests
- Pre-commit hooks and CI badge

### 🛠 Mini-project
> Create a Great Expectations suite for Titanic and fail the pipeline on violations.

### 🎓 Short course
[Great Expectations – Quickstart](https://greatexpectations.io/)

📖 **PfDA 3e**: Ch6 (I/O pitfalls), Ch3.3 (Files & OS)
</details>

---

<details>
<summary>📅 <strong>Week 11 – Domain Tracks (Choose 1–2)</strong></summary>

### ⏳ Time Series
- **Objectives:** Time-based splits, leakage prevention, lag/rolling features, calendar effects  
- **Mini-project:** M5-like retail demand subset with lags/rolls; evaluate on time-based CV  
- **Short course:** [Kaggle – Time Series](https://www.kaggle.com/learn/time-series)  
- **PfDA 3e:** Ch11 (full chapter)

### 📝 NLP
- **Objectives:** Text normalization vs retention, vocabulary drift, feature hashing for scale  
- **Mini-project:** IMDB reviews TF-IDF + sentiment classification; analyze leakage risks  
- **Short course:** [Kaggle – NLP](https://www.kaggle.com/learn/nlp)  
- **PfDA 3e:** Ch7 §7.4–7.5

### 🗺 Geospatial
- **Objectives:** Handle raster stacks & CRS alignment, compute NDVI/texture, aggregate patches  
- **Mini-project:** Compute NDVI from Sentinel-2 for a small AOI; build basic features  
- **Short course:** [Kaggle – Geospatial Analysis](https://www.kaggle.com/learn/geospatial-analysis)  
- **PfDA 3e:** External resources (not covered)
</details>

---

<details>
<summary>📅 <strong>Week 12 – Capstone: End-to-End, Reproducible & Documented</strong></summary>

### 🎯 Objectives
- Package your pipeline with custom transformers
- Document reproducible steps and lock environments
- Present metrics comparing baseline vs engineered features

### 📦 Deliverables
- Packaged `src/` with CLI entry point
- README with repro steps
- Environment lockfile
- Model metrics report

### 🛠 Mini-project
> Single-command pipeline from raw → clean → features → model evaluation producing a `reports/` bundle.

### 🎓 Short course
Review prior resources; skim sklearn docs for any gaps

📖 **PfDA 3e**: Ch13, skim Ch5, Ch7, Ch8, Ch10
</details>

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
MIT License — free to learn, share, and adapt.

Copyright (c) 2025 Saugat Poudel

---

## 📣 Share Your Progress
If you complete a week, share your mini-project on GitHub with the tag:  
