# Superstore Python Project

## Project Overview

This project analyzes the Superstore dataset using Python (pandas & matplotlib) to evaluate business performance, profitability, customer and product insights.

The goal of this project was to demonstrate:
- Knowledge of Python, including Pandas library
- Data aggregation and transformation
- Time analysis
- Data visualization with matplotlib
- Use of reusable functions
- Basic loop-based reporting
- Clear business interpretation of results

## Data Source

The analysis is based on three CSV files exported from a Superstore SQL project:  
https://github.com/kathkam/superstore-sql-project.git  

Exported files:
- fact_sales.csv  
- dim_customer.csv  
- dim_product.csv  

These files are merged in Python to create one analytical dataset.

## Project Structure
/data  
fact_sales.csv  
dim_customer.csv  
dim_product.csv  

/notebooks  
01_data_loading.ipynb  
02_data_preparation.ipynb  
03_data_analysis.ipynb  

README.md  

## Technologies Used
Python 3+  
pandas  
matplotlib  
Jupyter Notebook  

## Analysis Performed
### 1. Data Preparation
Loaded and merged fact and dimension tables  
Converted date columns to datetime  
Verified row counts and data integrity  

### 2. Overall KPIs
Calculated key performance indicators:  
Total Sales  
Total Profit  
Profit Margin  
Number of Orders  
Number of Customers  
Average Order Value  

### 3. Category Analysis
Sales by Category  
Profit by Category  
Profit Margin by Category  

Key findings:  
- Technology is the strongest performing category.  
- Furniture shows significantly lower profitability due to low-margin sub-categories.  

### 4. Sub-Category Analysis  
Top 5 most profitable sub-categories  
Bottom 5 least profitable sub-categories  
Visualization of top 10 sub-categories by profit  

Key findings:  
- Copiers and Phones have a high profitability.  
- Tables generate significant losses.

### 5. Time-Based Performance Trends  
Analyzed yearly trends for:  
Sales  
Profit  
Profit Margin  

Key findings:  
- Profit consistently increased from 2014 to 2017.  
- Margin improved significantly from 2014 to 2016.  
- Slight margin decline in 2017 suggests possible pricing or cost issues.  

### 6. Reusable Functions & Loop-Based Reporting
Implemented reusable functions:  
- grouped_calc() – helper in aggregation  
- column_summary() – KPI summary for a chosen column  

Used loop-based ranking reports to automatically generate:  
- Top & Bottom Customers by Sales, Profit, and Margin  
- Top & Bottom Products by Sales, Profit, and Margin  

## Key Findings
Revenue growth is driven mainly by Technology products.  
Furniture is not showing significant profitability due to low-margin sub-categories (especially Tables).  
Profitability improved over time due to increased revenue and efficiency.  
Customer and product analysis highlights most and least profitable contributors.  

## How to Run the Project
### Requirements  
Python 3+  
pip  
Jupyter Notebook  

Python packages used:  
- pandas
- matplotlib

### 1. Clone the repository:

In the terminal / PowerShell:
```
git clone https://github.com/kathkam/superstore-python-project.git
cd superstore-python-project
```

### 2. Create a virtual environment:
```
python -m venv .venv
.\.venv\Scripts\activate
```  
  
You should now see (.venv) in the terminal  

### 4. Install dependencies:  
```
pip install pandas matplotlib jupyter
```

### 5. Open the notebook:  
```
jupyter notebook
```

### 6. Open the analysis notebook  

Run 03_data_analysis.ipynb  

## Project Purpose
This project was built to showcase Python-based data analysis skills for Data Analyst roles, with emphasis on:
- Data transformation
- Aggregation logic
- Analytical thinking
- Visualization
- Code structure and reusability
