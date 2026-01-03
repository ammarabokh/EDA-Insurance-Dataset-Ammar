# Exploratory Data Analysis (EDA) – Insurance Dataset

## 📌 Overview
This project performs **Exploratory Data Analysis (EDA)** on an insurance dataset. The goal is to understand the structure of the data, identify data quality issues (missing values, incorrect data types, outliers), and explore relationships between variables using statistical analysis and visualization.

The notebook walks through a complete EDA workflow that is commonly used in real-world data science projects.

---

## 📂 Dataset
- **Source:** Kaggle – Playground Series S4E12 (Insurance dataset)
- **File used:** `train.csv`
- **Type:** Tabular data (numerical + categorical + date columns)

---

## 🛠 Libraries Used
The following Python libraries are used throughout the notebook:
- `pandas` – data manipulation and analysis
- `numpy` – numerical computations
- `matplotlib` & `seaborn` – data visualization
- `warnings` – suppress unnecessary warnings

---

## 🔍 Notebook Structure & Explanation

### Step 1: Reading the Data
- The dataset is loaded into a Pandas DataFrame.
- Initial inspection using:
  - `df.head()` / `df.tail()`
  - `df.info()`
  - `df.shape`

**Purpose:** Understand the size of the dataset, column names, and data types.

---

### Step 2: Identifying Data Problems

#### 1️⃣ Dropping Unnecessary Columns
- The `id` column is removed because it does not add analytical value.

**Reason:** Identifiers do not contribute to statistical analysis or modeling.

---

#### 2️⃣ Converting Date Columns
- Date and time columns are converted to `datetime64` format.

**Reason:**
- Enables time-based analysis
- Prevents errors in calculations and visualizations

---

### Step 3: Missing Values Analysis
- Percentage of missing values is calculated for each column.
- Missing values are analyzed to decide whether to:
  - Drop rows
  - Drop columns
  - Impute values (mean, median, mode)

**Goal:** Improve data quality without losing important information.

---

### Step 4: Exploratory Data Analysis (EDA)

#### 📊 Univariate Analysis
- Distribution of numerical variables
- Count plots for categorical variables

**Techniques used:**
- Histograms
- Boxplots
- Value counts

---

#### 📈 Bivariate & Multivariate Analysis
- Relationship between variables
- Correlation analysis

**Techniques used:**
- Scatter plots
- Heatmaps
- Group-by analysis

---

### Step 5: Outlier Detection
- Outliers are detected using:
  - Boxplots
  - IQR (Interquartile Range)

**Important Note:**
Outliers are analyzed carefully and not removed automatically. The context of the data is considered before taking any decision.

---

### Step 6: Visualization
- Clear and informative visualizations are created using:
  - `seaborn`
  - `matplotlib`

**Purpose:**
- Identify trends
- Detect anomalies
- Support data-driven decisions

---

## 📌 Key Insights
- Data contains both numerical and categorical features
- Some columns require cleaning and type conversion
- Presence of outliers that need contextual interpretation
- Visualization plays a critical role in understanding the data

---

## 🚀 How to Run the Notebook
1. Clone or download the repository
2. Install required libraries:
```bash
pip install pandas numpy matplotlib seaborn
```
3. Open the notebook:
```bash
jupyter notebook
```
4. Run all cells sequentially

---

## 🧠 Conclusion
This notebook demonstrates a **complete EDA pipeline**, from raw data loading to insights extraction. It follows best practices used in professional data analysis projects and can serve as a strong foundation for further modeling or machine learning tasks.

---

## ✍️ Author
Prepared and analyzed by **Ammar**

---

✅ *This README is designed to clearly explain the notebook for recruiters, teammates, and reviewers.*

