🛍️ Customer Shopping Behavior Analysis
SQL • Python • Power BI

This project analyzes 3,900 customer shopping transactions to uncover insights into spending patterns, product preferences, customer segments, and subscription behavior. The analysis combines Python for EDA, PostgreSQL for business queries, and Power BI for dashboarding.

📘 1. Project Overview

The goal of this project is to understand customer shopping behavior and drive data-backed business decisions.
We explored relationships between demographics, purchase behavior, discounts, shipping types, and review ratings.

🗂️ 2. Dataset Summary

Rows: 3,900
Columns: 18
Key Features:
Customer demographics (Age, Gender, Location, Subscription Status)
Purchase details (Item, Category, Amount, Season, Size, Color)
Behavioral fields (Discount Applied, Promo Code, Previous Purchases, Frequency, Rating, Shipping Type)
Missing Values: 37 missing ratings (imputed using median per category)

🐍 3. Exploratory Data Analysis (Python)

Performed detailed data cleaning and preparation:
✔ Data Cleaning
Loaded data using pandas
Standardized column names to snake_case
Imputed missing review_rating values
Checked redundancy between discount_applied and promo_code_used → removed promo code
Feature engineering:
age_group (binned ages)
purchase_frequency_days

✔ Database Integration
Loaded cleaned dataset into PostgreSQL using SQLAlchemy for SQL-based business analysis.

🛢️ 4. SQL Analysis (PostgreSQL)

Executed analytical SQL queries to answer business questions:
Revenue by Gender
High-Spending Discount Users
Top 5 Products by Review Rating
Shipping Type: Standard vs. Express Spend Comparison
Subscriber vs. Non-Subscriber Spending
Products Most Dependent on Discounts
Customer Segmentation: New, Returning, Loyal
Top 3 Best-Selling Products per Category
Subscription Likelihood of Repeat Buyers (>5 purchases)
Revenue Contribution by Age Group

📊 5. Power BI Dashboard

Created an interactive dashboard highlighting:
Revenue trends
Subscriber vs. non-subscriber behavior
Demographic insights
Top-rated & top-selling products
Discount analysis
Shipping preferences
The dashboard helps decision-makers quickly identify growth opportunities.

💡 6. Business Recommendations

Based on the analysis:
Boost Subscriptions through targeted benefits
Implement Loyalty Programs for repeat buyers
Optimize Discount Strategy to protect margins
Promote High-Rated & Best-Selling Products
Run Targeted Marketing Campaigns for top age groups and express-shipping users

📦 Tech Stack

Python: Pandas, NumPy, Matplotlib/Seaborn
Database: PostgreSQL
Visualization: Power BI
Tools: SQLAlchemy, Jupyter Notebook
