# Pizza_Sales_SQL_Project

# 🍕 Dominos Pizza Sales Analysis (SQL)

Hey there! Welcome to my SQL portfolio project. In this project, I took a bunch of raw transactional logs from a Dominos store setup and built an end-to-end relational database analysis. 

The goal here was simple: turn messy daily receipts into clear, actionable insights that can help a restaurant manager optimize their menu, prep ingredients better, and make smarter business choices.

---

## 🛠️ The Tech Stuff & Data Model
* **Database Engine:** MySQL
* **SQL Skills Used:** Schema design, multi-table joins, subqueries, group by aggregates, and advanced window functions (`RANK()`, `SUM() OVER()`).
* **How it connects:** The project links customer order data (`orders`, `orders_details`) with the master menu registries (`pizzas`, `pizza_types`) to give a full view of the business.

---

## 📂 Project Structure & Script Walkthrough

Everything is consolidated into a single, clean script: `dominos_sales_analysis.sql`. The queries are broken down into logical phases:

### 1️⃣ Setting Up the Environment
* Creating the database from scratch and building the core tables.
* Setting up primary keys and data types so the database runs smoothly and doesn't break when loading real data.

### 2️⃣ Answering the Basics (The Essential KPIs)
* Finding out exactly how many orders came through the door.
* Calculating the total revenue made across all pizza lines.
* Identifying the most expensive pizza on the menu and mapping out which size (Small, Medium, Large) customers actually order the most.

### 3️⃣ Digging Deeper (Operational Trends)
* **Menu Breakdown:** Pulling totals for each category (Classic, Veggie, Supreme, Chicken) to see what people love most.
* **Peak Hour Traffic:** Grouping orders by the hour of the day so the kitchen knows exactly when rush hour hits and how to schedule staff.
* **Daily Averages:** Using nested subqueries to calculate a reliable baseline of how many pizzas sell on an average day.

### 4️⃣ Advanced Business Intelligence (The Clever Queries)
* **Revenue Percentages:** Finding out exactly what percentage of total money comes from which pizza category.
* **Running Totals:** Using window functions to calculate cumulative revenue day-by-day, letting you see the business grow over time.
* **Top 3 per Category:** Using partition rankings to extract the top 3 highest-earning pizzas *inside* each specific category so we know our true heavy hitters.

---

## 💡 Real-World Takeaways

* **Smarter Staffing:** By finding the exact hours when orders spike, the store can save money on labor and reduce customer wait times.
* **Better Prep & Inventory:** Knowing which sizes and categories fly off the shelves means less wasted dough and fewer ingredient shortages.
* **Growth Tracking:** The cumulative revenue chart makes it easy to spot if sales are speeding up or slowing down over time.

---

## 🚀 How to check it out
1. Clone this repo to your machine.
2. Open it up in your favorite SQL editor (MySQL Workbench, DBeaver, or VS Code).
3. Run the script to see how the database initializes and queries the metrics!
