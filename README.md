# Atliq Sales Dashboard

The Atliq Sales Dashboard is an interactive Power BI dashboard developed to analyze real-time sales data for Atliq, focusing on metrics like revenue, top cities, top customers, product types, and customer types. This dashboard allows business stakeholders to make informed decisions, optimize operations, and understand sales trends.

## Table of Contents
- [Project Overview](#project-overview)
- [Project Demo](#Project-demo)
- [Key Metrics and Features](#Key-Metrics-and-Features)
- [Data Source](#Data-Source)
- [Implementation Details](#implementation-details)
- [Insights and Findings](#Insights-and-Findings)

  
## Project Overview

The objective of this project is to create a comprehensive sales dashboard that enables Atliq's sales and marketing teams to quickly access and analyze essential KPIs. 

## Key Metrics and Features

- **Total Revenue**: Shows overall revenue generated from sales.
- **Revenue by City**: Identifies top-performing cities by revenue.
- **Revenue by Customer**: Highlights key customers and their contribution to revenue.
- **Revenue Trend**: Displays monthly revenue trends, helping to identify seasonal patterns.
- **Product Selection**: Allows filtering of metrics by individual products to understand their specific impact.
- **Product Type**: Differentiates between "Own Brand" and "Distribution" products.
- **Customer Type**: Shows the split between "Brick & Mortar" and "E-Commerce" customers.

## Data Source

This data is provided by the CodeBasis challenge platform and is updated in real-time to reflect current sales performance. The data includes information on revenue, cities, customers, product types, and customer segments.

## Implementation Details

### 1. Data Understanding and Requirements Gathering
   - Gathered business requirements to identify relevant KPIs and metrics for sales analysis.
   - Defined primary data sources and metrics, such as revenue, product categories, customer types, and regions.

### 2. Data Modeling
   - Designed a star schema to structure the data for efficient querying and analysis.
   - Created fact and dimension tables:
     - **Fact Table**: Sales transactions including metrics like SalesAmount, CustomerID, ProductID, etc.
     - **Dimension Tables**: City, Customer, Product, Date, and CustomerType, each providing contextual information for slicing and dicing the data.

### 3. Data Extraction, Transformation, and Loading (ETL)
   - Extracted sales data from source systems (as provided by CodeBasis).
   - Transformed data to fit the star schema, ensuring data quality and integrity.
   - Loaded the transformed data into the Power BI data model.

### 4. Data Validation and Quality Assurance
   - Implemented validation rules and performed data quality checks to ensure data consistency and accuracy.
   - Conducted cross-checks between raw data and transformed data to verify the data pipeline's accuracy.

### 5. Handling Row Dropping
   - Addressed rows with invalid or erroneous data:
     - For example, rows where `SalesAmount ≤ 0` were either corrected or dropped as per business rules.

### 6. Reporting and Analytics
   - Developed a Power BI dashboard to provide insights on the defined KPIs.
   - Utilized various visualizations to create an intuitive and actionable user interface, including bar charts, line charts, and donut charts.
   - Implemented slicers for year, month, and product selection to enable dynamic filtering.

## Insights and Findings

- **Revenue Concentration**: The majority of revenue is concentrated in certain cities, with Delhi NCR contributing the highest at 53.39%.
- **Top Customers**: Key customers like "Electricalara Stores" contribute significantly to the overall revenue, with individual breakdowns available for further analysis.
- **Revenue Trend**: Seasonal peaks and troughs are visible in the revenue trend, highlighting periods of increased or decreased sales activity.
- **Product and Customer Segmentation**: The dashboard differentiates between "Own Brand" and "Distribution" products, as well as between "Brick & Mortar" and "E-Commerce" customers, allowing the business to tailor its strategies to each segment.

