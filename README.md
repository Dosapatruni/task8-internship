# task8-internship
The objective of this task was to design a basic interactive dashboard that shows sales performance by product, region, and time (month/year) using the Superstore dataset. The goal was to create clean visuals, highlight top-performing areas, and extract meaningful insights.

⚙️ Steps I Followed
1. Data Preparation

Imported the Superstore Sales dataset (CSV) into Power BI.

Used Power Query for cleaning:

Removed extra unused columns (Unnamed: 16, Unnamed: 17).

Ensured correct data types (Order Date = Date, Sales & Profit = Decimal).

Created a Date Table using DAX to handle Year, Month, and Quarter analysis.

Built relationships between the Date Table and the Sales data.

2. DAX Measures Created

To analyze the data effectively, I created the following measures:

Total Sales

Total Profit

Orders (distinct count of Order ID)

Customers (distinct count of Customer ID)

Profit Margin %

AOV (Average Order Value)

Time-intelligence measures: Sales YTD, Sales QTD, Sales MTD, YoY Sales %, YoY Profit %.

Dynamic Dashboard Title that updates with slicers.

Top-N Sub-Category Sales measure with a What-if parameter to dynamically select Top 5, 10, etc.

3. Dashboard Design

The dashboard layout was divided into different sections:

Top KPIs (Cards)

Total Sales, Total Profit, Profit Margin %, Orders, Customers.

Visuals

Line Chart – Sales and Profit trends over time.

Clustered Bar Chart – Sales by Region.

Donut Chart – Sales by Category.

Top-N Sub-Category Bar – Dynamic view of best-performing sub-categories.

Map (Filled) – Sales distribution by State.

Filters & Slicers

Date, Region, Segment, Category, and Top-N parameter.

Formatting

Theme colors applied: Indigo (#4F46E5), Cyan (#06B6D4), Emerald (#10B981), Red (#EF4444), Amber (#F59E0B), Neutral shades (#E5E7EB, #94A3B8, #0B1220).

Font: Segoe UI (Report title 22–24, KPIs 36, labels 11–12).

Rounded corners (12–16px) and drop shadow for modern clean look.

4. Advanced Features

Dynamic Title automatically adjusts to Region/Category/Date slicers.

Report Page Tooltip for Sub-Category details (sales, profit margin, category share).

Sync Slicers across all visuals for consistent filtering.

Conditional Formatting on Profit KPIs (Green for positive, Red for negative).

🔍 Insights from Dashboard

West Region achieved the highest sales, while South Region lagged behind.

Technology Category dominated sales share, but Furniture showed lower profit margins.

Sales consistently peak during Q4 (Nov–Dec) across years.

Top 5 Sub-Categories contribute the majority of revenue, indicating high product concentration.
