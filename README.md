<h1>**🛒 Zepto Inventory Analysis using SQL**</h1>

**📌 Overview**<br>
This project focuses on analyzing Zepto’s inventory dataset using SQL to uncover actionable insights around pricing strategy, discount patterns, stock availability, and category-level performance.

The dataset consists of 3,732 products across multiple categories, where raw data was first structured into a relational table, followed by data validation, cleaning, and transformation (including handling invalid pricing and standardizing values from paise to rupees).

Through a combination of aggregations, filtering, and conditional logic, this project translates raw inventory data into meaningful business insights that can support decision-making in pricing, inventory management, and supply planning.

**📊 Dataset Summary**
<ul><li>Source: Kaggle – Zepto Inventory Dataset</li>
<li>Rows: 3,732</li>
<li>Columns: 9</li>
<li>Key Fields:</li>
<li>sku_id – Unique product identifier</li>
<li>category – Product category</li>
<li>name – Product name</li>
<li>mrp – Maximum Retail Price</li>
<li>discountPercent – Discount applied</li>
<li>discountedSellingPrice – Final selling price</li>
<li>availableQuantity – Units available</li>
<li>weightInGms – Product weight</li>
<li>outOfStock – Stock status</li></ul>

**🛠️ Tools & Skills Used**
<ul><li>SQL (PostgreSQL)</li>
<li>Data Cleaning & Transformation</li>
<li>Aggregations & Grouping</li>
<li>Conditional Logic (CASE WHEN)</li>
<li>Business-Oriented Analysis</li></ul>

**🔍 Project Workflow**
1. Data Exploration
<ul><li>Counted total records to validate dataset size</li>
<li>Checked for null values across all columns</li>
<li>Identified unique product categories</li>
<li>Analyzed stock distribution (in-stock vs out-of-stock)</li>
<li>Detected duplicate product names across SKUs</li></ul>

2. Data Cleaning
<ul><li>Removed invalid records where MRP = 0</li>
<li>Converted price fields from paise to rupees for accurate analysis</li>
<li>Ensured consistency across pricing columns</li></ul>

3. Key Business Analysis
<ul><li>Top Discounted Products (Max: 51%)</li>
Products like Dukes Waffy (Strawberry, Chocolate, Orange) offer the highest discounts at 51%, indicating aggressive pricing in the wafers/snacks segment.

<li>High MRP but Out of Stock (₹399 – ₹565)</li>
Products such as Patanjali Cow’s Ghee (₹565) and premium diaper SKUs are out of stock, highlighting potential missed revenue on high-value items.

<li>Top Revenue-Contributing Categories</li>
Cooking Essentials: ₹3,37,369
Munchies: ₹3,37,369
Paan Corner: ₹2,70,849
These categories dominate estimated revenue based on price × quantity.

<li>Highest Average Discount by Category</li>
Fruits & Vegetables: ~15.46%
Meats, Fish & Eggs: ~11.03%
Indicates that fresh/perishable categories rely more on discount-driven sales.

<li>Worst Price Efficiency (Highest ₹/gram)</li>
Products like Indulekha Bhringa Hair Oil (~₹3.67/g) rank among the least cost-efficient, showing pricing variation across categories.

<li>Inventory Weight Concentration</li>
Cooking Essentials: 1,404,654 g
Munchies: 1,404,654 g
Chocolates & Candies: 490,797 g
Inventory is heavily concentrated in a few categories, impacting storage and logistics planning.</ul>

**📈 Key Insights**
<ul><li>Duplicate Product Names Across SKUs</li>
Several products appear multiple times under different SKUs, indicating variations in pack sizes, weights, or packaging formats.

<li>Presence of High-Value Stockouts</li>
Multiple products priced above ₹300+ are out of stock, suggesting missed revenue opportunities in premium segments.

<li>Uneven Discount Distribution</li>
Discounts are not uniformly applied across categories, with some categories consistently offering higher average discounts, reflecting category-specific pricing strategies.

<li>Pricing Inefficiencies Identified</li>
Price-per-gram analysis highlights significant variation, where some products are disproportionately priced compared to their weight, indicating scope for pricing optimization.

<li>Inventory Skew Toward Select Categories</li>
A large portion of total inventory weight is concentrated in a few categories like Cooking Essentials and Munchies, which may impact warehouse space and supply chain planning.</ul>
