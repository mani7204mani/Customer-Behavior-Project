🛒 Customer Shopping Behavior Analysis

🧩 Overview

This project analyzes customer shopping behavior using transactional data from 3,900 purchases across various product categories. 

The goal is to uncover insights into spending patterns, product preferences, customer segmentation, and 

subscription behavior to support data-driven business decisions.

The analysis includes data preparation and EDA in Python, business analysis through PostgreSQL SQL queries, and an interactive Power BI 

dashboard to present insights visually.

📁 Dataset Summary

Rows: 3,900

Columns: 18

Key Features:

Customer Demographics: Age, Gender, Location, Subscription Status

Purchase Details: Item Purchased, Category, Purchase Amount, Season, Size, Color

Shopping Behavior: Discount Applied, Promo Code Used, Previous Purchases, Purchase Frequency, Review Rating, Shipping Type

Missing Data: 37 values in the Review Rating column

🛠️ Tools & Technologies

Programming Language: Python (Pandas, NumPy, Matplotlib, Seaborn)

Database: PostgreSQL

Visualization Tool: Power BI

Environment: Jupyter Notebook 

Key Libraries:

pandas – data loading and cleaning

matplotlib, seaborn – EDA and visualization

sqlalchemy, psycopg2 – PostgreSQL integration

🚀 Steps Followed
1. Data Loading & Cleaning (Python)

Imported dataset using Pandas.

Checked structure and summary statistics using .info() and .describe().

Handled missing values in Review Rating by imputing median ratings per category.

Standardized column names using snake_case for consistency.

Engineered new features:

age_group — categorized customer age into ranges.

purchase_frequency_days — calculated average days between purchases.

Removed redundant columns after consistency checks.

Loaded cleaned dataset into PostgreSQL for further analysis.

2. Data Analysis using SQL
   
Performed analytical queries in PostgreSQL to answer key business questions:

Revenue by Gender – compared total revenue between male and female customers.

High-Spending Discount Users – identified customers who used discounts but spent above the average purchase amount.

Top 5 Products by Rating – listed highest-rated products.

Shipping Type Comparison – analyzed spending differences between standard and express shipping.

Subscribers vs. Non-Subscribers – compared spending and revenue.

Discount-Dependent Products – found products with highest percentage of discounted purchases.

Customer Segmentation – classified customers as New, Returning, or Loyal.

Top 3 Products per Category – highlighted most purchased items in each category.

Repeat Buyers & Subscriptions – explored link between frequent purchases and subscriptions.

Revenue by Age Group – calculated revenue contribution across age segments.

4. Power BI Dashboard
   
Developed an interactive Power BI dashboard to visualize results from Python and SQL analysis.

Visuals Used: Bar charts, donut charts, and trend lines.

Filters: Age group, category, subscription status, and season.

KPIs Displayed: Total revenue, average rating, discount usage, and top-performing products.

💡 Business Recommendations

Boost Subscriptions: Promote exclusive subscriber benefits.

Customer Loyalty Programs: Encourage repeat buyers through rewards.

Review Discount Strategy: Balance sales boosts with profit margins.

Product Positioning: Highlight top-rated and best-selling products.

Targeted Marketing: Focus campaigns on high-revenue age groups and express-shipping customers.

▶️ How to Run
Clone the repository:

bash
Copy code
git clone [[https://github.com/yourusername/customer-shopping-analysis.git](https://github.com/mani7204mani/Customer-Behavior-Project/)](https://github.com/mani7204mani/Customer-Behavior-Project.git)
cd Customer-Behavior-Project
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Set up PostgreSQL:

Create a database (e.g., customer_behaviour)

Update credentials in the Python script or notebook.

Run the analysis:

bash
Copy code
jupyter notebook
Execute cells step by step to perform data cleaning, EDA, and SQL queries.

View Dashboard:

Open Customer Behavior Dashboard.pbix in Power BI to explore visual insights.

📄 Report & Dashboard

Full analytical report: Customer Shopping Behavior Analysis.pdf

Power BI dashboard file: Customer Behavior Dashboard.pbix

Screenshots available in dashboard/ folder

👨‍💻 Author
P .Mani Shankar

Innovative Software Developer | Aspiring Data Engineer

📧 mani7204mani@gmail.com

🔗 LinkedIn | GitHub

