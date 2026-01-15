Customer Shopping Behavior Analysis

1. **Overview**
This end-to-end data analytics project explores customer transactional behavior to drive strategic business decisions. By analyzing 3,900 purchases, the project identifies key spending patterns, customer segments, and product preferences. The workflow spans from raw data cleaning in Python to relational database management in PostgreSQL, culminating in an interactive Power BI dashboard and an AI-generated executive presentation.

2. **Dataset**
-Source: Transactional Purchase Data.
-Size: 3,900 rows and 18 columns.
-Key Features: Customer demographics (Age, Location, Subscription Status), purchase details (Category, Amount, Item), and behavioral data (Review Ratings, Discount usage, Shipping type).
-Data Quality: Addressed 36 missing values in the Review Rating column via median imputation.

3. Tech Stack & ToolsPhaseTools
 UsedData Cleaning & EDA **Python (Pandas, NumPy)**
 Database Management ****PostgreSQL**
 Business Intelligence- **Power BI**
 Presentation & Reporting **Gamma (AI PPT), MS Word**

4. Project Steps
   Phase 1: Python EDA & Data Cleaning

Initial Exploration: Performed structural checks using df.info() and summary statistics with .describe().
Data Imputation: Filled missing review ratings using category-specific medians.
Feature Engineering: * Binned ages into an age_group column.
Derived purchase_frequency_days.
Standardized columns to snake_case for database compatibility.
Redundancy Check: Dropped promo_code_used after verifying overlap with discount_applied.

Phase 2: SQL Analysis (PostgreSQL)

Cleaned data was migrated to PostgreSQL to answer critical business questions:
Revenue Segmentation: Compared performance by Gender and Age Group.
Customer Loyalty: Classified buyers into "New," "Returning," and "Loyal" segments based on purchase history.
Shipping & Subscription Impact: Analyzed if higher spend correlates with express shipping or subscription status.
Product Performance: Identified the Top 3 items within each category and products most dependent on discounts.

5. Dashboard (Power BI)
The interactive Power BI dashboard provides a visual breakdown of:
Key KPIs: Total Customers (3.9K), Average Purchase Amount ($59.76), and Average Review Rating (3.75).
Demographic Insights: Revenue and Sales volume by Age Group and Gender.
Subscription Trends: Distribution of subscribers (27%) vs. non-subscribers (73%).
Category Analysis: Comparative sales between Clothing, Accessories, Footwear, and Outerwear.

6. Results & Recommendations

Revenue Leaders: Male customers contributed significantly more revenue ($157,890) compared to female customers ($75,191).
Segment Strength: The "Loyal" customer segment is the largest, with over 3,100 customers.
Actionable Insights: * Boost Subscriptions: Implement targeted promotions to convert the 73% of non-subscribers.
Strategic Marketing: Focus campaigns on high-revenue age groups (Middle-aged and Adults).
Margin Control: Review discount policies for products like "Hats" and "Sneakers," which show high discount dependency.

