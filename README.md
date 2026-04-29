Customer Shopping Behavior Analysis

Overview 
This project provides a comprehensive end-to-end analysis of customer purchasing patterns to drive data-informed business decisions. By leveraging Python for data cleaning, PostgreSQL for advanced querying, and Power BI for interactive visualization, the project identifies key revenue drivers, customer segments, and product performance metrics.DatasetThe analysis is based on the customer_shopping_behavior.csv dataset. It contains 3,900 records detailing customer demographics (age, gender), transaction details (purchase amount, category, item), and behavioral attributes (subscription status, shipping preferences, and review ratings).

Tools
VS Code: Primary IDE for Python development.Python (Pandas, SQLAlchemy): Used for Exploratory Data Analysis (EDA), data cleaning, and ETL processes.  PostgreSQL: Hosted the cleaned data for complex relational querying and segmentation. 
Power BI: Created an interactive dashboard to visualize KPIs and customer trends. 

1. Data Cleaning (Python):
Handled missing values in review_rating by imputing the median based on product category.  
Standardized column names (lowercase with underscores) for database compatibility.  
Engineered new features including age_group (binned using qcut) and purchase_frequency_days.

2. Database Integration:
Established a connection between Python and PostgreSQL using SQLAlchemy.  
Automated the data load into a customer table within the customer_behavior database

3.Advanced SQL Querying:
Performed multi-level analysis including revenue contribution by gender, customer segmentation (New vs. Loyal), and product ranking within categories.

4.Data Visualization:
Connected Power BI to the processed data to build a dashboard focusing on sales distribution and demographic behavior.

Dashboard
The interactive Power BI dashboard provides a high-level view of:
Key Performance Indicators (KPIs): Total customers (3.9K), average purchase amount ($59.76), and average review rating (3.75).  
Demographic Insights: Sales and revenue distribution across different age groups (Young Adult, Adult, Middle Aged, Senior).  
Category Analysis: Breakdown of revenue and order volume by product categories like Clothing and Accessories.  
Subscription Trends: Visual comparison showing that 27% of the customer base are subscribers

Results
Customer Segmentation: Successfully categorized the user base into 'New', 'Returning', and 'Loyal' segments based on historical purchase counts.  
Revenue Drivers: Identified the top-performing product categories and determined the revenue contribution of various age demographics.  
Shipping & Spend: Compared average purchase amounts across different shipping types to understand service-level impact on spending.  
Subscription Value: Analyzed whether subscribed customers exhibit higher average spends and total revenue compared to non-subscribers.

How to Run
Python Environment: Install dependencies using pip install pandas sqlalchemy psycopg[binary].
Database Setup: Ensure PostgreSQL is running and create a database named customer_behavior.
Data Loading: Run the Jupyter Notebook/Python script to clean the customer_shopping_behavior.csv and export it to SQL.  
Queries: Execute the provided SQL scripts in your PostgreSQL tool (e.g., pgAdmin) to generate business insights.  
Visualization: Open the Power BI .pbix file (if provided) and refresh the data source to view the updated dashboard.






