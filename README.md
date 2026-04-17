📊 Analysing Motorcycle Part Sales

📌 Project Overview

This project analyzes motorcycle part sales data to uncover trends in revenue generation, warehouse performance, and product demand. The goal is to generate actionable insights that can guide business decisions around inventory, logistics, and sales strategy.


🗂️ Dataset Description

The dataset contains transactional sales data with the following key fields:

* order_number – Unique identifier for each order
* date – Order date (June to August 2021)
* warehouse – Order fulfillment location (North, Central, West)
* client_type – Retail or Wholesale
* product_line – Category of motorcycle parts
* quantity – Number of items sold
* unit_price – Price per item
* total – Total order value
* payment – Payment method
* payment_fee – Fee percentage charged based on payment method


🎯 Objective

To analyze Wholesale transactions and determine:

* Net revenue generated
* Performance across product lines
* Monthly sales trends
* Warehouse-level performance


🧮 Methodology

* Filtered dataset to include only Wholesale transactions
* Aggregated data by:

  * Product line
  * Month
  * Warehouse
* Calculated net revenue using:

```sql
SUM(total) - SUM(payment_fee)
```

* Sorted results by:

  * Product line
  * Month (chronologically)
  * Net revenue (descending)


📈 Key Insights

🚀 Top Performing Product Lines

* Engine and Frame & Body generate the highest revenue
* These categories are major contributors to overall business performance


🏬 Warehouse Performance

* Central warehouse** consistently outperforms others across most categories
* West warehouse** shows the lowest performance and may require operational improvements


📅 Monthly Trends

* August records the highest revenue across multiple product lines
* Indicates a possible seasonal demand spike


🔄 Regional Demand Variation

* Sales performance varies significantly across warehouses
* Example: Electrical systems perform strongly in Central but poorly in West


⚙️ Stable Product Category

* Suspension & Traction shows consistent performance across all months and locations
* Represents a reliable revenue stream


📉 Low Impact Category

* Miscellaneous products generate the least revenue
* May require bundling or repositioning


💡 Business Recommendations

* Scale high-performing categories
  Focus on Engine and Frame & Body inventory and marketing

* Replicate Central warehouse strategy
  Apply successful practices to North and West locations

* Optimize West warehouse operations
  Improve inventory management and demand forecasting

* Leverage seasonal demand
  Increase stock and marketing efforts ahead of August

* Adopt regional inventory strategies
  Align stock levels with warehouse-specific demand patterns


🛠️ Tools Used

* SQL (PostgreSQL)
* Data aggregation & analysis techniques


📎 Conclusion

This analysis highlights key revenue drivers, regional performance gaps, and seasonal trends in motorcycle part sales. The insights can help improve operational efficiency, inventory planning, and revenue growth strategies.
