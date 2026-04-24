# Data Warehouse and OLAP Project - Financial Fraud Detection from Loan Application and Banking Transaction Data

## 📌 General Information
- **University:** University of Information Technology - VNU-HCM (UIT)
- **Course:** Data Warehouse and OLAP (IS217.Q11)
- **Instructor:** MSc. Do Thi Minh Phung
- **Team Members:**
  - Dinh Van Lam - 23520829
  - Dang Nguyen Hoang Thach - 23521411

## 🎯 Project Objectives
Fraud in loan applications and financial transactions is a major risk for credit institutions. This project focuses on researching and designing a Data Warehouse using ETL processes, multi-dimensional data analysis (OLAP), data visualization via Dashboards, and Data Mining algorithms to assist in the early detection of financial fraud.

## 📊 Dataset
- **Source:** [Kaggle - Loan Application & Transaction: Fraud Detection](https://www.kaggle.com/datasets/prajwaldongre/loan-application-and-transaction-fraud-detection)
- **Size:** 50,000 rows, 21 columns (reduced to 16 columns after Python preprocessing).
- **Content:** Customer profile information, loan details, income, credit score (CIBIL), application status (Approved/Declined), and fraud flags.

## 🛠 Technologies and Tools Used
- **Data Preprocessing:** Python (Pandas)
- **Data Warehouse Construction (ETL):** SQL Server Integration Services (SSIS), Microsoft SQL Server (SSMS).
- **Multi-dimensional Analysis (Cube):** SQL Server Analysis Services (SSAS), MDX query language.
- **Data Visualization (BI Dashboard):** Power BI, Google Data Studio (Looker Studio).
- **Data Mining:** Python, XGBoost, Random Forest.

## 🗄️ Data Warehouse Architecture (Star Schema)
The Data Warehouse schema is designed using a Star Schema, which includes:
- **Fact Table:** `FACT` (contains measures such as requested loan amount, loan term, monthly income, credit score, EMI...).
- **Dimension Tables:**
  - `DIM_CUSTOMER`: Customer demographic information.
  - `DIM_DATE`: Time dimension (Day, month, year, quarter of application).
  - `DIM_LOANTYPE`: Loan classification dimension.
  - `DIM_LOANPURPOSE`: Loan purpose dimension.
  - `DIM_PROPERTY`: Property ownership status dimension.
  - `DIM_LOCATION`: Geographic area dimension (Address, city, state).
  - `DIM_LOANSTATUS`: Application processing status dimension.
  - `DIM_FRAUDFLAG`: Flag indicating whether the application is fraudulent.

## 📈 Key Achievements
1. **ETL & OLAP:**
   - Successfully built an automated data cleaning and loading process (ETL) into the Data Warehouse.
   - Configured a Cube model with multiple hierarchies, returning fast results for 15 complex MDX analytical queries.
2. **Data Visualization (BI):**
   - Deployed highly interactive Dashboards on Power BI and Looker Studio.
   - Provided insights into loan distribution, application approval trends over time, and risk rates across different states.
3. **Data Mining:**
   - Solved a Classification problem based on highly imbalanced data (Approved 83.5% vs. Declined 16.5%).
   - Trained and evaluated the effectiveness of two models: **XGBoost** and **Random Forest**.
   - Extracted Feature Importance to analyze the independent variables that most strongly influence application rejection decisions (e.g., low CIBIL score, monthly income, etc.).
