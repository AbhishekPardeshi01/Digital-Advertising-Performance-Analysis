# Digital Advertising Performance Analysis

## 📌 Project Overview

**Digital Advertising Performance Analysis** is a data analytics project focused on evaluating the performance of digital advertising activities using campaign, traffic, lead, conversion, cost, and sales data.

The project analyzes **2,600 advertising records** to understand advertising performance, measure key marketing KPIs, identify keyword-level differences, and generate data-driven insights.

The analysis was performed using **Python, Pandas, NumPy, Matplotlib, Seaborn, and SciPy** in Google Colab.

---

## 🎯 Problem Statement

Digital advertising generates large amounts of performance data, but raw advertising data may contain missing values, inconsistent categorical values, currency-formatted fields, inconsistent date formats, and other data-quality issues.

The objective of this project is to clean and analyze the advertising dataset and evaluate important performance indicators such as:

- Click-through rate (CTR)
- Conversion rate
- Cost per lead
- Cost per conversion
- Return on Ad Spend (ROAS)
- Leads and conversions
- Sales performance
- Keyword-level advertising performance

---

## 🎯 Project Objectives

- Clean and preprocess the advertising dataset.
- Identify and handle missing values.
- Convert currency fields into usable numerical values.
- Validate the conversion-rate information.
- Standardize inconsistent categorical values.
- Investigate and standardize advertising dates.
- Analyze advertising traffic, leads, conversions, cost, and sales.
- Calculate important digital advertising KPIs.
- Compare performance across keywords.
- Analyze relationships between numerical advertising metrics.
- Generate meaningful visualizations and data-driven insights.

---

## 📊 Dataset

The dataset contains **2,600 records and 13 columns**.

### Dataset Features

| Column | Description |
|---|---|
| `Ad_ID` | Unique identifier for an advertisement |
| `Campaign_Name` | Advertising campaign name |
| `Clicks` | Number of clicks received |
| `Impressions` | Number of times an advertisement was displayed |
| `Cost` | Advertising cost |
| `Leads` | Number of generated leads |
| `Conversions` | Number of conversions |
| `Conversion Rate` | Recorded conversion rate |
| `Sale_Amount` | Sales generated |
| `Ad_Date` | Advertisement date |
| `Location` | Advertising location |
| `Device` | Device used by the audience |
| `Keyword` | Keyword associated with the advertisement |

---

## 🧹 Data Cleaning & Preprocessing

Several data-quality issues were identified and addressed during the analysis.

### Missing Values

Missing values were identified in numerical performance fields including:

- `Clicks`
- `Impressions`
- `Cost`
- `Leads`
- `Conversions`
- `Conversion Rate`
- `Sale_Amount`

The missing-value patterns were investigated before performing the analysis.

### Currency Cleaning

The `Cost` and `Sale_Amount` fields originally contained currency-formatted values such as:

```text
$231.88
$216.84
$1,892
```

These values were cleaned and converted into numerical format for analysis.

### Conversion Rate Validation

The recorded `Conversion Rate` was compared with a calculated rate based on:

```text
Conversions / Clicks
```

This helped identify differences between the stored and calculated values and allowed missing conversion-rate values to be evaluated for possible recalculation.

### Date Standardization

The `Ad_Date` field contained inconsistent date formats. Different parsing approaches were tested and the dates were standardized for analysis.

The resulting dates were verified to belong to **November 2024**.

### Categorical Standardization

Inconsistent spellings and capitalization were identified and standardized.

For example, campaign-name variations were standardized to:

```text
Data Analytics Course
```

Location variations were standardized to:

```text
Hyderabad
```

Device values were standardized into:

```text
Desktop
Mobile
Tablet
```

---

## 📈 Key Performance Indicators

The overall advertising performance calculated from the dataset was:

| KPI | Result |
|---|---:|
| Total Impressions | 11,516,270 |
| Total Clicks | 345,725 |
| Total Cost | ₹538,371.80 |
| Total Leads | 51,050 |
| Total Conversions | 16,467 |
| Total Sales | ₹3,688,173 |
| Overall CTR | 3.002% |
| Overall Conversion Rate | 4.763% |
| Cost Per Lead | ₹10.55 |
| Cost Per Conversion | ₹32.69 |
| ROAS | 6.85 |

---

## 🔎 Keyword-Level Analysis

Six different keyword values were analyzed to compare advertising performance.

| Keyword | CTR | Conversion Rate | Cost/Conversion | ROAS |
|---|---:|---:|---:|---:|
| `data analytics course` | 3.019% | 4.726% | ₹32.36 | 6.991 |
| `data anaytics training` | 2.985% | 4.844% | ₹32.20 | 6.905 |
| `learn data analytics` | 3.057% | 4.809% | ₹33.12 | 6.881 |
| `analytics for data` | 2.872% | 4.796% | ₹33.15 | 6.873 |
| `data analitics online` | 3.026% | 4.699% | ₹32.67 | 6.746 |
| `online data analytic` | 3.053% | 4.709% | ₹32.66 | 6.708 |

