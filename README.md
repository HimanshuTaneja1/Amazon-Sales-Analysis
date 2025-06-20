
Amazon Sales Data Analysis Project
Overview
This project leverages SQL to analyze Amazon sales data, addressing 22 advanced business problems to derive actionable insights into sales performance, customer behavior, inventory management, and operational efficiency. The analysis uses a relational database to answer complex business questions, such as identifying top-selling products, calculating customer lifetime value, and detecting shipping delays.

Objectives
Analyze sales trends, product performance, and customer purchasing patterns.
Identify operational inefficiencies, such as low stock levels or shipping delays.
Provide data-driven recommendations for inventory, cross-selling, and seller performance optimization.
Dataset
The dataset includes Amazon sales data with the following key tables and attributes:

Sales/Orders: Order ID, product ID, product name, category, sales amount, order date, customer ID, shipping provider.
Customers: Customer ID, name, registration date, state.
Inventory: Product ID, stock quantity, last restock date, warehouse details.
Payments: Order ID, payment status (success, failed, pending).
Returns: Order ID, product ID, return details.
Sellers: Seller ID, sales records, order status. (Note: Adjust table/column names based on your actual dataset schema.)
Tools and Technologies
SQL: Core tool for querying, transforming, and analyzing data.
Database: [Specify database, e.g., MySQL, PostgreSQL, SQLite].
Other Tools: [Optional, e.g., Python for preprocessing, Tableau for visualizations].
Project Structure
data/: Raw and processed dataset files (if included).
sql_queries/: SQL scripts for the 22 business problems and stored procedures.
results/: Output reports, summaries, or visualizations from the analysis.
schema.sql: Database schema setup (if applicable).
README.md: Project overview and instructions.
Setup Instructions
Clone the Repository:
bash
git clone https://github.com/your-username/amazon-sales-analysis.git
Set Up the Database:
Import the dataset into your SQL database (e.g., MySQL, PostgreSQL).
Run schema.sql to create the necessary tables and relationships.
Execute SQL Queries:
Navigate to the sql_queries/ folder.
Run the SQL scripts in your database management tool (e.g., MySQL Workbench, pgAdmin).
Review Results:
Check the results/ folder for query outputs or generated reports.
Analysis Scope
This project addresses 22 advanced business problems, each implemented as an SQL query to extract meaningful insights. Below is a summary of the key analyses:

Top Selling Products: Identifies the top 10 products by sales value, including quantity sold.
Revenue by Category: Calculates total revenue per product category with percentage contributions.
Average Order Value (AOV): Computes AOV for customers with more than 5 orders.
Monthly Sales Trend: Tracks monthly sales over the past year, comparing current and previous months.
Customers with No Purchases: Lists registered customers without orders, including registration duration.
Least-Selling Categories by State: Identifies the lowest-performing categories per state with sales totals.
Customer Lifetime Value (CLTV): Ranks customers by their total order value.
Inventory Stock Alerts: Flags products with stock below 10 units, including restock details.
Shipping Delays: Detects orders with shipping delays exceeding 3 days.
Payment Success Rate: Calculates the percentage of successful payments with status breakdowns.
Top Performing Sellers: Ranks top 5 sellers by sales value, including success rates.
Product Profit Margin: Ranks products by profit margin (price minus cost of goods sold).
Most Returned Products: Identifies top 10 products by return count with return rates.
Orders Pending Shipment: Lists paid orders awaiting shipment with payment details.
Inactive Sellers: Finds sellers with no sales in the last 6 months, including last sale date.
Customer Segmentation: Categorizes customers as "returning" (>5 returns) or "new".
Cross-Sell Opportunities: Suggests products for cross-selling based on purchase patterns.
Top Customers by State: Identifies top 5 customers per state by order count and sales.
Revenue by Shipping Provider: Analyzes revenue, order count, and delivery times by provider.
Decreasing Revenue Products: Lists top 10 products with the highest revenue decline (2022 vs. 2023).
Stored Procedure: Automatically updates inventory stock when sales are recorded.
Key Insights
