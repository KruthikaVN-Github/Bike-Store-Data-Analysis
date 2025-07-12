# 🚴 Bike Store Sales, Inventory & Customer Analysis using SQL

## 📌 Project Summary

This project explores the sales, inventory, and customer behavior of a multi-branch bike retail chain. Using structured SQL queries on a relational dataset of 9 interlinked tables, the analysis uncovers key patterns in customer loyalty, inventory distribution, and product performance.

The insights enable smarter inventory planning, personalized marketing, and customer retention strategies — making this a business-relevant, SQL-rich case study for retail analytics.

---

## 🧱 Dataset Overview

| Table Name       | Description |
|------------------|-------------|
| `brands`         | Brand information for each product |
| `categories`     | Product category classifications (e.g., Mountain, Electric) |
| `customers`      | Customer demographic data |
| `order_items`    | Transaction-level data, including product, quantity, and price |
| `orders`         | Order metadata such as order date and customer ID |
| `products`       | Product details, including brand, category, and model |
| `staffs`         | Sales personnel and their associated stores |
| `stocks`         | Store-wise inventory levels for each product |
| `stores`         | Physical store locations and related metadata |

---

## 🎯 Business Objectives

- Segment customers based on order behavior
- Analyze store-wise and category-wise inventory patterns
- Identify overstocked and understocked product lines
- Recommend strategies to improve inventory efficiency and customer retention

---

## 🔍 Key Insights

### 👥 Customer Loyalty & Behavior
- Most customers placed **only one order**, but a few (e.g., *Debra Burks, Kasha Todd*) placed **three or more orders**, indicating a **small but loyal customer segment**.

### 🛒 Stock Distribution by Store & Category
- **Cruisers Bicycles** had the **highest stock across all stores**, especially at *Rowlett Bikes* (1148 units), potentially signaling **overstocking**.
- **Cyclocross** and **Electric Bikes** consistently had **lowest inventory**, which may indicate **either high demand or understocking**.
- Stock patterns were generally consistent across stores, but **Santa Cruz Bikes** had more balanced inventory than others.

---

## 💡 Strategic Recommendations

### 1️⃣ Customer Retention

- **Identify & reward loyal customers** using order frequency — offer them exclusive discounts, loyalty rewards, or early product access.
- **Re-engage one-time buyers** with personalized promotions and product recommendations based on past purchases.

### 2️⃣ Inventory Optimization

- **Address potential overstocking** of Cruisers at Rowlett Bikes via:
  - Promotions or bundled offers
  - Inter-store transfers to high-demand locations
- **Investigate understocked categories** (Cyclocross & Electric Bikes):
  - Check if it's due to **supply chain issues or underestimated demand**
  - Consider raising **reorder points** and improving supplier collaboration
- **Implement dynamic inventory adjustments** based on real-time sales and lead times.

### 3️⃣ Operational Planning

- Align **staffing schedules with peak sales periods** using order date/time analysis.
- Use **seasonality trends** to proactively stock top-selling models.
- Launch **targeted marketing campaigns** aligned with product categories showing consistent high demand.

---

## 🧠 SQL Techniques Used

- Complex **multi-table joins** across 9 tables
- **Aggregate queries** for order counts, inventory totals
- **GROUP BY + HAVING** to extract top customers and stock extremes
- **CASE WHEN** for category-based classifications
- **Subqueries and filtering** for customized business logic

---

## 📊 Tools & Tech Stack

- **SQL**: SQLite (via Python), MySQL-compatible syntax
- **Python**: `pandas`, `sqlite3` for data handling and exploration
- **Visualization**: `matplotlib`, `seaborn` (for insights presentation)



