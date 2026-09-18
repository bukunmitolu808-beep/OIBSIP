# OIBSIP
Data analysis projects: cleaning, Excel, Tableau, reporting.
# Retail Sales Data Analysis

This repository contains my data analysis project on a retail sales dataset. The project explores sales performance, customer demographics, product categories, and purchasing trends using Python and Google Colab.

## Project Objective

The aim of this project is to clean, explore, and analyse retail sales data in order to identify useful business insights and support decision-making.

## Dataset

The dataset contains 1,000 retail transaction records and 9 columns:

- Transaction ID
- Date
- Customer ID
- Gender
- Age
- Product Category
- Quantity
- Price per Unit
- Total Amount

## Tools Used

- Python
- Google Colab
- Pandas
- Matplotlib
- Seaborn
- Microsoft Excel

## Data Cleaning

The following checks and cleaning activities were completed:

- Checked the dataset shape, column names, and data types
- Checked for missing values
- Checked for duplicate records
- Converted the Date column to datetime format
- Checked values in Gender and Product Category for consistency
- Validated that Total Amount equals Quantity multiplied by Price per Unit
- Exported a final cleaned dataset

## Exploratory Data Analysis

The analysis includes visualisations and insights on:

- Total sales by product category
- Average transaction value by product category
- Sales by gender
- Customer age-group distribution
- Monthly sales trends
- Number of transactions by age group

## Key Insights

- Electronics generated the highest total sales.
- Beauty had the highest average transaction value.
- Female customers generated slightly more total revenue than male customers.
- Customers aged 45–54 made the highest number of transactions.
- The dataset contained 1,000 records with no missing values and no duplicate rows.
- Total Amount was successfully validated against Quantity and Price per Unit.

## Files in This Repository

- `Retail Sales EDA Project.ipynb` – Google Colab notebook containing the cleaning process, analysis, charts, and findings
- `cleaned_retail_sales_final.csv` – Final cleaned retail sales dataset
- `README.md` – Project documentation

## How to Run the Project

1. Download or clone this repository.
2. Open the `.ipynb` file in Google Colab or Jupyter Notebook.
3. Upload the dataset if required.
4. Run the notebook cells in order to reproduce the analysis and visualisations.

## Author

**Bukunmi Tolu**

Aspiring Data Analyst with interests in data cleaning, Excel, Python, visualisation, and business insights.
