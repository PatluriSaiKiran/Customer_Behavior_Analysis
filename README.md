# End-to-End Retail Data Analytics Pipeline (Customer Shopping Trends)

## Project Overview & Strategic Business Value
This project simulates a real-world corporate analytics workflow across three distinct environments:
1. **Python (Data Engineering/ETL):** Automatically extracting, profiling, and cleaning raw, messy customer behavior logs.
2. **SQL (Analytical Processing):** Ingesting the structured datasets into a relational database to run complex analytical business queries (CTEs, Window Functions) to uncover purchasing drivers.
3. **Power BI (Business Intelligence):** Connecting directly to the data infrastructure to deliver an interactive executive dashboard for leadership teams to make data-driven decisions.

---

## 3-Tier Technical Architecture

### 1. Data Engineering Layer (Python)
Instead of relying on heavy visualization libraries (`matplotlib`/`seaborn`), Python was used purely for **ETL operations and database migrations** using the `pandas` and `SQLAlchemy` ecosystems.
* **Data Profiling:** Evaluated data dimensions, missing schemas, and invalid record entries using native Pandas methodologies.
* **Data Scrubber Pipeline:** Normalized text fields, cast date variables into standardized `datetime` objects, and handles null values programmatically.
* **Database Engine Migration:** Established an automated database connection string using Python to programmatically inject the completely clean tabular data directly into an SQL Server/PostgreSQL environment, eliminating manual entry barriers.

### 2. Analytical Processing Layer (SQL)
With the data successfully migrated to the database, advanced relational querying was utilized to extract targeted business KPIs:
* **Cohort & Structural Isolation:** Developed **CTEs (Common Table Expressions)** to keep massive query scripts clean, modular, and easy for peer review.
* **Advanced Sequencing:** Employed **Window Functions** (`ROW_NUMBER()`, `RANK()`) to track purchase intervals, identify repeat buyers, and isolate highest-value customer actions over time.
* **Data Aggregation:** Calculated critical metrics such as Average Order Value (AOV), Purchase Frequency, and customer demographic distribution buckets using precise condition filtering (`CASE WHEN`, `GROUP BY`, `HAVING`).

### 3. Business Intelligence & Semantic Layer (Power BI)
The final delivery layer transitions data from text outputs to an interactive visual engine:
* **Star Schema Architecture:** Optimized the dataset by setting up structured lookup (Dimension) and transactional (Fact) relationships.
* **DAX Formulas:** Developed custom measures using `CALCULATE()` and time-intelligence logic to generate cross-filtering metrics that update instantly based on user interaction.
* **Executive Report UI:** Modeled an enterprise layout featuring high-level summary metrics at the very top, behavioral patterns in the body, and drill-down tables at the bottom.

---

## Tech Stack & Dependencies
* **Data Transformation:** Python 3.x (`pandas`, `sqlalchemy`)
* **Database Management:** SQL (PostgreSQL / MySQL / MS SQL Server)
* **Business Intelligence Engine:** Power BI Desktop

---

##  Core Business Insights & Actions Delivered
* **Revenue Drivers Isolated:** Identified the exact high-value customer segments contributing disproportionately to total business revenue, steering targeted marketing budgets.
* **Slipping Customer Flags:** Created frequency thresholds using SQL to reveal customer cohorts showing early signs of churn risk, enabling the operations team to deploy automated retention workflows.
* **Optimized Marketing Triggers:** Uncovered clear trends in purchasing behavior linked to explicit customer demographics, informing precise cross-selling strategies.

## Dashboard preview 
<img width="1169" height="626" alt="Screenshot 2026-04-29 094127" src="https://github.com/user-attachments/assets/b22fe0a9-88cd-43d6-b31f-961c55e1544b" />







