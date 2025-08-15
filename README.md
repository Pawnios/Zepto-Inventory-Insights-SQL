# Zepto-Inventory-Insights-SQL
This project is a data analysis and business initiative focused on a fictional commerce company, similar to Zepto. The goal is to derive actionable insights from a SQL database containing data on orders, customers, and delivery partners. It replicates the typical workflow of a data analyst in the e-commerce or retail sector by using SQL to manage and analyze real-world product data. The focus is on building a robust inventory database, performing detailed exploratory analysis, cleaning inconsistent data, and extracting meaningful business insights.


# Key Tasks

1. Designed a structured SQL database from unrefined inventory data
2. Conducted EDA to examine product availability, pricing issues, and category distribution
3. Cleaned data by fixing nulls, removing faulty records, and converting prices from paise to rupees
4. Wrote insight-driven SQL queries to evaluate stock trends, revenue drivers, and pricing effectiveness

# Dataset Summary
The dataset, originally sourced from Kaggle and based on Zepto’s product listings, mirrors what analysts often face in real e-commerce systems. Each record represents a unique SKU (Stock Keeping Unit), with duplicate product names reflecting variations in size, weight, discounts, or packaging — a common scenario in online catalogs.

Key Columns:

sku_id – Synthetic primary key identifying each entry
name – Product title as displayed on the app
category – Classification such as Fruits, Snacks, or Beverages
mrp – Maximum Retail Price (converted from paise to ₹)
discountPercent – Discount percentage applied on MRP
discountedSellingPrice – Final selling price after applying discount
availableQuantity – Inventory count for the product
weightInGms – Weight of the product in grams
outOfStock – Boolean indicating stock status
quantity – Units per package (varies for loose and packed items)
