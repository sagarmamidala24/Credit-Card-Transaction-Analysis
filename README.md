# Credit-Card-Transaction-Analysis

The Credit Card Transactions Analysis project explores transaction trends, detects anomalies, and extracts insights using Pandas. 
It includes data cleaning, manipulation, and fraud detection. Key analyses include transaction categorization, aggregation, customer behavior insights, and merging customer data.
The data analysis feature engineering, visualization, and insights generation on a dataset of credit card transactions.
Here's a summary of the key steps:

## 1️⃣ Data Exploration and Cleaning
Data Loading: Loads the dataset into a DataFrame and displays the first 5 rows.

Shape & Columns: Checks the dimensions and column names of the dataset.

Summary Statistics: Explores numerical columns with descriptive statistics.

Missing Values: Verifies no missing values and removes duplicates if needed.

Date Conversion: Converts Transaction_Date to datetime format and extracts year, month, and day.

## 2️⃣ Data Selection and Indexing
Filter Transactions: Extracts specific data:

Transactions in January 2023.

Transactions with Amount > 1000 and Transaction_Type = "Online".

Transactions marked as "Approved".

## 3️⃣ Data Manipulation and Feature Engineering
New Columns:

Calculates a 5% discount on transactions over $500 (Discounted_Amount).

Categorizes Amount as "Low," "Median," or "High" (T_Level).

Column Removal: Drops columns with over 30% missing values.

## 4️⃣ Aggregation and Insights
Insights Generated:

Total transaction amount per Category.

Count of declined transactions per Payment_Mode.

Top 5 merchants based on transaction count.

Average transaction amount per Location.

## 5️⃣ Fraud Detection Indicators
Patterns and Red Flags:

Identifies customers making over 10 transactions in a single day.

Finds transactions for the same Customer_ID in different locations within 5 minutes.

Flags transactions with Amount > $5000 and Transaction_Type = "Online" as high-risk.

## 6️⃣ Data Merging and Joining
Merge Operation: Combines customer demographic data with transaction data using Customer_ID.

Insights by Age Group: Finds average transaction amount for different age groups.

## 📊 Visualization
Bar Chart: Displays total transaction amount per Category using Seaborn.

Correlation Heatmap: Shows relationships between Amount, Transaction_Status, and Payment_Mode.

The code integrates data cleaning, analysis, and visual storytelling, providing deep insights into credit card transactions and identifying potential fraud patterns.
