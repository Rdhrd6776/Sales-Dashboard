# Sales-Dashboard

Sales Data Analytics Project | Excel + Python + SQL + Power BI


This report outlines the professional blueprint for transitioning from basic Excel operations to a comprehensive data analytics pipeline using Python, SQL, and Power BI. This project demonstrates a complete ETL (Extract, Transform, Load) process designed for scalability and accuracy

--------------------------------------------------------------------------------
1. Skills and Technologies Used
The project integrates four distinct professional roles into a single workflow
Excel (Operations/Sales): Used as the initial source for raw, messy data entry
Python (Data Analysis): Utilized for automated data cleaning, transformation, and logic building
MySQL (Data Engineering): Employed for secure, centralized data warehousing and permanent connections
Power BI (Business Intelligence): Used for creating visual trends, identifying regional performance, and generating actionable business insights

--------------------------------------------------------------------------------
2. Data Cleaning and Transformation Process
The raw Excel data contained several issues, including messy formatting, duplicate entries, and missing values
. The cleaning was performed in Python (Jupyter Notebook) for better speed and accuracy with large datasets
Initial Loading: The raw file (520 rows) was imported into Python using the pandas library
Deduplication: The first cleaning step involved identifying and removing 20 duplicate rows, reducing the dataset to 500 rows
Handling Missing Values:
Blank entries were identified in the Order Date column
Rather than filling them with "0" or "NA" (which would break the date data type), these rows were dropped using the subset function to ensure data integrity
The final cleaned data consisted of 482 rows
Feature Engineering: Three new columns were generated to enhance analysis:
Profit: Calculated by subtracting Cost from Sales
Year: Extracted from the Order Date
Month: Extracted from the Order Date
Database Loading: The cleaned data was pushed from Python to a MySQL database via an SQLAlchemy engine, creating a permanent data warehouse

--------------------------------------------------------------------------------
3. Findings and Business Insights
The final analysis, visualized in the Power BI dashboard, revealed several key performance indicators (KPIs) and trends
Overall Performance:
Total Sales: 20M
Total Profit: 5M
Profit Margin: The dashboard records a "Sum of Profit % on sales" of 12.10K
Sales Trends: A line chart of "Sales by Month" shows significant fluctuations, with a notable peak in the early part of the year (around March) followed by a dip in April

Regional Insights:
The North region is the highest contributor to profit, followed by the South region
The West region shows the lowest profit performance
Product Performance:
Printers are the top-selling product
Profit distribution is relatively balanced across categories, with Tablets (23.31%) and Laptops (20.31%) leading the profit share

--------------------------------------------------------------------------------
4. Strategic Advantages of this Pipeline
Connection Stability: Unlike Excel-to-Power BI connections, which are temporary and break if file locations change, the SQL connection is permanent and scalable
Automation: By using Python for ETL, the manual work of applying Excel formulas is replaced by an automated script that handles large data sets much faster
Decision Making: The transition from raw data to visual insights allows management to make faster decisions based on regional and product-specific trends

Dashboard image: - !(https://github.com/Rdhrd6776/Sales-Dashboard/blob/main/Sale_Dashboard.png)
