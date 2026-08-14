  # Exploratory Data Analysis - Superstore Dataset

## Project Overview

This project focuses on performing Exploratory Data Analysis (EDA) on a cleaned Superstore dataset.

The purpose of this analysis is to identify important patterns, relationships, trends, and potential outliers in the dataset using statistical analysis and data visualization.

---

## Objective

The main objective of this project is to build the habit of questioning data visually and statistically before drawing conclusions.

The analysis focuses on:

- Understanding numerical variables
- Studying data distributions
- Identifying potential outliers
- Understanding relationships between numerical variables
- Comparing Sales across product categories
- Comparing Profit across regions
- Investigating the relationship between Discount and Profit
- Summarizing the most important findings

---

## Dataset

The analysis uses the cleaned Superstore dataset.

### Dataset Summary

- **Rows:** 9,977
- **Columns:** 13
- **Missing values:** 0
- **Duplicate rows:** 0

### Main Columns

- Ship Mode
- Segment
- Country
- City
- State
- Postal Code
- Region
- Category
- Sub-Category
- Sales
- Quantity
- Discount
- Profit

---

## Tools Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab

---

## EDA Approach

### 1. Data Inspection

I first inspected the dataset to understand its structure, columns, data types, and number of records.

### 2. Summary Statistics

I used `df.describe()` to understand the numerical variables using:

- Count
- Mean
- Standard deviation
- Minimum
- Maximum
- Quartiles

### 3. Correlation Analysis

I calculated correlations between Sales, Quantity, Discount, and Profit.

A correlation heatmap was created to understand these relationships visually.

### 4. Sales Distribution

A histogram was used to understand how Sales values are distributed across transactions.

The analysis showed that most transactions are concentrated at lower Sales values, while a smaller number of transactions have very high Sales values.

### 5. Profit Distribution

A histogram was used to understand the distribution of Profit.

The analysis showed that most Profit values are concentrated around zero, with both positive and negative values present.

### 6. Outlier Analysis

Boxplots were used to identify potential extreme values in Sales and Profit.

These extreme values were treated as observations requiring investigation rather than automatically being considered data errors.

### 7. Sales by Category

Total Sales were compared across product categories to identify which category contributes the most to overall Sales.

Technology generated the highest total Sales among the three categories.

### 8. Profit by Region

Total Profit was compared across regions to understand regional profitability.

The West region generated the highest total Profit among the four regions.

### 9. Discount vs Profit

A scatter plot and correlation analysis were used to investigate the relationship between Discount and Profit.

The correlation between Discount and Profit was approximately **-0.22**, indicating a weak negative relationship.

---

## Key Findings

### Sales Distribution

Most transactions have relatively low Sales values, while a smaller number of transactions have very high Sales values. The Sales distribution is therefore right-skewed.

The mean Sales value is approximately **230.15**, while the median is approximately **54.82**.

### Category Performance

Technology generated the highest total Sales among the three product categories, followed by Furniture and Office Supplies.

### Regional Profitability

The West region generated the highest total Profit among the four regions.

### Discount and Profit

Discount and Profit have a weak negative correlation of approximately **-0.22**.

This suggests that higher discounts tend to be associated with lower Profit to some extent. However, correlation does not prove causation.

### Outliers

The analysis identified extreme Sales and Profit values. These were not automatically removed because an outlier can represent a genuine business transaction rather than a data-entry error.

---

## Top 3 Insights

1. **Sales are highly concentrated at lower values**, while a small number of high-value transactions increase the overall average.

2. **Technology has the highest total Sales**, making it an important contributor to overall sales performance.

3. **Discount has a weak negative relationship with Profit**, suggesting that higher discounts are associated with lower profitability to some extent.

---

## Time-Series Analysis Limitation

I checked the available columns before performing time-based analysis.

The cleaned dataset does not contain a date column. Therefore, a genuine time-series analysis could not be performed without creating or assuming dates that are not present in the dataset.

Instead, I continued the EDA using the available numerical and categorical variables.

---

## Final Outcome

This exploratory analysis helped identify important distributions, relationships, category-level sales patterns, regional profit patterns, and potential outliers in the Superstore dataset.

The analysis demonstrates how statistical summaries and visualizations can be used together to understand data and identify meaningful findings before drawing conclusions.

---

## Project Files

- `Superstore_EDA_Day_2.ipynb` — Complete EDA notebook
- `cleaned_superstore.csv` — Cleaned Superstore dataset
- `README.md` — Project documentation
