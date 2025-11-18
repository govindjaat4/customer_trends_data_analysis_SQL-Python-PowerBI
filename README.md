# customer_trends_data_analysis_SQL-Python-PowerBI
Customer Shopping Behavior Analysis
📌 Project Overview
This project analyzes customer shopping behavior using transactional data from 3,900 purchases across various product categories. The primary goal is to uncover insights into spending patterns, customer segments, product preferences, and subscription behavior to guide strategic business decisions.


📂 Dataset Summary
The dataset contains 3,900 rows and 18 columns. It includes the following key features:


Customer Demographics: Age, Gender, Location, Subscription Status.


Purchase Details: Item Purchased, Category, Purchase Amount, Season, Size, Color.


Shopping Behavior: Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type.


Data Quality: There were 37 missing values in the 'Review Rating' column which required handling.

🛠 Tech Stack

Python (Pandas): Data cleaning, preprocessing, and feature engineering.


SQL (PostgreSQL): Structured data analysis and solving business questions.



Power BI: Interactive dashboard creation for visual insights.

⚙️ Methodology
1. Data Preparation & Cleaning (Python)
Before analysis, the raw data was processed using Python:


Missing Data Handling: Imputed null values in the Review Rating column using the median rating of each product category.


Standardization: Renamed columns to "snake_case" for better readability and consistency.

Feature Engineering:

Created an age_group column by binning customer ages.

Derived a purchase_frequency_days column from purchase data.


Optimization: Dropped redundant columns (e.g., promo_code_used) after consistency checks.


Database Integration: Loaded the cleaned DataFrame into PostgreSQL for SQL analysis.

2. Exploratory Data Analysis (SQL)
Key business questions were answered using SQL queries:


Revenue by Gender: Male customers generated $157,890 in revenue compared to $75,191 by Female customers.



Top Products: Identified top-rated products, with "Gloves" achieving the highest average rating of 3.86.


Shipping Analysis: Express shipping users had a slightly higher average purchase amount ($60.48) than Standard shipping users ($58.46).


Customer Segmentation: The majority of customers (3,116) fall into the "Loyal" segment.


Age Demographics: The "Young Adult" group contributed the highest total revenue ($62,143).

3. Visualization (Power BI)
An interactive dashboard was built to track KPIs and trends:


Total Customers: 3.9K.


Average Purchase Amount: $59.76.


Average Review Rating: 3.75.


Visuals Included: Revenue by Category, Sales by Age Group, and Subscription Status distribution.



📊 Key Insights & Business Recommendations
Based on the analysis, the following strategies are recommended:


Boost Subscriptions: Promote exclusive benefits to convert non-subscribers, as only 27% of customers are currently subscribed.



Customer Loyalty: Implement programs to reward repeat buyers and maintain the large "Loyal" customer segment.


Targeted Marketing: Focus marketing efforts on high-revenue groups, specifically Young Adults and customers opting for Express Shipping.


Product Positioning: Highlight top-rated products (e.g., Gloves, Sandals) and discount-dependent items (e.g., Hats, Sneakers) in campaigns.


This project demonstrates the end-to-end data analysis lifecycle from Python preprocessing to SQL querying and Power BI visualization.
