# Pandas Learning Repository

A structured, practical path to mastering Pandas for data analysis, data engineering, and ML preprocessing.

---

## 0. Prerequisites

### Install Python

* Python >= 3.9 recommended

Verify:

```bash
python3 --version
```

### Install pip3

```bash
python3 -m ensurepip --upgrade
pip3 --version
```

### Install Pandas

```bash
pip3 install pandas
```

Verify installation:

```bash
pip3 show pandas
```

Homepage: [https://pandas.pydata.org](https://pandas.pydata.org)

---

## 1. Project Setup

Create workspace:

```bash
mkdir pandas-learn
cd pandas-learn
python -m venv venv
```

Activate venv:

**Linux / Mac**

```bash
source venv/bin/activate
```

**Windows**

```bash
venv\Scripts\activate
```

Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

Run notebook:

```bash
jupyter notebook
```

---

## 2. Learning Roadmap

### Stage 1 — Foundations

Topics:

* Series
* DataFrame
* Index
* dtypes
* Importing data (CSV, JSON)

Notebook: `01_basics.ipynb`

Exercises:

1. Create Series from list, dict, scalar
2. Create DataFrame manually
3. Load CSV and inspect columns
4. Change column data types

---

### Stage 2 — Selection & Filtering

Topics:

* loc vs iloc
* Boolean filtering
* Query API
* Sorting

Notebook: `02_selection_filtering.ipynb`

Exercises:

1. Filter rows by condition
2. Select specific columns
3. Multi-condition filters
4. Top N values by column

---

### Stage 3 — Data Cleaning

Topics:

* Missing values
* fillna / dropna
* duplicates
* string operations
* type conversion

Notebook: `03_cleaning.ipynb`

Exercises:

1. Detect missing values
2. Replace missing with mean/median
3. Remove duplicates
4. Clean messy text column

---

### Stage 4 — Transformations

Topics:

* apply / map / transform
* lambda functions
* column creation
* binning

Notebook: `04_transformations.ipynb`

Exercises:

1. Create new derived columns
2. Categorize ages into groups
3. Normalize numeric columns

---

### Stage 5 — Grouping & Aggregation

Topics:

* groupby
* aggregation
* multi-index
* pivot tables

Notebook: `05_groupby.ipynb`

Exercises:

1. Average salary by department
2. Count per category
3. Multi-column grouping
4. Pivot summary report

---

### Stage 6 — Merging & Joining

Topics:

* concat
* merge
* join
* key relationships

Notebook: `06_merge_join.ipynb`

Exercises:

1. Inner join
2. Left join
3. Combine monthly datasets
4. Detect unmatched rows

---

### Stage 7 — Time Series

Topics:

* datetime index
* resampling
* rolling windows

Notebook: `07_timeseries.ipynb`

Exercises:

1. Convert string to datetime
2. Daily → monthly aggregation
3. Moving average

---

### Stage 8 — Performance & Optimization

Topics:

* vectorization
* categorical dtype
* memory optimization
* avoiding loops

Notebook: `08_performance.ipynb`

Exercises:

1. Compare loop vs vectorized
2. Reduce memory usage
3. Speed up large dataset operations

---

### Stage 9 — Visualization

Topics:

* matplotlib integration
* seaborn plots

Notebook: `09_visualization.ipynb`

Exercises:

1. Line plot
2. Bar chart
3. Heatmap correlation

---

## 3. Real Projects

### Project 1 — Sales Analytics

Tasks:

* Clean dataset
* Monthly revenue trends
* Top customers
* Category performance

### Project 2 — User Behavior Analysis

Tasks:

* Session duration distribution
* Retention cohorts
* Active users per day

### Project 3 — Data Pipeline Simulation

Tasks:

* Load raw logs
* Clean and normalize
* Aggregate metrics
* Export report CSV

---

## 4. Repository Structure

```
pandas-learn/
│
├── data/
├── notebooks/
│   ├── 01_basics.ipynb
│   ├── 02_selection_filtering.ipynb
│   ├── 03_cleaning.ipynb
│   ├── 04_transformations.ipynb
│   ├── 05_groupby.ipynb
│   ├── 06_merge_join.ipynb
│   ├── 07_timeseries.ipynb
│   ├── 08_performance.ipynb
│   └── 09_visualization.ipynb
│
├── projects/
├── requirements.txt
└── README.md
```

---

## 5. requirements.txt

```
pandas
numpy
matplotlib
seaborn
jupyter
```

---

## Goal

By completing this repository, you should be able to:

* Clean real-world datasets
* Build data analysis workflows
* Prepare ML-ready datasets
* Optimize dataframe operations
* Design repeatable data pipelines
