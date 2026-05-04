# 📊 Sales Data Analysis (Excel Project)

This project focuses on cleaning and analyzing a retail store’s daily sales data using Microsoft Excel. The goal is to handle missing values, manage outliers, and identify a reliable metric to represent typical sales performance.

---

## 📁 Dataset Overview

The dataset contains the following columns:

- **Date** – Transaction date  
- **Product** – Item sold  
- **Sales_Amount** – Sales value (in ₹)  
- **Region** – Location of sale  

---

## 🔍 Problem Context

During the initial analysis, the following issues were identified:

- Some rows had **missing Sales_Amount values**
- A few entries had **extremely high values (outliers)** compared to others
- The business required a **single metric to represent typical daily sales** specifically for the **South region**

---

## 🎯 Objectives

- Clean the dataset by handling missing values  
- Identify a reliable statistical measure for “typical” sales  
- Minimize the impact of extreme values without removing data  
- Perform region-specific analysis (South only)  

---

## 📈 Approach & Solution

### 1. Handling Missing Values
- Blank `Sales_Amount` values were identified and excluded from calculations  
- Ensured only valid numeric data is considered during analysis  

---

### 2. Choosing the Right Metric

- **Median** was selected as the best measure of typical sales  
- Reason:
  - Not affected by extreme values (outliers)  
  - Gives a more realistic central value  
  - Mode was not useful since most values are unique  

---

### 3. Handling Outliers When Average is Required

Although median is more reliable, management preferred using **average** as the summary metric.  

To address this, the **TRIMMEAN function** was used. This approach:
- Removes extreme high and low values automatically  
- Reduces the impact of outliers  
- Keeps the dataset intact without deleting any rows  

This provides a more balanced and realistic average for decision-making.

---

## 📊 Key Learnings

- Median is more reliable than mean when outliers exist  
- TRIMMEAN helps improve average calculations in skewed data  
- Data cleaning is essential before analysis  
- Excel functions can effectively solve real-world data problems  

---

## 📌 Conclusion

This project demonstrates how Excel can be used to:
- Clean and prepare data  
- Handle missing values  
- Reduce the impact of outliers  
- Generate meaningful insights for business decisions  

---

## 📂 Files Included

- `sales-analysis.xlsx` – Cleaned dataset and analysis  
