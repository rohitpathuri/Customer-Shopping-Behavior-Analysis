# Customer-Shopping-Behavior-Analysis
Customer Shopping Behavior Analysis – An end-to-end data analytics project using Python, SQL, and Power BI to analyze 3,900 customer transactions. Uncovers insights on spending patterns, customer segmentation, product performance, and subscription behavior to support data-driven business decisions.

📊 Customer Shopping Behavior Analysis

An end-to-end data analytics project that analyzes customer shopping behavior using transactional data from 3,900 purchases. The project leverages **Python, SQL (PostgreSQL), and Power BI** to uncover insights into customer spending patterns, product performance, discount usage, and subscription behavior, supporting data-driven business decision-making. :contentReference[oaicite:0]{index=0}

📌 Project Overview

Understanding customer behavior is critical for optimizing sales strategies, improving customer retention, and increasing revenue.  
This project analyzes real-world transactional data to identify key trends in customer demographics, purchasing behavior, and product preferences.

**Key Goals:**
- Identify high-value customers and profitable segments
- Analyze the impact of discounts and subscriptions
- Understand product performance across categories
- Provide actionable business recommendations through data insights


📂 Dataset Summary

- **Total Records:** 3,900 transactions  
- **Total Features:** 18 columns  

Key Attributes:
- **Customer Demographics:** Age, Gender, Location, Subscription Status  
- **Purchase Details:** Item Purchased, Category, Purchase Amount, Season, Size, Color  
- **Behavioral Data:**  
  - Discount Applied  
  - Previous Purchases  
  - Purchase Frequency  
  - Review Rating  
  - Shipping Type  

Data Quality:
- 37 missing values found in the `review_rating` column
- Missing values were handled using **median imputation by product category**


🔧 Data Cleaning & Preprocessing (Python)

Data preprocessing was performed using **Python (Pandas & NumPy)** and included:

- Data loading and inspection using `df.info()` and `df.describe()`
- Handling missing values in review ratings
- Standardizing column names to **snake_case**
- Feature engineering:
  - `age_group` (Young Adult, Adult, Middle-aged, Senior)
  - `purchase_frequency_days`
- Data consistency checks:
  - Identified redundancy between `discount_applied` and `promo_code_used`
  - Removed unnecessary columns
- Loaded cleaned data into **PostgreSQL** for SQL-based analysis

🗄️ SQL Analysis (PostgreSQL)

The cleaned dataset was analyzed using SQL to answer key business questions:

Key Analyses:
1. **Revenue by Gender** – Compared total revenue contribution by male and female customers  
2. **High-Spending Discount Users** – Identified customers who used discounts but still spent above average  
3. **Top 5 Products by Rating** – Ranked products based on average review ratings  
4. **Shipping Type Comparison** – Compared average purchase value between Standard and Express shipping  
5. **Subscribers vs Non-Subscribers** – Analyzed spending behavior and revenue contribution  
6. **Discount-Dependent Products** – Identified products with the highest discount dependency  
7. **Customer Segmentation** – Classified customers into New, Returning, and Loyal segments  
8. **Top Products by Category** – Identified best-selling products in each category  
9. **Repeat Buyers & Subscriptions** – Checked if repeat buyers are more likely to subscribe  
10. **Revenue by Age Group** – Evaluated revenue contribution across age groups  


 📊 Power BI Dashboard

An interactive **Power BI dashboard** was built to visualize insights and KPIs, including:

- Total customers and average purchase amount
- Subscription distribution
- Revenue and sales by category
- Revenue and sales by age group
- Customer behavior filters for deeper exploration

The dashboard enables stakeholders to quickly identify trends and make informed decisions.


💡 Business Recommendations

Based on analytical insights, the following recommendations were proposed:

- **Boost Subscriptions:** Promote exclusive benefits to increase subscriber base  
- **Customer Loyalty Programs:** Reward repeat buyers to convert them into loyal customers  
- **Optimize Discount Strategy:** Balance discounts to improve sales without hurting margins  
- **Product Positioning:** Highlight top-rated and best-selling products in campaigns  
- **Targeted Marketing:** Focus on high-revenue age groups and express-shipping users  


🛠️ Tech Stack

- **Python** (Pandas, NumPy)
- **SQL** (PostgreSQL)
- **Power BI**
- **Jupyter Notebook**



