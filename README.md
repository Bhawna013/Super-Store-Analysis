# Super-Store-Analysis
This analysis aims to extract business insights from e-commerce order data to inform sales, marketing, and customer retention strategy.

Sales & Marketing Analytics Report


* Dataset: Superstore E-commerce Orders

* Tools used: Python, Pandas, Matplotlib, Seaborn

	<img width="435" height="272" alt="image" src="https://github.com/user-attachments/assets/6d39f6a4-1a70-4633-b47a-6344729178fa" />


* Author: Bhawna Kumari



1. Project Overview & Objectives

This analysis aims to extract business insights from e-commerce order data to inform sales, marketing, and customer retention strategy. The key objectives are:

a. Understand historical sales trends over time.

b. Decompose revenue by category and region to reveal high/low performing segments.
			
c. Analyze repeat customers (cohort analysis, segmentation) to measure loyalty and retention.
			
d. Segment customers (by spend / frequency) using RFM / clustering.
			
e. Present findings in a clean, narrative dashboard/visualization for stakeholders.



2. Data Preparation & Cleaning

A. Loading & parsing

* Read the CSV with pd.read_csv(...); parse date columns into datetime types.
<img width="1125" height="233" alt="image" src="https://github.com/user-attachments/assets/78deca24-7aa3-4a48-bd26-82fdb81a82b3" />
<img width="1490" height="409" alt="image" src="https://github.com/user-attachments/assets/82d37bcc-42b0-4e22-9e26-5f620caaaa43" />


* Use pd.to_datetime() with dayfirst=True to correctly interpret DD-MM-YYYY style dates.

B. Cleaning numeric fields

* The sales (and similar) columns sometimes had thousand separators (spaces or commas). These were removed (e.g. .str.replace(' ', '').str.replace(',', '')) before converting to numeric types.

* This ensures aggregations (sum, mean) work correctly.

C. Categorical conversions

* Columns like segment, state, category, sub_category, region etc. were cast to Pandas category dtype to reduce memory footprint and speed up grouping operations.

D. Feature engineering

* Created additional derived variables:

	* shipping_days and a binned category shipping_speed (Fast / Medium / Slow) from shipping duration.

	* Flags like order_is_weekend, delivery_is_weekend, high_discount, etc.



🧾 Key Insights & Business Takeaways

Based on the analysis of the SuperStore Orders dataset, here are the key performance highlights and strategic insights derived from the data:

📊 Overall Business Performance:

| Metric                        | Value                                                 |
| :---------------------------- | :---------------------------------------------------- |
| **Total Sales**               | **$12,642,905**                                       |
| **Total Profit**              | **$1,469,035**                                        |
| **Profit Margin**             | **11.62%**                                            |
| **Average Order Value (AOV)** | **$505.01**                                           |
| **Total Orders**              | **25,035**                                            |
| **Unique Customers**          | **795** (100% repeat customers → excellent retention) |
| **Unique Products**           | **10,292**                                            |
| **Average Shipping Days**     | **3.97 days**                                         |


💡 The business shows strong customer retention and consistent order volume, with a healthy overall profit margin.


🏆 Top Performers

Top-Selling Products:

  * Dominated by Technology and Furniture categories.

  * “Apple Smart Phone, Full Size” is the highest-selling product.

Top-Profit Products:

 * “Canon imageCLASS 2200 Advanced Copier” generates the most profit.

Top Customers by Sales:

 * Sean Miller and Tamara Chand lead in total sales.

Top Customers by Profit:

 * Tamara Chand and Raymond Buch are the most profitable customers.

Most Frequently Sold Product:
	
 * Staples appears most often in orders, indicating strong office supply demand.




⚠️ Loss-Making Products

Some products — notably “Cisco TelePresence System EX90 Videoconferencing Unit” and certain printers and furniture items — show negative profit margins.

📉 These items likely suffer from pricing, cost, or discounting inefficiencies and warrant a profitability review.




🌍 Geographical Performance

Top Countries:

  * United States leads in sales, followed by Australia and France.

Top States:

  * England and California drive the most revenue across categories.

Top Markets:

  * APAC region dominates in sales, followed by EU and US.

Top Regions:

  * Central and South regions are top contributors to total sales.


💡 Regional segmentation highlights strong international performance, especially in APAC markets.


🚚 Order & Shipping Behavior

Weekday vs Weekend:

  * 88.6% of sales occur on weekdays; only 11.4% on weekends.

Shipping Speed Distribution:

  * Medium-speed shipping accounts for 59.4% of sales.

Profit vs Shipping Speed:

  * Medium and fast shipments tend to yield better profit outcomes.

Shipping Cost vs Profit:

  * Weak correlation overall, though some high-cost shipments lead to losses.

💡 Most customers prefer weekday orders and medium shipping, balancing cost and delivery time.



💸 Discount Impact Analysis

  * High Discounts (≥ 30%) lead to negative profit margins, despite:

  * Representing only 20.86% of products

  * Contributing 13.73% of total sales

⚠️ Aggressive discounting erodes profitability. Businesses should reevaluate discount thresholds and apply them more selectively.



🗂️ Category & Sub-Category Insights

Top Categories by Sales:

  * Technology

  * Furniture

  * Office Supplies

Top Sub-Categories:

  * Phones, Copiers, and Chairs lead sales.

Category Profitability:

  * Technology yields both the highest revenue and profit.

  * Furniture and Office Supplies generate significant revenue but lower profit margins.

💡 Technology remains the primary growth driver; furniture shows volume but thinner margins.


📦 Operational Insights

Order Priority vs Shipping Days:

  * Higher priority orders have shorter average shipping durations — confirming efficient fulfillment workflows.

Discount vs Shipping Cost:

  * No strong linear relationship; discounts and logistics costs appear independent.


🧠 Strategic Recommendations

  * Reduce Over-Discounting: Limit discounts >30% to avoid margin erosion.

  * Review Low-Profit SKUs: Audit pricing and supplier costs for loss-making items.

  * Capitalize on Repeat Customers: Leverage loyalty programs and personalized offers for the 100% returning customer base.

  * Optimize Shipping Strategy: Encourage medium-speed shipping options to balance speed and profitability.

  * Regional Targeting: Focus marketing and inventory on APAC and high-performing regions (England, California).

  * Technology Category Expansion: Increase assortment and marketing spend on tech products to maximize profit potential.


The business is performing well overall, with strong customer retention and consistent sales growth. However, tightening discount policies and optimizing underperforming products could unlock significant additional profit.












