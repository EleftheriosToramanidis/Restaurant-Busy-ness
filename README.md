---
title: "Database Reporting Project – Indian Food Delivery"
author: "Eleftherios (Leo) Toramanidis"
output: github_document
---

# Overview

This project builds a small management reporting system for a group of Indian
restaurants in the UK (London, Birmingham and Cambridge).  
The aim is to turn raw CSV order data into clear reports that support
data‑driven decisions about staffing, stock, menu design and promotions.

# Objectives

- Import and structure delivery order data in a relational database.
- Design SQL queries and reports for key business questions.
- Explain how each report can be used to improve profitability and service quality.

# Technologies

- Microsoft Access (primary implementation)
- SQLite (alternative implementation)
- SQL (joins, aggregation, grouping, filtering)
- CSV files as data sources

# Data Model

The database includes tables for:

- **Restaurants** – restaurant identifiers and locations.  
- **Customers / Deliveries** – customer and delivery grid references.  
- **Orders** – one row per order with restaurant and order date.  
- **OrderItems** – one row per item in an order, including product, quantity,
  price, category, spice level and vegetarian flag.

Foreign keys link orders to restaurants and items to orders so that demand can be
analysed by location, weekday and product.

# Reports

## 1. Busyness Report

Summarises, for each restaurant and day of the week:

- number of orders  
- number of items sold  
- total revenue  
- average order value  

**Business use**

- Align staffing with real demand (more staff on peak days, fewer on quiet days).  
- Plan stock and prep volumes to avoid stock‑outs and reduce waste.  
- Check whether busy days are genuinely profitable or dominated by low‑value orders.

## 2. Most Popular Items Report

Ranks menu items by total quantity sold, grouped by product and category, with
a minimum volume threshold to focus on meaningful sellers.

**Business use**

- Identify “hero” dishes to highlight on menus, websites and promotions.  
- Support purchasing and batch‑cooking plans around high‑volume items.  
- Flag low‑volume dishes for redesign, re‑pricing or removal to simplify operations.

## 3. Main Dish Bundle Recommendation Report

Analyses order lines to find items frequently bought together with each main
dish (e.g. sides and starters) and counts how often those combinations occur.

**Business use**

- Design evidence‑based bundles and meal deals around natural pairings.  
- Increase average order value through convenient recommendations on digital
  ordering platforms and by staff.  
- Adjust menu layout and pricing so high‑margin sides are presented as default pairings.

# Business Value

Together, the three reports provide a rounded view of:

- when customers order (demand patterns)  
- what they prefer (popular dishes)  
- how they build their meals (bundles)

Managers can use this toolkit to refine staffing, stock levels, menu content,
pricing and promotions in a coordinated way that supports higher revenue,
better cost control and an improved guest experience.

# How to Run

1. Import the CSV files into **MS Access** (or SQLite) following the schema above.  
2. Create SQL queries for the Busyness, Most Popular Items and Bundle reports.  
3. In Access, base formatted reports on these queries, with appropriate grouping
   and totals.  
4. Export reports to PDF or use them live for analysis and decision‑making.
