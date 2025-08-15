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

1. sku_id – Synthetic primary key identifying each entry
2. name – Product title as displayed on the app
3. category – Classification such as Fruits, Snacks, or Beverages
4. mrp – Maximum Retail Price (converted from paise to ₹)
5. discountPercent – Discount percentage applied on MRP
6. discountedSellingPrice – Final selling price after applying discount
7. availableQuantity – Inventory count for the product
8. weightInGms – Weight of the product in grams
9. outOfStock – Boolean indicating stock status
10. quantity – Units per package (varies for loose and packed items)

# Data Exploration
1. Assessed overall dataset structure and record count
2. Identified null values and reviewed unique product categories
3. Compared in-stock vs. out-of-stock items
4. Analyzed SKU duplications due to different package formats

# Data Cleaning
1. Removed entries with zero MRP or selling price
2. Standardized pricing by converting all monetary values from paise to ₹

📊 Business Insights
- Ranked top 10 best-value products based on highest discounts
- Highlighted out-of-stock items with high MRP
- Estimated revenue potential by product category
- Filtered high-cost products with low discounts
- Ranked categories offering highest average discounts
- Calculated price-per-gram to evaluate product value
- Categorized inventory into Low, Medium, and Bulk weight groups
- Computed total inventory weight per product category
