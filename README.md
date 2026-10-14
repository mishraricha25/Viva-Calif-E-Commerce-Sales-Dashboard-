# 🛍️ E-Commerce Sales Dashboard (Excel)

An interactive Excel dashboard that turns raw e-commerce order data into clear answers about sales trends, customer behaviour, product popularity, delivery speed and customer satisfaction.


## 📌 Project Overview

The business wants to understand how its online store is performing. This project cleans and prepares the order data, builds KPIs with PivotTables, and presents everything on a single-page dashboard so decision-makers can see the full picture at a glance.

**Tools used:** Microsoft Excel (Tables, Formulas, PivotTables, PivotCharts, Slicers, Dashboard formatting)

---

### Workbook sheets

| Sheet | Purpose |
|---|---|
| **Data** | Raw order data (2,400 rows) stored as an Excel Table named `orders` |
| **Questions & KPIs** | List of KPIs and business questions answered |
| **Dashboard** | Final visual report |
---

## 🗃️ Dataset

2,400 orders placed between **1 Jan 2025 and 29 Mar 2025** (13 weeks), for **20 products** sold through **5 order channels** to customers across **California counties**.

| Column | Description |
|---|---|
| TX ID | Unique transaction / order ID |
| Product | Product purchased (e.g. Shorts, Sneakers, Hoodies & Sweatshirts) |
| Quantity | Units ordered |
| Unit Price | Price per unit |
| Amount | Quantity × Unit Price |
| Order Date | Date the order was placed |
| Ship Date | Date the order was shipped |
| Customer Gender | M / F / O (some values are blank) |
| Order Mode | App, Website, Target.com, Instagram, Partner App |
| Rating | Customer rating (1–5) |
| State / County | Customer location |

### ➕ Columns I added (calculated)

| Column | Formula | Why |
|---|---|---|
| **Days to Deliver** | `=[@[Ship Date]]-[@[Order Date]]` | Measures how long it takes to ship an order |
| **Weeknum** | `=WEEKNUM([@[Order Date]])` | Groups orders by week for the 13-week trend |
| **Gender Value** | Formula that converts the gender code (M / F / O / blank) into a readable label | Gives a clean category for the gender split chart |

---

## 📊 KPIs

- **Total Orders**
- **Total Quantity**
- **Total Amount** (revenue)
- **Avg. Rating**
- **Avg. Days to Deliver**

## ❓ Business Questions Answered

| # | Question | Visual |
|---|---|---|
| 1 | Trend in the last 13 weeks | Line chart by week number |
| 2 | How our customers like to buy | Orders by order mode |
| 3 | How many they buy? | Orders by quantity |
| 4 | Which products are popular? | Top products bar chart |
| 5 | Overall gender split | Donut / pie chart |
| 6 | Where do our customers live? | Orders by county |
| 7 | How long we take to ship the orders | Distribution of days to deliver |
| 8 | How happy are our customers? | Ratings distribution |

---
## 🔍 Key Insights

- **Revenue:** ~$649K from 2,400 orders; average order value $270; average rating 3.96; average delivery 2.3 days.
- **Trend:** February was the strongest month per day; Wednesday is the best sales day (~19% of revenue). Week 1 is a partial week (1–4 Jan).
- **Products:** Sneakers (19.7%) and Jeans (17.4%) drive over a third of revenue; T-Shirts have the most orders but lower revenue.
- **Bulk buying:** Orders of 10+ units are only 12% of orders but 41% of revenue.
- **Channels:** App leads (35% of revenue); Instagram has the highest average order value ($295) and best rating.
- **Customers:** Women place 51% of orders and spend more per order than men.
- **Geography:** Los Angeles County alone is 33% of revenue; the top 5 counties give 65%.
- **Delivery:** 67% of orders ship within 2 days; delivery time shows almost no effect on ratings.
- **Satisfaction:** 73% of customers give 4–5 stars.

---

## 🛠️ How I Built It

1. **Prepared the data**: converted the range into an Excel Table (`orders`) and added Days to Deliver, Weeknum and Gender Value.
2. **Built KPIs** using PivotTables / formulas on the `Questions & KPIs` sheet.
3. **Created one PivotTable + PivotChart per question.**
4. **Designed the dashboard**: arranged charts and KPI cards, applied the brand colour palette and logo, and removed gridlines.
5. **Added slicers** (if used) to filter all charts together.

---


Aspiring Data Analyst | Excel · SQL · Power BI

🔗 [LinkedIn](https://www.linkedin.com/) · 💻 [GitHub](https://github.com/)
