# Zepto PostgreSQL Analysis

## Project Overview
This project analyzes Zepto product data using PostgreSQL to provide insights into product SKUs, pricing, inventory status, and category-wise revenue. It demonstrates data validation, cleaning, and business-level analysis using SQL queries.

## Tools Used
- PostgreSQL
- pgAdmin
- SQL

## Dataset
- The full dataset used in this project contains **over 3,000 product records**.
- Columns include:
  - `sku_id` – Unique identifier for each SKU
  - `category` – Product category
  - `name` – Product name
  - `mrp` – Maximum retail price
  - `discount_percent` – Discount percentage
  - `availabale_quantity` – Quantity available
  - `discounted_selling_price` – Selling price after discount
  - `weight_in_grams` – Product weight
  - `out_of_stock` – Product availability (TRUE/FALSE)
  - `quantity` –
 
  - ## SQL File Structure
- **01_table_creation.sql** – Creates the `Zepto` table
- **02_data_quality_checks.sql** – Validates data for NULLs, duplicates, and distribution
- **03_data_cleaning.sql** – Cleans zero-price records and standardizes prices
- **04_business_analysis.sql** – Performs analysis to generate business insights

## Key Analysis & Insights
1. **Duplicate SKUs:** Identified products with multiple SKUs to understand variant distribution.
2. **Top Discounts:** Highlighted top 10 best-value products by discount percentage.
3. **Inventory Status:** Checked out-of-stock products and high-priced items.
4. **Revenue Analysis:** Calculated category-wise revenue to identify top-performing categories.

## Query Output Screenshots
- **Table Overview:** ![Table Overview](screenshots/01_table_overview.png)
- **Duplicate SKU Analysis:** ![Duplicate SKU Analysis](screenshots/02_duplicate_skus.png)
- **Top Discounted Products:** ![Top Discounts](screenshots/03_top_discounts.png)
- **Category-wise Revenue:** ![Category Revenue](screenshots/04_category_revenue.png)

## How to Reproduce
1. Clone this repository:
```bash
git clone https://github.com/yourusername/zepto-postgresql-analysis.git
