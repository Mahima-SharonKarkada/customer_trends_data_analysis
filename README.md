# customer_trends_data_analysis
Analyzed 3,900 retail transactions using Python, PostgreSQL &amp; Power BI. Covers data cleaning, SQL business queries, customer segmentation, discount patterns &amp; revenue trends. Built an interactive dashboard and derived actionable business recommendations. My first end-to-end data analytics project.

🛍️ CUSTOMER SHOPPING BEHAVIOUR ANALYSIS

Uncovering retail trends through data from raw transactions to actionable business strategy.
🌱 This is my first end-to-end data analytics project, completed > as part of my learning journey into data analysis.

<u><b>PROJECT OVERVIEW</b></u>
A leading retail company sought to better understand its customers' shopping behavior to improve sales, customer satisfaction, and long-term loyalty. This end-to-end data analysis project works through 3,900 transactional records across multiple product categories to surface insights on spending patterns, customer segments, product preferences, and subscription behaviour.

Core Business Question:
"How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?"

 
Dataset Summary
Property	Detail
Rows	3,900
Columns	18
Missing Data	37 values in Review Rating
Key Features:
•	Demographics: Age, Gender, Location, Subscription Status
•	Purchase Details: Item Purchased, Category, Purchase Amount (USD), Season, Size, Color
•	Behavior: Discount Applied, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type, Payment Method

 Data Preparation (Python)
Performed using pandas in Python:
•	Data Loading — Imported dataset and explored structure with df.info() and .describe()
•	Missing Data Handling — Imputed missing Review Rating values using the median rating per product category
•	Column Standardization — Renamed all columns to snake_case
•	Feature Engineering: 
o	age_group — binned customer ages into segments (Young Adult, Adult, Middle-aged, Senior)
o	purchase_frequency_days — derived from purchase frequency data
•	Redundancy Check — Confirmed discount_applied and promo_code_used were redundant; dropped promo_code_used
•	Database Integration — Loaded cleaned DataFrame into PostgreSQL for SQL analysis

Data Analysis (PostgreSQL)
Ten business queries were run to extract key insights:
	Query	Key Finding
1	Revenue by Gender	Male: $157,890 · Female: $75,191
2	High-Spending Discount Users	839 customers used discounts yet spent above average
3	Top 5 Products by Rating	Gloves (3.86), Sandals (3.84), Boots (3.82)
4	Shipping Type Comparison	Express avg: $60.48 · Standard avg: $58.46
5	Subscribers vs. Non-Subscribers	Subscribers: 1,053 · Non-subscribers: 2,847
6	Discount-Dependent Products	Hat (50%), Sneakers (49.66%), Coat (49.07%)
7	Customer Segmentation	Loyal: 3,116 · Returning: 701 · New: 83
8	Top 3 Products per Category	Jewelry, Blouse, Sandals, Jacket lead their categories
9	Repeat Buyers & Subscriptions	2,518 repeat buyers are non-subscribers  opportunity!
10	Revenue by Age Group	Young Adult: $62,143 · Middle-aged: $59,197

Power BI Dashboard
An interactive dashboard was built to visualize key metrics and trends:
KPI Cards:
•	📦 3.9K Total Customers
•	💰 $59.76 Average Purchase Amount
•	⭐ 3.75 Average Review Rating
Visuals Included:
•	% of Customers by Subscription Status (Donut Chart)
•	Revenue & Sales by Category (Bar Charts)
•	Revenue & Sales by Age Group (Horizontal Bar Charts)
Filters/Slicers: Subscription Status, Gender, Category, Shipping Type

 Business Recommendations
1.	Boost Subscriptions — Only 27% of customers subscribe. Promote exclusive subscriber perks (early access, free shipping) to convert the 2,518 non-subscribing repeat buyers.
2.	Customer Loyalty Programs — Reward Returning customers to accelerate their move into the Loyal segment.
3.	Review Discount Policy — Nearly half of Hat and Sneaker purchases are discounted. Audit margins and test discount thresholds to avoid over-reliance.
4.	Product Positioning — Spotlight top-rated items (Gloves, Sandals, Boots) and top-selling products (Jewelry, Blouse, Jacket) in campaigns.
5.	Targeted Marketing — Prioritize Young Adults and Middle-aged customers (highest revenue contributors) and Express-shipping users (higher avg spend).

🛠️ Tech Stack : 
•	Python (pandas for data cleaning & EDA) 
•	SQL / PostgreSQL (business queries & analysis) 
•	Power BI (interactive dashboard & visualization)


🎓 WHAT I LEARNED
- How to clean and prepare real-world messy data using  pandas 
  (handling nulls, renaming columns, feature engineering)
- Writing SQL queries for actual business questions  segmentation,
  ranking, aggregations, and window functions
- How to connect Python to PostgreSQL and load DataFrames directly
  into a database
- Building an  interactive Power BI dashboard  with slicers, KPI cards,
  and multiple chart types
- Thinking like a data analyst by  translating raw data into business
  Recommendations

🙏 ACKNOWLEDGEMENTS 
This project was inspired by and built along with a tutorial on YouTube by 
Amlan Mohanty . All analysis, code, and insights were implemented and documented by me as a hands-on learning exercise.
