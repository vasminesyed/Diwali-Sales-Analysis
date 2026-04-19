# Diwali Sales Analysis

Python-based exploratory data analysis on Diwali festival sales data to find who is buying, what they are buying, and which states drive the most sales.

## What this project does

Analyzed Diwali sales data to find patterns in customer demographics and product performance. The goal was to understand which customer segments are buying more during Diwali and which product categories perform best. These insights can help businesses plan their inventory and target their marketing better before the next festive season.

## Dataset

- Source: Kaggle Diwali Sales dataset
- Records: 11,000+ rows
- Columns: User ID, customer name, product ID, gender, age group, marital status, state, occupation, product category, orders, amount

## Steps followed

**1. Data Loading**
- Loaded CSV file using Pandas
- Checked shape, data types, null values

**2. Data Cleaning**
- Dropped blank/null columns (Status, unnamed column)
- Removed rows with missing Amount values
- Changed data type of Amount column to integer

**3. Exploratory Data Analysis (EDA)**

Analysis was done across 6 dimensions:

- **Gender** - Compared number of orders and total sales amount for Male vs Female
- **Age Group** - Checked which age group buys the most
- **State** - Found top 10 states by orders and by revenue
- **Marital Status** - Compared buying behavior of married vs unmarried customers
- **Occupation** - Checked which job types spend the most during Diwali
- **Product Category** - Found top selling categories by number of orders

## Key findings

**Gender**
- Women place more orders than men
- Women also spend more money overall - higher purchasing power

**Age Group**
- 26-35 age group has the highest number of orders and revenue
- Mostly female customers in this group

**Top States**
- Uttar Pradesh, Maharashtra, and Karnataka are the top 3 states by both orders and revenue

**Marital Status**
- Married women are the biggest buyers during Diwali

**Occupation**
- Customers working in IT, Healthcare, and Aviation sectors spend the most

**Product Categories**
- Food, Clothing, and Electronics are the top 3 categories
- These three categories make up majority of total festive sales

## Libraries used

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

## How to run

```bash
# Clone the repo
git clone https://github.com/vasminesyed/Diwali-Sales-Analysis.git

# Install required libraries
pip install pandas numpy matplotlib seaborn

# Open the notebook
jupyter notebook Diwali_Sales_Analysis.ipynb
```

## File structure

```
Diwali-Sales-Analysis/
│
├── Diwali_Sales_Analysis.ipynb    # Full analysis notebook
├── README.md                      # Project documentation
```
