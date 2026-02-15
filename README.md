Database Reporting Project – Indian Food Delivery
This project builds a small management reporting system for a group of Indian restaurants in the UK (London, Birmingham and Cambridge). The goal is to turn raw order data in CSV format into clear, repeatable reports that support better operational and commercial decisions.

Objectives
Import and model delivery order data in a relational database.

Design SQL queries and reports that answer key business questions about demand, customer preferences and product combinations.

Explain how these reports can be used by managers to improve profitability and service quality.

Technologies Used
Microsoft Access (database, queries and formatted reports)

SQLite (alternative implementation of the same logic)

SQL (joins, aggregation, grouping, filters)

CSV data files as the input source

Data and Schema
The dataset contains records of:

Restaurants (location and identifier)

Customers and delivery locations

Orders and order dates

Order line items (menu item, quantity, price, spice level, vegetarian flag, etc.)

These tables are linked through primary and foreign keys so that orders and items can be analysed by restaurant, day of week and product.

Key Reports
1. Busyness Report
Summarises, for each restaurant and each day of the week:

Number of orders

Number of items sold

Total revenue

Average order value

This helps managers:

Align staffing levels with real demand (e.g. more staff on Fridays/Saturdays, fewer on quiet days).

Plan stock and prep volumes more accurately to avoid both stock‑outs and waste.

Decide whether busy days are truly profitable or dominated by low‑value orders.

2. Most Popular Items Report
Ranks menu items by total quantity sold, grouped by product and category, with a minimum volume threshold to focus on meaningful sellers.

Business uses include:

Identifying “hero” dishes to feature in menus, websites and promotions.

Supporting purchasing and batch‑cooking plans around high‑volume items.

Flagging under‑performing dishes that may need re‑pricing, redesign or removal from the menu.

3. Main Dish Bundle Recommendation Report
Analyses order lines to find items frequently bought together with each main dish (e.g. sides and starters), and counts how often those combinations occur.

This allows the business to:

Design evidence‑based bundles and meal deals that reflect what customers already order.

Increase average order value through convenient recommendations rather than hard selling.

Optimise menu layout and pricing so that high‑margin sides are presented as natural pairings for popular mains.

Business Benefits
Taken together, the three reports form a decision‑support toolkit that shows:

When customers order (busyness patterns).

What they prefer to eat (most popular items).

How they naturally compose their meals (bundle combinations).

Managers can use these insights to refine staffing levels, stock orders, menu content, pricing and promotions in a coordinated way that supports higher revenue, better cost control and an improved guest experience.

How to Run
Import the CSV files into MS Access (or SQLite) following the relational schema described above.

Create the queries corresponding to each report (Busyness, Most Popular Items, Main Dish Bundles).

In MS Access, build formatted reports based on those queries, grouping by restaurant and weekday or by product and category as required.

Export the reports to PDF or use them directly inside the database application for analysis and decision‑making.

Author
Eleftherios (Leo) Toramanidis – MSc Business Analytics, University of Bath.
