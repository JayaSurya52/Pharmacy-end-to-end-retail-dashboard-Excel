# Pharmacy End-to-End Retail Dashboard – Excel

An interactive Retail Sales Dashboard built in Excel using Power Query, Power Pivot, and DAX. The dashboard transforms raw sales data into actionable insights through KPI tracking, trend analysis, and dynamic visualizations.

---

## Problem Statement

This project involves developing an interactive Retail Sales Dashboard in Microsoft Excel to analyze sales performance, customer behavior, product trends, and regional performance.

The dashboard is designed to transform raw sales data into meaningful business insights using Power Query, Power Pivot, Pivot Tables, and Pivot Charts.

## Business Problem

Retail companies generate thousands of sales transactions every day. Analyzing this data manually is difficult and time-consuming. Management teams often struggle to identify:

- Monthly sales trends
- Sales by category
- Quarterly sales performance
- Products that generate the most revenue

To address these challenges, an automated and interactive dashboard was developed to provide quick and accurate business insights.

## KPI Requirements

- Total Sales Revenue
- Total Purchase
- Total GST Paid
- Total Profit
- Total Profit Margin %

## Tools & Technologies Used

| Tool | Purpose |
|---|---|
| Microsoft Excel | Dashboard Development |
| Power Query | Data Cleaning and Transformation |
| Power Pivot | Data Modeling |
| Pivot Tables | Analysis and Reporting |
| Pivot Charts | Visual Representation |
| Slicers & Timelines | Interactive Filtering |

## Step-by-Step Implementation

### Step 1: Load Data into Power Query

- Imported raw datasets into Power Query.
- Validated data quality.
- Performed cleaning and transformation operations.

### Step 2: Build Data Model

Created relationships between:

- Sales Table
- Purchase Table
- Calendar Table

This established a structured data model inside Power Pivot.

### Step 3: Create Measures

Developed business measures such as:

**Total Sales**
```DAX
Total Sales = SUM('Sales Table'[Net Amount])
```

**Total Purchase**
```DAX
Total Purchase = SUM('Purchase Table'[Total Amount])
```

**GST Paid**
```DAX
GST Paid = SUM('Sales Table'[Sales GST]) - SUM('Purchase Table'[Purchase GST])
```

**Total Profit**
```DAX
Total Profit = [Total Sales] - [Total Purchase] - [GST Paid]
```

**Profit Margin %**
```DAX
Profit Margin % = DIVIDE([Total Profit], [Total Sales])
```

### Step 4: Create Pivot Tables

Pivot Tables were created to analyze:

- Sales by Month
- Sales by Quarter
- Sales by Category
- Top 5 Products by Sales

### Step 5: Create Visualizations

The following charts were designed:

- Line Charts
- Bar Charts
- Doughnut Chart
- Column Chart

### Step 6: Add Interactivity

Implemented:

- Slicers
- Timelines
- Dynamic Filtering

Users can interact with dashboard components and view data instantly.

### Step 7: Dashboard Design

Designed a professional dashboard layout with:

- KPI Section
- Sales Trends
- Product Analysis
- Quarterly Sales Performance
- Staff Performance

## Conclusion & Future Improvements

### Conclusion

The Retail Sales Dashboard successfully transformed raw business data into meaningful visual insights. The dashboard improved reporting efficiency and enabled management to make faster, data-driven decisions.

The project demonstrates strong skills in:

- Excel Dashboarding
- Data Cleaning
- Data Modeling
- Business Analysis
- Data Visualization
- Reporting Automation

### Future Improvements

Future enhancements may include:

- Profit Analysis Dashboard
- Sales Forecasting
- Customer Retention Analysis
- Power BI Integration
- Automated Data Refresh