These values describe the performance observed in this dataset and should not be interpreted as guarantees of future campaign performance.

---

## 📊 Analysis Performed

The project includes analysis of:

- Dataset structure and data types
- Missing-value patterns
- Numerical distributions
- Currency and numerical data cleaning
- Date consistency
- Categorical data standardization
- Data-quality validation
- Advertising KPIs
- Campaign-level data validation
- Keyword-level performance
- CTR
- Conversion Rate
- Cost Per Lead
- Cost Per Conversion
- ROAS
- Correlation between advertising metrics
- Data visualizations

---

## 📉 Visualizations

The project contains visualizations for understanding advertising performance, including:

- Distribution of numerical advertising metrics
- Missing-value analysis
- Keyword performance
- CTR comparison
- Conversion-rate comparison
- Cost-per-conversion comparison
- ROAS comparison
- Correlation matrix / heatmap
- Advertising performance relationships

---

## 🔬 Methodology

The project follows a structured data-analysis workflow:

1. Dataset loading
2. Dataset inspection
3. Data-type analysis
4. Missing-value analysis
5. Numerical data cleaning
6. Currency conversion
7. Conversion-rate validation
8. Date investigation and standardization
9. Categorical-value cleaning
10. Data-quality validation
11. Exploratory Data Analysis
12. KPI calculation
13. Keyword-level analysis
14. Correlation analysis
15. Visualization
16. Interpretation of results
17. Final conclusions

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **SciPy**
- **Google Colab**
- **Jupyter Notebook**
- **Microsoft Excel / CSV**

---

## 📁 Project Structure

```text
Digital-Advertising-Performance-Analysis/
│
├── README.md
├── requirements.txt
├── Digital_Advertising_Performance_Analysis.ipynb
├── Digital_Advertising_Performance_Dataset.csv
└── Project_Report.docx
```

---

## ▶️ How to Run the Project

### 1. Clone or download the repository

Download or clone this GitHub repository.

### 2. Install the required libraries

```bash
pip install -r requirements.txt
```

### 3. Open the notebook

Open:

```text
Digital_Advertising_Performance_Analysis.ipynb
```

The notebook can be opened using Google Colab, Jupyter Notebook, or JupyterLab.

### 4. Keep the dataset in the same directory

The notebook uses:

```text
Digital_Advertising_Performance_Dataset.csv
```

Make sure the CSV file is available when running the notebook.

### 5. Run the notebook sequentially

Execute the cells from beginning to end to reproduce the analysis.

---

## 📌 Key Findings

- The dataset contains **2,600 advertising records**.
- The advertising activity generated **11.52 million impressions** and **345,725 clicks**.
- A total of **51,050 leads** and **16,467 conversions** were recorded.
- Total recorded sales were approximately **₹3.69 million**.
- The overall CTR was approximately **3.00%**.
- The overall conversion rate based on total conversions and clicks was approximately **4.76%**.
- The overall cost per lead was approximately **₹10.55**.
- The overall cost per conversion was approximately **₹32.69**.
- The calculated overall ROAS was approximately **6.85**.
- Keyword performance showed differences in CTR, conversion rate, cost per conversion, and ROAS.
- The analysis also identified data-quality issues that required cleaning before reliable KPI analysis could be performed.

---

## 🚀 Future Scope

The project can be extended through:

- **Predictive models** for conversion and sales prediction.
- Machine-learning models for identifying factors associated with advertising performance.
- Prediction of future campaign KPIs.
- Keyword performance prediction.
- Customer or audience segmentation.
- Automated campaign-performance monitoring.
- Interactive dashboards using Power BI, Tableau, or Streamlit.
- Time-series analysis using larger multi-period advertising datasets.
- Automated anomaly and data-quality detection.
- Integration with real-time advertising platforms for continuous performance monitoring.

---

## ⚠️ Limitations

- The analysis is based on the available **2,600-record dataset**.
- The dataset covers advertising activity within the available time period rather than a long-term historical period.
- The results describe relationships and patterns in the available data and do not establish causation.
- Future campaign performance may differ from the patterns observed in this dataset.

---

## 📄 Project Report

A detailed project report is included in:

```text
Project_Report.docx
```

The report provides detailed information about the problem statement, objectives, dataset, methodology, data cleaning, analysis, findings, and conclusions.

---

## 📌 Conclusion

The **Digital Advertising Performance Analysis** project demonstrates how raw advertising data can be transformed into meaningful business insights through systematic data cleaning, exploratory analysis, KPI calculation, visualization, and statistical analysis.

The project provides an overview of advertising traffic, leads, conversions, costs, sales, and keyword-level performance while also demonstrating the importance of data-quality validation before drawing analytical conclusions.

---

## 👤 Project Information

**Project Title:** Digital Advertising Performance Analysis  
**Domain:** Data Analytics / Digital Marketing  
**Dataset Size:** 2,600 records × 13 columns  
**Environment:** Google Colab / Jupyter Notebook  
**Language:** Python
