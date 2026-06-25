# 🛒 SuperStore Sales & Marketing Analytics  

**Author:** *Bhawna Kumari*  
**Tools Used:** Python, Pandas, Matplotlib, Seaborn    
**Objective:** To analyze e-commerce sales and marketing data to uncover trends, customer behavior, and actionable insights for business growth.

---

##  Project Overview  

This project explores the Global Superstore dataset to understand how the business performs across products, customers, markets, shipping operations, and profitability. Rather than focusing only on descriptive statistics, the analysis aims to answer practical business questions that could support strategic decision-making.

The project follows a typical data analytics workflow:
1. Data cleaning and preparation
2. Exploratory Data Analysis (EDA)
3. Business insight generation
4. Recommendations based on the findings

Python, Pandas, Matplotlib, and Seaborn were used throughout the analysis.

---

## Business Objective 

Retail businesses generate large amounts of transactional data every day. However, raw data alone does not explain what drives revenue, where profits are being lost, or which customers and products create the most value.

The objective of this project was to transform transactional sales data into meaningful business insights by answering questions such as:

- How much revenue and profit does the business generate?
- Which products contribute the most to sales and profit?
- Which products consistently lose money?
- Which customer segments are most valuable?
- Which markets and regions perform best?
- How do discounts affect profitability?
- Does shipping priority influence delivery performance?
- Are there patterns across time that can support planning?

---
## Data Preparation 

Before performing any analysis, the dataset was inspected for quality issues.

The preparation process included:

1. Checking data types
2. Identifying missing values
3. Removing duplicate records where necessary
4. Converting date columns into datetime format
5. Creating additional features such as shipping days and weekday/weekend classifications
6. Standardizing column names for easier analysis

This ensured the dataset was clean and suitable for further exploration

---

## Dataset Summary  

- **Total Records:** 25,035 orders  
- **Unique Customers:** 795  
- **Unique Products:** 10,292  
- **Time Period Covered:** Multi-year e-commerce transactions  
- **Key Columns:**  
  - Order ID, Order Date, Ship Date, Customer Name, Segment, Region, Market, Category, Sub-Category, Sales, Profit, Discount, Shipping Cost  


---

## 📈 Key Takeaways from the Analysis  

### **Overall Performance**
| Metric | Value |
|:-------|:------|
| **Total Sales** | **$12,642,905** |
| **Total Profit** | **$1,469,035** |
| **Profit Margin** | **11.62%** |
| **Average Order Value (AOV)** | **$505.01** |
| **Total Orders** | **25,035** |
| **Unique Customers** | **795** (100% repeat customers → excellent retention) |
| **Unique Products** | **10,292** |
| **Average Shipping Days** | **3.97 days** |

💡 *The business shows strong customer retention and consistent order volume, with a healthy overall profit margin.*

---

### 🏆 **Top Performers**

- **Top-Selling Products:**  
  - Top-selling products are dominated by Technology, especially smartphones.
  - Technology products clearly generate the largest share of revenue.
  - Furniture products such as executive leather armchairs also contribute significantly but         appear less frequently than technology products.
  - *“Apple Smart Phone, Full Size”* is the best-selling product.
    
<img width="1146" height="632" alt="image" src="https://github.com/user-attachments/assets/4efcdffe-db35-49bd-a87d-8690fb242ed3" />

---
  
- **Top-Profit Products:**  
  - *“Canon imageCLASS 2200 Advanced Copier”* yields the highest profit.
  - Interestingly, Apple Smart Phone is the highest-selling product but is not the highest-          profit product.
  - This shows that high sales do not necessarily produce high profits.
    
  <img width="1041" height="607" alt="image" src="https://github.com/user-attachments/assets/651d1120-1aa7-4969-8036-0e5cba8bf5aa" />

---

- **Top Customers by Sales:**
  
  *Sean Miller* lead in total sales.

**Business Insight**
The highest-value customers are concentrated mainly in
- US
- APAC
These customers contribute a significant share of overall revenue.
Such customers are ideal candidates for
- loyalty programs
- premium services
- personalized marketing
- account management
  
<img width="1043" height="623" alt="image" src="https://github.com/user-attachments/assets/96cd2888-7bc7-4aa3-83a9-34fb6480b1de" />

---
  
- **Top Customers by Profit:**
  
  *Tamara Chand* is the most profitable.

**Business Insight**
- This indicates that the customer generating the most revenue is not necessarily the most profitable. Differences in product mix, discounts, or costs can lead to this outcome.

  <img width="976" height="623" alt="image" src="https://github.com/user-attachments/assets/8c4583a9-44b2-4abc-8fba-210b43f72d8e" />

---

- **Most Frequently Sold Product:**

  - *Staples* dominates in quantity sold.
 
**Business Insight** 
- Customers bought Staples most often.
- Cheap office supplies usually appear here because people purchase them repeatedly.

<img width="1139" height="620" alt="image" src="https://github.com/user-attachments/assets/5cfcf8d8-aeec-42ed-b210-a2cb57e3cd53" />

---

### ⚠️ **Loss-Making Products**

- Products such as **“Cisco TelePresence System EX90 Videoconferencing Unit”**, high-end printers, and certain furniture items show **negative profits**.  
- These require review for **pricing**, **discount**, or **cost structure optimization**.

<img width="685" height="469" alt="image" src="https://github.com/user-attachments/assets/b6f18651-da14-406b-8639-b4df16bc323c" />

---

### 🌍 **Geographical Performance**
- **Top Countries:** 🇺🇸 USA → 🇦🇺 Australia → 🇫🇷 France
  
  <img width="1074" height="604" alt="image" src="https://github.com/user-attachments/assets/3b0556c3-9254-4ebf-96a0-9613867b6b43" />

