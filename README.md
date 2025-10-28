# FMCG-Analytics


## Project Overview  
This Power BI dashboard delivers **actionable, data-driven insights** for an FMCG business, enabling stakeholders to monitor sales performance, customer behavior, product trends, and time-based KPIs across regions and categories. Built with a clean, interactive design, it supports strategic decision-making in a competitive retail and distribution environment.

The dashboard consolidates data from **Sales, Products, Customers, Date, and Geography** tables into a semantic model, leveraging **DAX measures**, **dynamic visuals**, and **smart filtering** for intuitive exploration.

---

## Live Report Link  
\https://app.powerbi.com/reportEmbed?reportId=6c3e1a38-caf0-4d68-84c7-07cc907282d7&autoAuth=true&ctid=6627360e-a7aa-4e24-bd88-a75fbc42bc55

---

## Tools Used  
- **Excel** – Primary data source and initial exploration  
- **Power BI Desktop** – Data modeling, DAX, visualization, and report design  
- **DAX (Data Analysis Expressions)** – Core calculations and time intelligence  
- **Power Query (M Language)** – Data transformation, cleaning, and date table creation  

---

## Power BI Techniques Implemented  

| Technique | Usage |
|--------|-------|
| **Calculated Measures (DAX)** | Dynamic KPIs like MTD/QTD/YTD, YoY Growth, Last 3 Months Sales |
| **Time Intelligence** | `DATESMTD`, `DATESQTD`, `DATESYTD`, `SAMEPERIODLASTYEAR`, `DATESINPERIOD` |
| **Disconnected Slicer Table** | Unified Time Period slicer (MTD/QTD/YTD/Last 3 Months) using `SWITCH` |
| **Slicers & Cross-Filtering** | Region, Product Category, Loyalty Status, Date Range |
| **Responsive Layout** | Optimized for desktop and mobile (Fit to Page) |

---


---

## Dashboard Structure  

### 1. **Executive Summary**  
- **KPI Cards**: Total Sales, YoY Growth, CLV, Inventory Turnover  
- **Line Chart**: Sales Trend Over Time  
- **Gauge**: Current vs. Target Sales  

### 2. **Sales Analysis**  
- **Clustered Column**: Sales by Category & Region  
- **Top 10 Products Bar Chart**  
- **YoY Growth Area Chart**  
- **Detailed Sales Matrix**  

### 3. **Customer Analysis**  
- **Donut**: Loyalty Status Distribution  
- **Scatter**: Spend vs. Visit Frequency  
- **Stacked Bar**: New vs. Returning Customers  
- **Customer Segmentation Matrix**  

### *(Optional)* **Branch Performance**  
- **Map Visual**: Revenue by Location  
- **Branch Sales KPIs**  

---

## Domain Knowledge (FMCG Context)  

| Area | Key Concepts Covered |
|------|------------------------|
| **Sales** | Regional performance, category contribution, top SKUs |
| **Customer** | Loyalty tiers, acquisition vs. retention, lifetime value |
| **Product** | Inventory turnover, fast vs. slow movers |
| **Time Analysis** | MTD/QTD/YTD, rolling 3-month trends, YoY comparison |

---

## Business Terms Used  

- **MTD / QTD / YTD** – Month/Quarter/Year to Date  
- **YoY Growth** – Year-over-Year percentage change  
- **Customer Lifetime Value (CLV)** – Total spend per customer  
- **Inventory Turnover** – Sales efficiency relative to stock  
- **New vs. Returning Customers** – Acquisition & retention tracking  

---

## Company’s Background: NovaMart Consumer Goods  
**NovaMart Consumer Goods** is a fast-growing FMCG company operating in the packaged food, personal care, and household essentials space. With a strong presence across urban and semi-urban markets in multiple regions, NovaMart distributes its products through modern trade (supermarkets), general trade (kirana stores), and e-commerce platforms. Facing increasing competition and margin pressure, the company is leveraging data analytics for the first time to optimize inventory, boost customer retention, and drive sales efficiency across channels.

---

## Importing Data into Power BI  
Data is sourced from **Excel workbooks** containing structured tables:  
`Sales`, `Products`, `Customers`, `Date`, `Geography`  

All files are imported via **Power Query**, transformed, and

## Importing Data into Power BI  
Data is sourced from **Excel workbooks** containing structured tables:  
`Sales`, `Products`, `Customers`, `Date`, `Geography`  

All files are imported via **Power Query**, transformed, and loaded into the model.  

**Relationships established via**:  
- `Sales[ProductID]` → `Products[ProductID]`  
- `Sales[CustomerID]` → `Customers[CustomerID]`  
- `Sales[Date]` → `Date[Date]`  
- `Sales[RegionID]` → `Geography[RegionID]`  
## Dashboard Navigation  

- **Slicers**:  
  - Region  
  - Category  
  - Loyalty  
  - Unified Time Period  

- **Bookmarks**:  
  - Drill to product details  
  - Reset filters   

---

**Ready to deploy?**  
**Publish to Power BI Service** → **Create App** → **Share with stakeholders.**
