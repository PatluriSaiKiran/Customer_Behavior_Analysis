🛍️ Customer Shopping Behavior Analysis
📌 Overview

This project presents an end-to-end data analytics workflow focused on analyzing customer purchasing behavior to generate actionable business insights.

The goal is to identify revenue drivers, customer segments, and product performance trends using a combination of data processing, SQL analysis, and interactive visualization.

📂 Dataset
File: customer_shopping_behavior.csv
Records: ~3,900 rows
Features include:
Customer demographics (age, gender)
Transaction details (purchase amount, category, item)
Behavioral attributes (subscription status, shipping type, review ratings)
🛠️ Tools & Technologies
Python (Pandas, SQLAlchemy) → Data Cleaning, EDA, ETL
PostgreSQL → Data Storage & Advanced Querying
Power BI → Dashboard & Data Visualization
VS Code → Development Environment
⚙️ Project Workflow
1️⃣ Data Cleaning & Feature Engineering (Python)
Handled missing values in review_rating using category-wise median imputation
Standardized column names (lowercase, underscores)
Created new features:
age_group (using quantile-based binning)
purchase_frequency_days
2️⃣ Database Integration
Connected Python to PostgreSQL using SQLAlchemy
Loaded cleaned data into customer_behavior database
Structured data into relational format for efficient querying
3️⃣ Advanced SQL Analysis
Revenue contribution by gender
Customer segmentation:
New Customers
Returning Customers
Loyal Customers
Product ranking within categories
Purchase behavior analysis
4️⃣ Data Visualization (Power BI)

Developed an interactive dashboard to present key insights:

📊 KPIs:
Total Customers: 3.9K
Avg Purchase Amount: $59.76
Avg Review Rating: 3.75
👥 Demographic Insights:
Revenue distribution across age groups
🛍️ Category Analysis:
Sales by product category
🔁 Subscription Trends:
27% customers are subscribers
📈 Key Insights
Identified top-performing product categories driving revenue
Found clear spending patterns across age groups
Segmented customers into New, Returning, and Loyal
Analyzed impact of subscriptions on revenue
Compared shipping preferences vs spending behavior
🚀 How to Run the Project
1️⃣ Setup Python Environment
pip install pandas sqlalchemy psycopg[binary]
2️⃣ Database Setup
Install and run PostgreSQL
Create database:
CREATE DATABASE customer_behavior;
3️⃣ Run Data Pipeline
Execute Python script / Jupyter Notebook to:
Clean data
Transform features
Load into PostgreSQL
4️⃣ Run SQL Queries
Use pgAdmin or any SQL tool
Execute analysis queries to generate insights
5️⃣ Power BI Dashboard
Open .pbix file
Refresh data connection
Explore interactive dashboard
📁 Project Structure
📦 Customer-Shopping-Analysis
 ┣ 📂 data
 ┃ ┗ customer_shopping_behavior.csv
 ┣ 📂 scripts
 ┃ ┗ data_cleaning.py
 ┣ 📂 sql
 ┃ ┗ analysis_queries.sql
 ┣ 📂 dashboard
 ┃ ┗ customer_analysis.pbix
 ┣ 📄 README.md
💡 Key Learnings
Built a complete ETL pipeline (Python → PostgreSQL → Power BI)
Improved data cleaning & feature engineering skills
Gained hands-on experience in advanced SQL analysis
Learned to transform raw data into business insights






