# Customer_Shopping_Behavior_Analysis
Customer Shopping Behavior Analysis
Overview
This project analyzes customer shopping behavior using transactional data from 3,900 purchases across multiple product categories.
The goal is to uncover insights into:
Spending patterns
Customer segmentation
Product preferences
Subscription behavior
The findings aim to help businesses improve marketing strategies, customer retention, and overall profitability.

Dataset
Source: Provided in Excel format
Rows: 3,900
Columns: 18

Key Features
Demographics: Age, Gender, Location, Subscription Status
Purchase Details: Item Purchased, Category, Purchase Amount, Season, Size, Color
Behavioral Data: Discount Applied, Promo Code Used, Frequency of Purchases, Review Rating, Shipping Type
Missing Data: 37 values in the Review Rating column

Tools & Technologies
Tool	Purpose
Python (Pandas, NumPy)	Data loading, cleaning, and preprocessing
PostgreSQL	Running SQL queries for business insights
Power BI	Dashboard creation and data visualization
Gamma App	Report and presentation design
Excel	Initial data source

Project Steps
1. Data Preparation (Python)
Imported dataset using pandas
Checked structure and summary statistics using .info() and .describe()
Handled missing values in Review Rating column (filled with median per product category)
Renamed columns to snake_case for readability
Added new features:
age_group (binned customer ages)
purchase_frequency_days (derived from timestamps)
Checked redundancy between discount_applied and promo_code_used
Loaded cleaned dataset into PostgreSQL for structured analysis

2.SQL Analysis (PostgreSQL)
Key analytical queries performed:
Revenue by Gender – Compare total revenue between male and female customers
High-Spending Discount Users – Find customers who use discounts but spend above average
Top 5 Products by Rating – Identify best-rated products
Shipping Type Comparison – Compare average purchase amount by shipping type
Subscribers vs. Non-Subscribers – Analyze spending and revenue differences
Discount-Dependent Products – Find products heavily reliant on discounts
Customer Segmentation – Classify users as New, Returning, or Loyal
Top 3 Products per Category – Rank best-selling items per category
Repeat Buyers & Subscriptions – Study correlation between repeat purchases and subscription
Revenue by Age Group – Determine high-revenue demographics

Power BI Dashboard-
An interactive Power BI dashboard was created to visualize:
Total revenue and purchase distribution
Gender-wise and age-group spending
Top products and best-rated categorie
Discount trends and subscription insights

4.Business Recommendations
Boost Subscriptions: Offer exclusive member benefits
Reward Loyalty: Introduce repeat-buyer reward programs
Review Discount Strategy: Ensure discounts drive growth sustainably
Promote Top Products: Use insights from high-rated items in campaigns
Target Marketing: Focus on high-revenue demographics and express-shipping customers

Results
Identified key spending patterns and high-value customer segments
Discovered that loyal and express-shipping customers generate higher revenue
Found that subscription plans significantly improve repeat purchase rates

How to Run
Prerequisites
Python (>=3.8)
PostgreSQL (installed and running)
Power BI Desktop

Steps
Clone this repository:
git clone https://github.com/Patilrohan0099/customer-_behavior_analysis.git
Open the dataset in Excel or Python for review
Run the data cleaning script in Python
Load the cleaned data into PostgreSQL
Execute SQL queries from the provided .sql file
Open the Power BI file to explore the dashboard
View the detailed report and presentation made in Gamma
