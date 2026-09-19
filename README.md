# OIBSIP Data Analytics Projects

This repository contains my data analytics projects completed as part of my OASIS Infobyte internship. The projects demonstrate my skills in data cleaning, exploratory data analysis, customer segmentation, visualisation, and communicating business insights.

## Tools Used

- Python
- Google Colab
- Pandas
- Matplotlib
- Seaborn
- Microsoft Excel

---

# Project 1: Retail Sales Data Analysis

## Objective

To clean, explore, and analyse a retail sales dataset in order to identify sales trends, customer behaviour, and product performance.

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

## Data Cleaning

The following data-quality checks were completed:

- Checked the dataset shape, column names, and data types
- Checked for missing values and duplicate records
- Converted the Date column to datetime format
- Checked Gender and Product Category values for consistency
- Validated that Total Amount equals Quantity multiplied by Price per Unit
- Exported a final cleaned dataset

## Analysis Performed

- Total sales by product category
- Monthly sales trend
- Sales by gender
- Customer age-group distribution
- Average transaction value by product category
- Number of transactions by age group

## Key Insights

- Electronics generated the highest total sales.
- Beauty had the highest average transaction value.
- Female customers generated slightly more total revenue than male customers.
- Customers aged 45–54 made the highest number of transactions.
- The dataset had no missing values or duplicate rows.
- Total Amount was successfully validated for all records.

## Files

- `Retail Sales EDA Project.ipynb` — Notebook containing cleaning, analysis, charts, findings, and recommendations
- `cleaned_retail_sales_final.csv` — Final cleaned retail sales dataset

---

# Project 2: Customer Segmentation Analysis

## Objective

To group customers into meaningful value segments based on their total spending and identify actions that can help improve customer value and retention.

## Dataset

This project uses the cleaned retail sales dataset containing 1,000 transaction records. Each Customer ID appears once in the dataset, so each row represents one customer's purchase behaviour.

## Methodology

Customer-level features were created using:

- Total amount spent
- Number of transactions
- Average transaction value
- Customer age
- Gender
- Total quantity purchased
- Most frequently purchased product category

Customers were assigned to three groups using the 33rd and 67th percentiles of total spending:

- Low-Value Customers
- Medium-Value Customers
- High-Value Customers

## Segmentation Results

| Customer segment | Number of customers | Average total spend | Average age |
|---|---:|---:|---:|
| Low-Value | 349 | 52.84 | 41.03 |
| Medium-Value | 352 | 210.11 | 42.66 |
| High-Value | 299 | 1,216.05 | 40.32 |

The customer distribution was relatively balanced across the three value segments. High-Value customers had the largest average spend, while age differences across the groups were small.

## Key Insights

- High-Value customers had the highest average spend, about 1,216.05 per customer.
- Medium-Value customers were the largest segment, with 352 customers and an average total spend of 210.11.
- Low-Value customers had the lowest average spend, about 52.84 per customer.
- Each customer made one transaction in this dataset; therefore, segment differences are driven mainly by purchase value rather than purchase frequency.
- Gender distribution was similar across all segments, so spend-based targeting is more useful than gender-based targeting.

## Recommendations

- Offer loyalty rewards, premium product bundles, and early access to High-Value customers.
- Use cross-selling and upselling campaigns to move Medium-Value customers into the High-Value segment.
- Encourage larger purchases among Low-Value customers through bundle offers, discounts, and minimum-spend promotions.
- Focus customer campaigns on spending behaviour and product preferences rather than gender alone.

## Files

- `Customer Segmentation Project.ipynb` — Notebook containing customer-level analysis, segmentation, chart, insights, and recommendations
- `customer_segments.csv` — Dataset containing customer features and assigned value segments

---

# Project 3: Data Cleaning Project (Level 1, Task 3)

## Objective

To clean a messy employee dataset by identifying and fixing data-quality issues such as missing values, incorrect data types, and invalid entries, and to document the cleaning process and results.

## Dataset

The dataset contains 1,020 employee records and 12 columns:

- Employee_ID
- First_Name
- Last_Name
- Age
- Department_Region
- Status
- Join_Date
- Salary
- Email
- Phone
- Performance_Score
- Remote_Work

## Data-Quality Issues Identified

- Missing values in `Age` (211) and `Salary` (24)
- `Join_Date` stored as text instead of datetime
- `Phone` column contained invalid negative integers
- Categorical columns (`Status`, `Performance_Score`, `Department_Region`) needed standardisation

## Data-Cleaning Process

1. **Converted Join_Date to datetime**  
   - Ensured dates are in a proper datetime format for analysis.

2. **Handled missing Age**  
   - Filled missing `Age` values with the median age.  
   - Converted `Age` from float to integer.

3. **Handled missing Salary**  
   - Filled missing `Salary` values with the median salary.

4. **Fixed invalid Phone column**  
   - Recognised that all phone values were invalid.  
   - Set the entire `Phone` column to missing (`<NA>`) to indicate unusable data.

5. **Standardised categorical columns**  
   - Cleaned and standardised `Status`, `Performance_Score`, and `Department_Region` to title case and removed extra spaces.

## Data Quality Report

**Before cleaning:**
- Shape: 1,020 rows × 12 columns
- Missing values: Age (211), Salary (24)
- Join_Date stored as text (object)
- Phone column contained invalid negative integers
- Duplicate rows: 0

**After cleaning:**
- Shape: 1,020 rows × 12 columns
- No missing values in Age, Salary, or Join_Date
- Phone column intentionally set to all missing due to invalid original data
- All categorical columns consistent and ready for analysis
- Duplicate rows: 0

## Files

- `Data_Cleaning_Project.ipynb` — Notebook documenting the full cleaning process and data-quality report
- `cleaned_employee_data.csv` — Final cleaned employee dataset

---

## Author

**Bukunmi Tolu**

Aspiring Data Analyst with interests in Python, Excel, data cleaning, data visualisation, customer analytics, and business insights.
