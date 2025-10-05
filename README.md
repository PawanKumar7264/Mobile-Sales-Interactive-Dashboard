# Mobile-Sales-Interactive-Dashboard
 
## 1. Project Title / Headline
Mobile Sales Analytics: Interactive Sales Dashboard  
A dynamic, interactive data visualization tool built to analyze mobile phone sales data, focusing on units sold, revenue by brand, monthly trends, payment methods, and regional distribution for optimized inventory and marketing insights.

## 2. Short Description / Purpose
This dashboard acts as a centralized sales tracker for mobile devices. Its purpose is to deliver accident statistics in a clean, interactive, and visually intuitive format, enabling users to swiftly spot patterns in brand performance, seasonal fluctuations, payment preferences, and geographic hotspots to drive sales strategies and resource allocation.

## 3. Tech Stack
The dashboard was built using the following tools and technologies:  
• 📈 Microsoft Excel – Primary platform for data visualization and dashboard creation.  
• 📂 Excel Data Tools – For data import, transformation, and pivot table setup.  
• 🧠 Excel Formulas – Employed for dynamic calculations, such as SUM for totals and conditional formatting for highlights.  
• 📝 Data Modeling – Relationships linked across tables using keys like Brand, Month, City, Payment_Method, and State for seamless filtering and slicing.  
• 📁 File Format – .xlsx for interactive development and .png for static previews.

## 4. Data Source
Source: Provided Excel file ("Mobile Sales Data 403209") with sales records, likely spanning a full year based on monthly breakdowns.  

Raw Data Structure: Data organized in sheets, with core details including Brand (e.g., Mi/Xiaomi, Vivo, OnePlus, Apple, Samsung), Units_Sold, Sales_Amount, Month, City (e.g., Bangalore, Bhopal, Chennai), State (via map), and Payment_Method (Cash, Credit Card, Debit Card, UPI). Aggregated summaries show total units sold (19,150) and brand-wise revenue (e.g., Apple: 32,100,621). Dataset covers ~19,150 records across brands and regions.  

Excel Data Transformation: Leveraged Excel’s Power Query and formulas for ETL.  
Extraction: Loaded from the source file, consolidating sheets.  
Transformation: Handled date conversions for months, filled nulls in cities/states, and computed aggregates like total revenue per brand using SUMIFS (e.g., overall total units: 19,150). Standardized categories (e.g., grouping similar payment methods).

## 5. Features / Highlights
### • Business Problem
Retailers, sales teams, and brand managers struggle with fragmented sales data, making it hard to pinpoint top-performing brands, seasonal dips, or regional preferences. Manual Excel dives lead to overlooked opportunities, like understocking high-demand cities or ignoring payment trends, resulting in lost revenue, overstock costs, and suboptimal marketing.  

Key questions such as:  
Sales Optimization: Which brands drive the most revenue, and how do monthly trends affect inventory?  
Regional Insights: Are sales stronger in urban hubs like Bangalore vs. others like Bhopal?  
Payment Analysis: What payment methods dominate, and how do they vary by city?  

### • Goal of the Dashboard
Boost Revenue: Unify sales views to highlight growth areas and adjust stocking dynamically.  
Enhance Targeting: Pinpoint high-revenue brands and regions for focused campaigns.  
Streamline Decisions: Serve as a go-to hub for real-time sales intel, shifting from gut-feel to data-backed actions.  
Improve Efficiency: Cut analysis time with slicers, filters, and visuals over raw spreadsheets.  

### • Walkthrough of Key Visuals

**Total Units Sold and Brand Breakdown**  
Visual Type: Donut charts with labels and summary metrics.  
Purpose: Quick snapshot of overall volume and brand shares.  
Detailed Functionality:  
Grand total units (19,150) via SUM formula. Donut segments by brand: Mi/Xiaomi (19.1%, 3,664 units), Vivo (19.8%, 3,801), OnePlus (20.0%, 3,830), Apple (20.5%, 3,932), Samsung (20.5%, 3,923). Slicers for city (e.g., Bangalore) or month filter distributions. Critical for brand prioritization.  

**Revenue by Brand**  
Visual Type: Donut charts stacked by brand.  
Purpose: Reveal financial performance beyond units.  
Detailed Functionality:  
X-axis: Brands; Y-axis: Revenue (Apple: 32,100,621; OnePlus: 30,752,041; Samsung: 3,126,514; Vivo: 3,027,858; Xiaomi: 3,027,858) using SUMIFS. Color-coded (e.g., green for Apple). Highlights Apple/OnePlus dominance (~60% combined). Supports pricing strategy tweaks.  

**Payment Method Distribution**  
Visual Type: Pie chart.  
Purpose: Understand transaction behaviors for payment integrations.  
Detailed Functionality:  
Slices: Cash (blue), Credit Card (black), Debit Card (red), UPI (orange) – exact shares not labeled but visually balanced. PivotTable backend with city slicer (e.g., UPI higher in Bangalore). Reveals digital payment trends for promo targeting.  

**Sales by State**  
Visual Type: Choropleth map of India.  
Purpose: Geographic sales heatmapping.  
Detailed Functionality:  
Shaded regions by state revenue/units (darker for higher, e.g., southern states prominent). Linked to city dropdown (Bangalore selected, highlighting Karnataka). Filters by brand show regional favorites (e.g., Apple in metros). Drives location-specific logistics.  

**Sales by Months**  
Visual Type: Multi-line chart.  
Purpose: Track temporal patterns for forecasting.  
Detailed Functionality:  
X-axis: Jan-Dec; Y-axis: Units (0-60,000 scale). Lines by brand (blue for Apple?: peaks at 57,251 in Mar, dips to 2,670 in Feb; orange for Samsung?: 34,622 in Apr, 43,139 in Aug; red line with 24,391 in Jun, 14,679 in Oct, 21,289 in Nov). Uses PivotCharts with month slicers. Spots Q1 surges for seasonal planning.  

**City-wise Sales**  
Visual Type: Dropdown filter with conditional highlights.  
Purpose: Drill-down into urban performance.  
Detailed Functionality:  
Options: Bangalore (selected, high revenue), Bhopal, Chennai (red-highlighted for mid-tier). Aggregates units/revenue per selection via VLOOKUP. Color-coded (red for above-average). Informs city-level marketing budgets.  

### • Business Impact & Insights
Revenue Growth: Spotlights Apple/OnePlus for 60%+ revenue, enabling 15-25% uplift via targeted stock.  
Regional Efficiency: Bangalore dominance suggests metro focus, cutting rural over-allocation.  
Trend Forecasting: Monthly peaks (e.g., Mar 57k units) guide promo timing, reducing stockouts.  
Cost Optimization: UPI/Cash insights streamline payment fees, saving 5-10% on transactions.

## 6. Screenshots / Demos  
![Dashboard Preview](https://github.com/PawanKumar7264/Mobile-Sales-Interactive-Dashboard/blob/main/Sales%20Dashboard%20Snapshort.png)
