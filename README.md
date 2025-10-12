# 📊 Power BI Pizza Sales Dashboard

This project analyzes key performance indicators (KPIs) for pizza sales using Power BI. It provides business insights by visualizing sales data, top and bottom performing products, and sales trends. The dashboard and supporting queries are inspired by real-time business requirements for data-driven decision-making.

## Project Overview

- 🎯 **Objective**: Analyze pizza sales data for actionable business insights.
- **Tools Used**: Power BI for dashboard visualizations, SQL for data extraction and transformation.

## Dataset Used

- https://github.com/Joshnavi-pilli/Pizza-Sales-Dashboard/blob/main/pizza_sales_excel_file.xlsx

## Dashboard Previews

The dashboard includes:
- Total Revenue, Average Order Value, Total Pizzas Sold, Total Orders, Average Pizzas per Order
- Best and Worst Sellers by Revenue, Quantity, and Orders
- Daily and Monthly Trends
- Category & Size-based Sales Analysis

## 🖼️ Dashboard Snapshots

- ![Main Dashboard]https://github.com/Joshnavi-pilli/Pizza-Sales-Dashboard/blob/main/Screenshot%202025-05-13%20052445.png

<img width="862" height="485" alt="Screenshot 2025-05-13 053135" src="https://github.com/user-attachments/assets/457c2588-8045-4739-a0f3-4e270678609b" />

- ![Best/Worst Sellers]https://github.com/Joshnavi-pilli/Pizza-Sales-Dashboard/blob/main/Screenshot%202025-05-13%20053135.png

<img width="814" height="494" alt="Screenshot 2025-05-13 052445" src="https://github.com/user-attachments/assets/ffc97280-9c08-43e8-98b6-7e0c9de27641" />


## KPIs Tracked

1. **Total Revenue**: Sum of total price of all pizza orders.
2. **Average Order Value**: Total revenue divided by total number of orders.
3. **Total Pizzas Sold**: Total quantity of pizzas sold.
4. **Total Orders**: Number of orders placed.
5. **Average Pizzas Per Order**: Total pizzas sold divided by total orders.

## 📊 Charts & Visuals

- **Daily Trend for Total Orders**: Visualizes patterns in daily order volume.
- **Monthly Trend for Total Orders**: Shows monthly fluctuation in sales.
- **% Sales by Pizza Category/Size**: Pie charts showing market share by category and size.
- **Top/Bottom 5 Sellers**: Bar charts for best and worst-selling pizzas by revenue, quantity, and order count.
- **Funnel Chart**: Breakdown of pizzas sold by category.

## SQL Queries

Data used in the dashboard was extracted with the following example SQL scripts (`sql-queries-for-pizza_db.txt`):

- **Total Revenue**:  
  `SELECT SUM(total_price) AS total_revenue FROM pizza_sales`

- **Average Order Value**:  
  `SELECT SUM(total_price)/COUNT(DISTINCT order_id) AS avg_order_value FROM pizza_sales`

- **Total Pizzas Sold**:  
  `SELECT SUM(quantity) AS total_pizzas_sold FROM pizza_sales`

- **Top 5 Sellers by Revenue**:  
  `SELECT TOP 5 pizza_name, SUM(total_price) AS total_revenue FROM pizza_sales GROUP BY pizza_name ORDER BY total_revenue DESC`

- _See the full file for more queries and details._

## 🍕 Pizza Sales Report Summary (Jan 15 – Dec 15)

#Overall Performance:

- Total Revenue: ₹817.86K

- Total Orders: 21,350

- Total Pizzas Sold: 49,574

- Average Order Value: ₹38.31

- Average Pizzas per Order: 2.32

## 📅 Trends

- Busiest Days: Fridays and Saturdays show the highest sales and orders.

- Busiest Months: July and January record the highest total orders.

- Lowest Orders: Observed during October and December.

## 🍕 Sales Breakdown

-  Top Pizza Category: Classic pizzas — contribute the most to total sales and revenue.

- Top Pizza Size: Large pizzas account for the majority of sales (45.98%).

- Top Revenue Contributors:

- 1️⃣ Thai Chicken Pizza – highest revenue (43K)

- 2️⃣ Barbecue Chicken Pizza – strong sales (42K)

Top Quantity & Orders: Classic Deluxe Pizza leads in total orders and quantity sold.

## ⚠️ Lowest Performers

-  Lowest Revenue & Orders: Brie Carre Pizza contributes the least in both revenue and quantity.

- Other low sellers include Spinach Pizza and Mediterranean Pizza.

## 📈 Key Insights

Focus marketing and promotions on Classic and Large-size pizzas, especially Fridays, Saturdays, and summer months (July).

Review and potentially redesign or discontinue low-selling pizzas like Brie Carre and Spinach varieties.

Introduce combo deals or discounts during slow months (October–December) to balance sales.

## ✅ Conclusion

The business performs best with Classic large pizzas, particularly on weekends and mid-year months. Optimizing inventory and promotional efforts around these patterns can significantly boost sales and profitability.

## Usage

1. Clone/download this repository.
2. Open the `.pbix` file in Power BI Desktop.
3. Review included PNG/JPEG dashboard snapshots.
4. Inspect and adapt SQL queries in your own database environment.

## Project Credits

- Designed & implemented by Joshnavi Pilli
- Data & problem statement inspired by pizza retail datasets

---

_For more details, see included images and SQL script. Pull requests and suggestions welcome!_
