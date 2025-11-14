# E-Commerce-Sales-Dashboard
📘**Project Overview​**

The E‑Commerce Sales Dashboard is an interactive Power BI report that provides a comprehensive view of sales amount, profit, quantity, and AOV with drill‑downs by state, category, sub‑category, customer, and payment mode.​
It enables quick decision‑making by revealing trends, top drivers, and areas of margin risk in a clean, actionable layout.​

🎯 **Objective​**

Analyze overall sales and profitability across months, regions, and product mix to support marketing and supply decisions.​
Identify high‑value customers and sub‑categories, track discount impact on profit, and monitor seasonal peaks/dips.​

📊**Key Performance Indicators (KPIs)​**

**Total Sales (Amount)** = SUM(Orders[Sales]) — headline KPI card.​
**Average Order Value (AOV)** = DIVIDE([Total Sales],[Total Orders]).​
**Total Profit =** SUM(Orders[Profit]) and Profit Margin = DIVIDE([Total Profit],[Total Sales]).​
**Total Orders =** DISTINCTCOUNT(Orders[Order ID]) and Total Quantity = SUM(Orders[Quantity]).​

📈**Dashboard Insights​**

**Monthly Trend:** Profit by Month chart shows clear seasonality with a few negative months indicating margin erosion requiring pricing/discount review.​
**State Performance:** Maharashtra and nearby states lead Sales Amount among available states, highlighting regional concentration.​
**Product Mix:** Sub‑Category bar shows items like Printers and Bookcases as top profit drivers in the sample, while others trail.​
**Customer & Payment:**Top customers contribute outsized revenue; payment mode share from the donut chart guides checkout optimization.​

🧮**Data Model & Source​**

**Star schema:** Fact Orders with dimensions Date, Product/Category, Geography (State/City), and Customer; relationships on Date and keys as appropriate.​
**Data Source:** <Excel/CSV e‑commerce dataset link>; key fields include Order ID, Order Date, State, Category, Sub‑Category, Quantity, Sales, Discount, Profit, Customer, and Payment Mode; sample/public data with no PII.​
**Transformations:**
Cleaned and standardized data using Power Query
Created calculated columns and DAX measures for KPIs
Applied data modeling for relationships across dimensions

⚙️**Tools & Technologies**

**Power BI Desktop**– Data visualization and dashboard creation
**Power Query Editor** – Data transformation and cleaning
**DAX (Data Analysis Expressions)** – Calculations and custom measures
**Microsoft Excel**– Raw data source

📉**Visual Components​**

**KPI Cards:** Sales Amount, AOV, Profit, Quantity to summarize performance at a glance.​
**Line/Column Chart:** Profit or Sales by Month to reveal trend and seasonality.​
**Bar Charts**: Amount by State; Profit by Sub‑Category to compare regions and product drivers.​
**Donut Charts**: Quantity share by Category and by Payment Mode to show mix.​
**Slicers:** Quarter and State filters for quick focus and exploration.​
