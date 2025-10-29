# Coffee Vending Machine Sales Analysis

This project is a dynamic sales dashboard built in Tableau. It analyzes transaction data from a coffee vending machine to identify sales trends, peak usage times, and product popularity.

---

## 📈 Project Objective

The goal of this dashboard is to provide a clear, interactive, and actionable overview of the vending machine's performance. It aims to answer key business questions:

* **What** are our top-selling and worst-selling products?
* **When** is the machine busiest (by hour and day of the week)?
* **How** are sales trending over time?
* **What** is the preferred payment method?

---

## 💾 Data Source

The data for this project came from two separate `.csv` files:
* `index_1.csv`
* `index_2.csv`

In Tableau, these files were combined using a **Union** to create a single, unified dataset for analysis.

**Data Preparation:**
* **Union:** Combined the two data files.
* **Calculated Fields:**
    * `Hour of Day`: Extracted the hour from the `datetime` field.
    * `Day of Week`: Extracted the weekday name from the `date` field.
    * `Total Items Sold`: Created from the `Number of Records` field.
    * `Avg. Price per Item`: `SUM([Total Sales]) / SUM([Total Items Sold])`

---

## 🛠️ Tools Used

* **Tableau Desktop:** Used for data connection, preparation, visualization, and dashboard creation.

---

## 📊 Dashboard Features

The final dashboard consists of several interactive components:

### Key Performance Indicators (KPIs)
A top-level banner displays the most important metrics:
* **Total Sales:** Total revenue from all transactions.
* **Total Items Sold:** Total number of products sold.
* **Avg. Price per Item:** The average revenue per item.

### Visualizations
1.  **Sales Over Time:** A line chart showing `Total Sales` by `date`.
2.  **Peak Hours Heatmap:** A grid showing `Total Items Sold` by `Day of Week` and `Hour of Day`.
3.  **Top Selling Products:** A horizontal bar chart ranking each `coffee_name` by `Total Sales`.
4.  **Payment Type:** A pie chart showing the breakdown of transactions by `cash_type`.

---

## 💡 How to Use This Dashboard

This dashboard is fully interactive.

* **Click any square on the Heatmap** (e.g., "Monday" at "8 AM") to filter the *entire* dashboard to show data for only that specific time block.
* **Click a slice on the Pie Chart** (e.g., "card") to filter the *entire* dashboard to show data for only that payment type.
* **Click any bar** on the `Top Selling Products` chart to see trends for just that item.

Clicking the same item again (or clicking in the white space) will clear the filter.

---

## 🔗 Live Dashboard

*[Optional: Insert the link to your Tableau Public dashboard here]*
