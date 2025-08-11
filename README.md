```json
{
  "program_name": "12-Week Data Cleaning & Feature Engineering Mastery Guide",
  "description": "A practical, portfolio-ready roadmap expanding a 10-week plan to 12 weeks, adding testing, leakage checks, geospatial/time series options, and automation/MLOps. Each week includes Objectives, Deliverables, a Mini-project, a Short course, and PfDA 3e chapter references.",
  "weeks": [
    {
      "week": 1,
      "title": "Data Familiarity & Baseline Cleaning",
      "objectives": [
        "Audit schema, dtypes, and value ranges",
        "Unify naming conventions",
        "Remove duplicates",
        "Build a data dictionary"
      ],
      "deliverables": [
        "data_dictionary.md",
        "Column naming map",
        "Type-fix script",
        "Initial EDA/profile report"
      ],
      "mini_project": "Audit the Titanic dataset for naming consistency, duplicates, and dtype fixes.",
      "short_course": "Kaggle – Pandas",
      "pfda_3e": ["Ch5 §5.1–5.2", "Ch6 §6.1", "Ch7 §7.2", "Ch3.3"]
    },
    {
      "week": 2,
      "title": "Missing Values Mastery",
      "objectives": [
        "Quantify missingness",
        "Visualize patterns of NA",
        "Choose imputation strategy per feature (drop, constant, KNN, MICE)"
      ],
      "deliverables": [
        "Missingness report",
        "Imputation plan",
        "Before/after data quality table"
      ],
      "mini_project": "Use Missingno on the Housing dataset; test 3 imputation methods and compare downstream model impact.",
      "short_course": "DataCamp – Handling Missing Data",
      "pfda_3e": ["Ch7 §7.1", "Ch6 §6.1"]
    },
    {
      "week": 3,
      "title": "Outliers, Anomalies & Transformations",
      "objectives": [
        "Detect outliers (IQR, Z-score, robust methods)",
        "Decide treat vs keep using domain context",
        "Apply transformations (e.g., Yeo-Johnson/Box-Cox)"
      ],
      "deliverables": [
        "Outlier policy",
        "Transformation notebook",
        "Before/after distribution plots"
      ],
      "mini_project": "Apply IQR capping on Boston Housing; compare RMSE before vs after.",
      "short_course": "Kaggle – Data Cleaning",
      "pfda_3e": ["Ch7 §7.2", "Ch4 §4.3–4.4", "Appendix A"]
    },
    {
      "week": 4,
      "title": "Categorical Encoding & Cardinality Control",
      "objectives": [
        "Clean categories (trim, unify, typo map)",
        "Group rare labels",
        "Apply safe encodings (OHE, ordinal, target/CatBoost, hashing) with CV"
      ],
      "deliverables": [
        "Encoding matrix per feature",
        "Leakage-safe encoding wrapper"
      ],
      "mini_project": "Encode categorical vars in Titanic; benchmark One-Hot vs Target encoding.",
      "short_course": "Kaggle – Feature Engineering",
      "pfda_3e": ["Ch7 §7.5", "Ch7 §7.4", "Ch12 §12.1–12.2"]
    },
    {
      "week": 5,
      "title": "Numerical Feature Creation",
      "objectives": [
        "Create groupby aggregations",
        "Engineer ratios/interactions",
        "Apply binning and transformations"
      ],
      "deliverables": [
        "Feature spec (name, formula, null policy, range)",
        "Top-k features by MI/Gini"
      ],
      "mini_project": "Create ride-duration and avg-speed features for NYC Taxi data; evaluate via CV.",
      "short_course": "Kaggle – Feature Engineering",
      "pfda_3e": ["Ch10 §10.1–10.4", "Ch5 §5.3", "Ch4 §4.3"]
    },
    {
      "week": 6,
      "title": "Dates, Time Features & Text Basics",
      "objectives": [
        "Extract date parts and cyclical encodings",
        "Add holiday flags and lags",
        "Text cleaning, counts, simple sentiment"
      ],
      "deliverables": [
        "Time-aware feature cookbook",
        "Text preprocessing pipeline"
      ],
      "mini_project": "Create lag features on retail sales; compute TF-IDF & sentiment on Tweets.",
      "short_course": "Kaggle – Time Series; NLP basics",
      "pfda_3e": ["Ch11 §11.1–11.7", "Ch6 §6.1", "Ch7 §7.4"]
    },
    {
      "week": 7,
      "title": "Scaling, Normalization & Pipelines",
      "objectives": [
        "Apply scaling methods (Standard, Min-Max, Robust)",
        "Build scikit-learn Pipelines & ColumnTransformers",
        "Persist preprocessing with joblib"
      ],
      "deliverables": [
        "End-to-end preprocessing pipeline (fit/transform)",
        "Save/load demonstration"
      ],
      "mini_project": "Compare models with Min-Max vs StandardScaler on credit data within a Pipeline.",
      "short_course": "scikit-learn – Preprocessing (user guide)",
      "pfda_3e": ["Ch12 §12.4", "Ch12 §12.1"]
    },
    {
      "week": 8,
      "title": "Data Integration, Joins & Reshaping",
      "objectives": [
        "Perform safe merges with key audits",
        "Use anti-joins to find orphans",
        "Reshape with pivot/melt; use concat/append appropriately"
      ],
      "deliverables": [
        "Join QA checklist",
        "Keys coverage report (match rate, dupes, one-to-many audits)"
      ],
      "mini_project": "Merge ads spend with sales by date/region; quantify orphan rows and row inflation.",
      "short_course": "Pandas merge/reshape documentation",
      "pfda_3e": ["Ch8 §8.1–8.3", "Ch6 §6.3–6.4"]
    },
    {
      "week": 9,
      "title": "Feature Selection & Dimensionality Reduction",
      "objectives": [
        "Apply filter (corr/MI), wrapper (RFE), and embedded (L1/trees) methods",
        "Explore PCA/UMAP for visualization",
        "Validate feature subsets without leakage"
      ],
      "deliverables": [
        "Feature selection report",
        "Compact, validated feature set"
      ],
      "mini_project": "Run RFE and L1 on churn data; compare baseline vs selected features.",
      "short_course": "StatQuest – Feature Selection",
      "pfda_3e": ["Ch12 §12.4", "Ch10 (as foundations)"]
    },
    {
      "week": 10,
      "title": "Data Quality Testing & Automation",
      "objectives": [
        "Create schema/range/null/uniqueness tests",
        "Add Pytest + (Pandera or Great Expectations)",
        "Wire basic CI to block failing data jobs"
      ],
      "deliverables": [
        "Pandera or GE suite",
        "pytest unit tests",
        "Pre-commit hooks and CI badge"
      ],
      "mini_project": "Create a Great Expectations suite for Titanic and fail the pipeline on violations.",
      "short_course": "Great Expectations – Quickstart",
      "pfda_3e": ["Ch6 (I/O pitfalls)", "Ch3.3 (Files & OS)"]
    },
    {
      "week": 11,
      "title": "Domain Tracks (choose 1–2)",
      "tracks": {
        "time_series": {
          "objectives": [
            "Time-based splits and leakage prevention",
            "Lag/rolling features, calendar effects"
          ],
          "mini_project": "M5-like retail demand subset with lags/rolls; evaluate on time-based CV.",
          "short_course": "Kaggle – Time Series",
          "pfda_3e": ["Ch11 (full chapter)"]
        },
        "nlp": {
          "objectives": [
            "Text normalization vs retention",
            "Vocabulary drift; feature hashing for scale"
          ],
          "mini_project": "IMDB reviews TF-IDF + sentiment classification; analyze leakage risks.",
          "short_course": "Kaggle – NLP (Intro)",
          "pfda_3e": ["Ch7 §7.4–7.5"]
        },
        "geospatial": {
          "objectives": [
            "Handle raster stacks and CRS alignment",
            "Compute NDVI/texture and aggregate patches"
          ],
          "mini_project": "Compute NDVI from Sentinel-2 for a small AOI; build basic features.",
          "short_course": "Kaggle – Geospatial Analysis",
          "pfda_3e": ["(Not covered in PfDA; use external resources)"]
        }
      },
      "deliverables": [
        "Domain-specific pipeline additions",
        "Domain data tests integrated into CI"
      ]
    },
    {
      "week": 12,
      "title": "Capstone: End-to-End, Reproducible & Documented",
      "objectives": [
        "Package your pipeline with custom transformers",
        "Document reproducible steps and lock environments",
        "Present metrics comparing baseline vs engineered features"
      ],
      "deliverables": [
        "Packaged src/ with CLI entry point",
        "README with repro steps",
        "Environment lockfile",
        "Model metrics report"
      ],
      "mini_project": "Single-command pipeline from raw → clean → features → model evaluation producing a reports/ bundle.",
      "short_course": "Review prior resources; skim sklearn docs for any gaps",
      "pfda_3e": ["Ch13", "Skim Ch5, Ch7, Ch8, Ch10"]
    }
  ],
  "notes": [
    "Use scikit-learn Pipelines/ColumnTransformer to avoid leakage (fit only on training folds).",
    "For target/mean encoding, implement inside CV folds or use built-in CV encoders.",
    "Add data tests (schema, bounds, null %, uniqueness) before each merge and at pipeline outputs.",
    "Track keys and join match rates; investigate orphans with anti-joins.",
    "Persist artifacts (joblib) and version data if possible (e.g., DVC)."
  ],
  "progress_tracker": [
    {"week": 1, "theme": "Data Familiarity & Baseline Cleaning", "completed": false},
    {"week": 2, "theme": "Missing Values Mastery", "completed": false},
    {"week": 3, "theme": "Outliers & Transformations", "completed": false},
    {"week": 4, "theme": "Categorical Encoding", "completed": false},
    {"week": 5, "theme": "Numerical Feature Creation", "completed": false},
    {"week": 6, "theme": "Date & Text Features", "completed": false},
    {"week": 7, "theme": "Scaling & Pipelines", "completed": false},
    {"week": 8, "theme": "Integration & Reshaping", "completed": false},
    {"week": 9, "theme": "Feature Selection", "completed": false},
    {"week": 10, "theme": "Data Testing & Automation", "completed": false},
    {"week": 11, "theme": "Domain Track (TS/NLP/Geo)", "completed": false},
    {"week": 12, "theme": "Capstone & Docs", "completed": false}
  ]
}
```
