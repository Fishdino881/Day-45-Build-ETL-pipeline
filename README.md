# Day-45-Build-ETL-pipeline

### 🔍 Overview

On Day 45, I implemented a **basic ETL pipeline using Python**, applying the concepts learned earlier.
The goal was to **extract data**, **clean & transform it**, and **load it into a target destination** in a structured format.

This is a foundational step toward **data engineering, analytics, and ML pipelines**.

---

##  ETL Pipeline Stages

### 1️ Extract

Data is extracted from a source file (CSV).

```python
import pandas as pd

data = pd.read_csv("raw_data.csv")
```

---

### 2️ Transform

Data cleaning and transformation steps:

* Handling missing values
* Removing duplicates
* Renaming columns
* Changing data types

```python
data.dropna(inplace=True)
data.drop_duplicates(inplace=True)
data.columns = data.columns.str.lower()
```

---

### 3️ Load

The transformed data is stored in a new file (or database).

```python
data.to_csv("clean_data.csv", index=False)
```



##  Tools & Technologies

* Python
* Pandas
* CSV files

---

##  Key Learnings

* Practical understanding of ETL workflows
* Importance of data quality before analysis
* How Python connects extraction, transformation, and loading
* Foundation for automated and scalable pipelines

---

##  Use Cases

* Data analysis preparation
* Machine learning pipelines
* Business intelligence reporting
* Backend data processing

