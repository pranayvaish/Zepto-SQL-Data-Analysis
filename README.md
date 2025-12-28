# Zepto SQL Data Analysis Project

This project performs **data exploration, cleaning, and analysis** on a grocery delivery dataset inspired by **Zepto** using **SQL (PostgreSQL)**.  
The goal is to extract meaningful business insights related to pricing, discounts, inventory, and revenue.

---

## Project Overview

The dataset contains product-level information such as:
- Category
- Product name
- MRP
- Discount percentage
- Selling price
- Available quantity
- Weight
- Stock status

Using SQL queries, we analyze product availability, pricing strategies, discounts, and inventory distribution.

---

## Table Structure

```sql
CREATE TABLE zepto (
    sku_id SERIAL PRIMARY KEY,
    category VARCHAR(120),
    name VARCHAR(150) NOT NULL,
    mrp NUMERIC(8,2),
    discountPercent NUMERIC(5,2),
    availableQuantity INTEGER,
    discountedSellingPrice NUMERIC(8,2),
    weightInGms INTEGER,
    outOfStock BOOLEAN,
    quantity INTEGER
);
