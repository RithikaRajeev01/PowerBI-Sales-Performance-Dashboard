# Executive Sales Performance Dashboard | Power BI

![Dashboard Overview](Images/dashboard_overview.png)

> Interactive executive dashboard built using Power BI and the AdventureWorks Sales Dataset to monitor revenue performance, customer growth, product performance, and regional sales trends.

## Overview

This project showcases an executive sales performance dashboard developed in Power BI using the AdventureWorks Sales dataset.

The objective was to transform transactional sales data into a centralized reporting solution that enables business stakeholders to monitor revenue performance, evaluate customer and product trends, identify underperforming areas, and support data-driven decision making.

---

## Business Problem

Sales data is often distributed across multiple tables containing customers, products, orders, and geographical information.

Without a consolidated reporting solution, business leaders struggle to:

* Track revenue performance over time
* Identify top and bottom performing products
* Understand customer segment contributions
* Evaluate regional sales performance
* Monitor business growth through KPIs

The goal of this project was to create a single executive dashboard capable of answering these questions through interactive analytics.

---

## Dataset

**Dataset:** AdventureWorks Sales Dataset

**Source:** Kaggle

Dataset includes:

* Sales Transactions
* Customer Data
* Product Data
* Product Categories
* Product Subcategories
* Territory Information

A custom Date Table was created to support time intelligence calculations and KPI growth analysis.

---

## Approach

### Data Preparation

* Cleaned and validated source data using Power Query.
* Established relationships across multiple tables.
* Created a Date Table for time-based analysis.

### Data Modeling

Implemented a dimensional model consisting of:

**Fact Table**

* Sales

**Dimension Tables**

* Customers
* Products
* Product Categories
* Product Subcategories
* Territories
* DateTable

### KPI Development

Created custom DAX measures to track:

* Revenue Growth %
* Orders Growth %
* Customer Growth %
* Previous Year Revenue
* Previous Year Orders
* Previous Year Customers

---

## Business Questions Answered

### Revenue Performance

* How is revenue trending over time?
* Is revenue growing or declining compared to previous periods?

### Customer Analysis

* Which customer segments contribute the most revenue?
* Is the customer base growing?

### Product Performance

* Which products generate the highest revenue?
* Which products require attention due to weak performance?

### Geographic Analysis

* Which territories generate the strongest sales performance?
* Where should future growth initiatives be focused?

### Operational Monitoring

* How are order volumes changing over time?
* Are business KPIs improving or declining?

---

## Business Decisions Supported

The dashboard helps decision-makers:

* Identify underperforming products requiring pricing, promotion, or inventory review.
* Prioritize high-performing product categories for investment.
* Evaluate customer segments contributing the highest business value.
* Monitor growth trends using Revenue, Orders, and Customer KPIs.
* Compare regional performance and identify expansion opportunities.
* Detect performance declines early through trend monitoring.

---

## Tech Stack

* Power BI Desktop
* Power Query
* DAX
* Excel
* CSV Data Sources

---

## Data Dictionary & Analytical Logic

### Revenue Growth %

Measures revenue growth compared to the previous year using DAX time intelligence.

### Orders Growth %

Measures changes in order volume compared to the previous year.

### Customer Growth %

Measures customer acquisition and retention trends over time.

### Date Table

A dedicated Date Table was implemented to support:

* Time Intelligence
* Year-over-Year Analysis
* Trend Analysis

### Data Model

A star-schema style model was implemented using:

* CustomerKey
* ProductKey
* TerritoryKey
* OrderDate

to ensure efficient filtering and reporting.

---

## Skills Demonstrated

* Business Intelligence Reporting
* Dashboard Design
* Data Modeling
* DAX
* Power Query
* KPI Development
* Time Intelligence
* Data Visualization
* Data Storytelling

---

## Repository Contents

```text
Reports/
 └── Sales_Performance_Dashboard.pbix

Data/
 ├── Sales.xlsx
 ├── AdventureWorks_Product_Categories.csv
 ├── AdventureWorks_Product_Subcategories.csv
 ├── AdventureWorks_Territories.csv
 └── AdventureWorks_Customer.csv

Images/
 └── dashboard_overview.png
```

---

## How to Run

1. Download the repository.
2. Open the PBIX file using Power BI Desktop.
3. Refresh the data if required.
4. Interact with filters and visuals to explore business performance.
