**🛒 Zepto Inventory Analysis using SQL**

**📌 Overview**
This project analyzes Zepto’s inventory dataset using SQL to uncover insights around pricing, discounts, stock availability, and category-level performance.
The focus is on real-world business questions such as identifying high-value products, estimating revenue, and understanding inventory distribution.

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
<li>Business-Oriented Analysis</li></ul>ul>

**🔍 Project Workflow**
1. Data Exploration
Counted total records to validate dataset size
Checked for null values across all columns
Identified unique product categories
Analyzed stock distribution (in-stock vs out-of-stock)
Detected duplicate product names across SKUs

2. Data Cleaning
Removed invalid records where MRP = 0
Converted price fields from paise to rupees for accurate analysis
Ensured consistency across pricing columns

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
<ul>Duplicate Product Names Across SKUs
Several products appear multiple times under different SKUs, indicating variations in pack sizes, weights, or packaging formats.

-Presence of High-Value Stockouts
Multiple products priced above ₹300+ are out of stock, suggesting missed revenue opportunities in premium segments.

-Uneven Discount Distribution
Discounts are not uniformly applied across categories, with some categories consistently offering higher average discounts, reflecting category-specific pricing strategies.

-Pricing Inefficiencies Identified
Price-per-gram analysis highlights significant variation, where some products are disproportionately priced compared to their weight, indicating scope for pricing optimization.

-Inventory Skew Toward Select Categories
A large portion of total inventory weight is concentrated in a few categories like Cooking Essentials and Munchies, which may impact warehouse space and supply chain planning.</ul>