- **Top States:** England and California
  
<img width="1481" height="678" alt="image" src="https://github.com/user-attachments/assets/4d48b72f-ce2a-43a1-951a-c5d6aea157b3" />

- **Top Markets:** APAC > EU > US
  
<img width="1033" height="604" alt="image" src="https://github.com/user-attachments/assets/85ce8ad5-6667-4418-a3e9-2521146cf3d7" />

- **Top Regions:** Central and South
   
<img width="945" height="669" alt="image" src="https://github.com/user-attachments/assets/bdab2395-d894-458a-85cb-116c92ee05d2" />


💡 *APAC and Central regions are driving revenue growth, indicating strong international demand.*

---

### 🚚 **Order & Shipping Behavior**
- **Weekdays vs Weekends:** 88.6% of sales occur on weekdays.

**Business insight**
- Most purchases occur on weekdays.
This could happen because
  - many customers are businesses
  - offices purchase during working days
    
  <img width="599" height="414" alt="image" src="https://github.com/user-attachments/assets/511341bd-7cdc-4dfd-be06-0c261f2a41b2" />

--- 

- **Shipping Speeds:**  
  - *Medium-speed shipping* → 59.4% of total sales.
 
<img width="554" height="397" alt="image" src="https://github.com/user-attachments/assets/e27b1b2a-2188-4c88-9a41-2160912a2b29" />

---

- **Shipping Speed vs Profit:**
  
  - Medium and fast deliveries correlate with higher profit margins.
 
 <img width="1016" height="601" alt="image" src="https://github.com/user-attachments/assets/85573d45-4d08-426e-b510-12dfa82dbd9f" />

---

- **Shipping Cost vs Profit:**
  
  - Weak correlation overall; some high-cost deliveries lead to losses.
  - Most orders
    - have small shipping costs
    - have profits around zero

- Only a few orders have
  - very high profit
  - very large loss
    
<img width="616" height="503" alt="image" src="https://github.com/user-attachments/assets/c62dce23-6fb1-4b46-850d-a81c1eeb9215" />


💡 *Optimizing shipping policies could further improve margins.*

---

###  **Discount Impact**

- **High Discounts (≥ 30%)** lead to **negative profit**, despite:  
  - Only 20.86% of products  
  - 13.73% of total sales
    
 <img width="620" height="510" alt="image" src="https://github.com/user-attachments/assets/0ac1bc64-56ad-4e4f-9228-f5f220e534bb" />
<img width="519" height="67" alt="image" src="https://github.com/user-attachments/assets/eb3c786b-63fb-4294-8dbc-a77e5852077e" />

⚠️ *Over-discounting directly erodes profitability.*

---

### 🗂️ **Category & Sub-Category Insights**

A. **Top Categories by Sales:**  
  1. Technology  
  2. Furniture  
  3. Office Supplies

<img width="557" height="424" alt="image" src="https://github.com/user-attachments/assets/3e45155a-24a6-471e-adeb-8928a38db9a6" />

B.  **Top Sub-Categories:**  

- Phones, Copiers, Chairs
- Phones are the strongest-selling sub-category.
  - Technology dominates again
 
<img width="930" height="611" alt="image" src="https://github.com/user-attachments/assets/76e15c36-0361-4c4a-844b-9554f0c3b1d3" />


C. **Profitability:**  

  - Technology → Highest sales & profit  
  - Furniture → High volume, lower margins
  - Office supplies -> Lowest sales, Higher profit than Furniture
    
<img width="988" height="588" alt="image" src="https://github.com/user-attachments/assets/489f9f8f-f437-4535-b66a-13cb62584589" />

💡 *Technology is the key growth driver. And Furniture has relatively weaker profitability.*

---

### 📦 **Operational Insights**

A. **Order Priority vs Shipping Days:**  

  - Higher-priority orders are delivered faster.
  - This indicates that the company's shipping process aligns with order urgency: critical orders are fulfilled quickest, while low-priority orders are intentionally allowed longer shipping times.

<img width="553" height="504" alt="image" src="https://github.com/user-attachments/assets/c2b41838-a848-49d4-9cdc-b3bba183efb7" />

B. **Discount vs Shipping Cost:**
  
  - No strong linear correlation — discounts appear independent of logistics costs.
    
<img width="556" height="505" alt="image" src="https://github.com/user-attachments/assets/a0ede2e1-2515-44cc-99d6-82b136bfd455" />

---

## 💡 Strategic Recommendations  

1. **Optimize Discount Policy** — Limit discounts >30% to prevent profit loss.  
2. **Audit Unprofitable Products** — Reevaluate pricing and supplier agreements.  
3. **Leverage Repeat Customers** — Launch loyalty programs and personalized offers.  
4. **Enhance Shipping Efficiency** — Focus on medium-speed deliveries for best ROI.  
5. **Regional Marketing Focus** — Invest more in APAC and top-performing states.  
6. **Expand Technology Category** — Promote and diversify top-performing tech SKUs.

---

## 🧠 Conclusion

The **SuperStore Sales Analysis** provides actionable insights into sales trends, customer retention, and profitability.

The company demonstrates **strong repeat customer behavior** and **robust sales performance**, but profitability can be further improved through **discount optimization, targeted regional focus, and category management.**

---

## 📂 Project Structure  

https://colab.research.google.com/drive/1VB0v6CB5Ad59pDLVuzsigbmXlLGrUYYN#scrollTo=LfZ8V0OP8iPQ
  











