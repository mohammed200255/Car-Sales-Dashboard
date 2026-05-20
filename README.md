# 🚗 Interactive Car Sales Analytics Dashboard — Power BI

## Project Overview

This project transforms raw Excel car sales data into a fully interactive, multi-page analytics dashboard built in Power BI. It covers the complete data lifecycle — from ingestion and cleaning through to strategic business insights — empowering sales teams and management to monitor performance in real time and make data-driven decisions.

The dashboard consists of two dedicated pages: a high-level **Dashboard** view and a drill-down **Details** view, connected by intelligent navigation buttons.

---

## Data Pipeline & Modeling

Raw Excel data was imported and processed using **Power Query**, where it was cleaned, shaped, and structured into an integrated relational data model. This foundation ensures consistency across all measures and enables reliable cross-filtering between visuals.

---

## Key Performance Indicators (KPIs)

Six headline KPI cards sit at the top of both pages, providing an at-a-glance performance summary at all times:

| KPI | Value | YoY Change |
|---|---|---|
| **YTD Total Sales** | $371M | +$71M (+23.59%) ✅ |
| **MTD Total Sales** | $54.28M | — |
| **YTD AVG Price** | $28K | -223.48 (-0.79%) 🔴 |
| **MTD AVG Price** | $28.26K | — |
| **YTD Cars Sold** | 13K | +2.62K (+24.57%) ✅ |
| **MTD Cars Sold** | 2K | — |

The **smart color-coding system** dynamically renders YoY differences in green (positive) or red (negative), giving users an instant signal of performance direction without reading the numbers.

### DAX Measures Engineered

- **Year-to-Date (YTD)** sales, average price, and units sold — with automatic year-over-year delta calculations
- **Month-to-Date (MTD)** equivalents for real-time monthly tracking
- **%GT YTD Cars Sold** — each company's or product's percentage contribution to total units sold
- Conditional formatting logic driving the color-coding system

---

## Dashboard Page

The main Dashboard page provides a strategic overview through five key visualizations:

### 📈 Sum of Price by Week
A line chart tracking weekly revenue across ~50 weeks, revealing a clear upward growth trend in the first half of the year followed by fluctuation and mid-year softening.

### 🎨 YTD Total Sales by Color
A donut chart breaking down sales by vehicle color:
- **Pale White** — $175M (47.0%) — largest segment
- **Black** — $125M (33.7%)
- **Red** — $71M (19.2%)

> While Pale White leads by volume, Black vehicles punch above their weight in average transaction value.

### 🚙 YTD Total Sales by Body Style
A donut chart showing body style distribution:
- **SUV** — $100M (26.9%) — most demanded style
- **Hatchback** — $83M (22.3%)
- **Sedan** — $74M (19.9%)
- **Passenger** — $63M (17.1%)
- **Hardtop** — $51M (13.8%)

### 🗺️ YTD Cars Sold by Dealer Region
An interactive Bing map displaying regional bubble sizes proportional to units sold. **Middletown** and **Aurora** are the standout top-performing regions, with additional activity in Pasco, Janesville, Scottsdale, Austin, and Greenville.

### 👥 Top 8 Customers by Sales
A horizontal bar chart ranking individual customers by total spend:

| Rank | Customer | Sales |
|---|---|---|
| 1 | Emma | $2.80M |
| 2 | Lucas | $2.64M |
| 3 | Thomas | $2.55M |
| 4 | Alexis | $2.19M |
| 5 | Lea | $2.13M |
| 6 | Chloe | $2.03M |
| 7 | Nathan | $2.01M |
| 8 | Paul | $1.98M |

### 🏢 Company Performance Table
A summary matrix showing each brand's YTD AVG Price, YTD Cars Sold, and %GT YTD Cars Sold with inline bar charts. Top brands by unit volume include **Chevrolet (7.87%)**, **Ford (6.68%)**, **Dodge (7.16%)**, and **Chrysler (4.66%)**.

---

## Details Page

The Details page provides granular drill-down capability into individual vehicle records, filterable by:

- **Body Style**
- **Engine**
- **Model**
- **Dealer Name**

The main visual is a sortable data table showing every vehicle record with columns for Company, Body Style, Model, Color, YTD AVG Price, and %GT YTD Cars Sold (with inline bar charts). The table is sorted by YTD AVG Price descending, with premium vehicles (Lincoln Continental, Toyota Tacoma, Volvo C70) at $82K+ leading the list.

---

## Interactive Features

- **Navigation buttons** — one-click switching between Dashboard and Details pages
- **Cross-filtering** — clicking any visual filters all others on the page simultaneously
- **Filter slicers** — Body Style, Engine, Model, and Dealer Name panels on the left sidebar
- **Sort controls** — column-level sorting on the details table
- **Tooltips** — hover-over detail on all chart elements

---

## Key Discoveries

| # | Insight | Detail |
|---|---|---|
| 1 | 🎨 **Color preference** | Pale White leads by volume (47%), but Black commands higher avg. prices |
| 2 | 🚙 **Body style demand** | SUVs are the most purchased style at 26.9% of total sales |
| 3 | 📈 **Sales trend** | Consistent weekly growth in H1, softening and volatility in H2 |
| 4 | 🏆 **Top regions** | Middletown and Aurora drive the highest dealer-level volume |
| 5 | 💰 **Premium brands** | Lincoln, Toyota (Tacoma), and Volvo achieve the highest avg. transaction prices ($82K+) |
| 6 | 📊 **Growth** | YTD sales up +23.59% and units sold up +24.57% YoY — strong overall momentum |

---

## Tools & Technologies

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard design, publishing, and interactivity |
| **Power Query** | Data ingestion, cleaning, and transformation |
| **DAX** | KPI measures, YTD/MTD calculations, conditional formatting |
| **Bing Maps** | Geographic regional sales visualization |
| **Excel** | Source data format |

---

## Skills Demonstrated

- End-to-end BI development from raw data to published dashboard
- Advanced DAX formula authoring (YTD, MTD, YoY, %GT)
- Multi-page report design with UX-focused navigation
- Data storytelling through complementary chart type selection
- Conditional formatting and dynamic KPI design
- Geographic data visualization with map visuals
- Drill-through architecture connecting summary and detail views
