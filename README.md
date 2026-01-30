
![Employee Attrition Banner](https://www.dreamstime.com/lunchboxes-different-meals-wooden-table-flat-lay-healthy-food-delivery-lunchboxes-different-meals-wooden-table-image162144231)

# Food Delivery Analysis

## Project Overview  
This Power BI report provides an end-to-end sales and delivery performance analysis for a Food Delivery business. The objective of the report is to help stakeholders understand order trends, delivery efficiency, and overall operational performance using clean data, optimized DAX measures, and intuitive visualizations.

The report is designed with a business-user-first approach, ensuring insights are easy to interpret and actionable.

## Data Sources  
The report is built using structured datasets related to food delivery operations. Typical data includes:
- Delivery Details (Fact Table)
- Order ID
- Delivery Time (Minutes)
- Order Date
- Delivery Status
- Revenue / Order Value
- Dimension Tables
- Date Dimension (Day, Month, Year)
- Location / Area
- Customer
- Restaurant / Outlet
These tables follow a Star Schema for better performance and clarity.  

## Data Cleaning & Transformation (Power Query)
Data preparation was performed using Power Query Editor. Key cleaning steps include:
- Removing duplicate records
- Handling missing or null values
- Standardizing column names and data types
- Converting date and time fields into usable formats
- Creating calculated columns where required (e.g., delivery buckets)
This step ensures the data model is reliable and analysis-ready before applying DAX.

## Data Modeling 
Implemented a Star Schema with:
- Fact table at the center (Delivery Details)
- Dimension tables connected using one-to-many relationships
- Filter direction is kept single-directional to avoid ambiguity and improve performance
- Proper relationships ensure accurate filter propagation across visuals
- 
## DAX Measures & Calculations
Key Measures
- Total Orders – Count of all delivery records
- On-Time Deliveries – Orders delivered within defined SLA (e.g., ≤ 30 minutes)
- On-Time Delivery %
- Late Delivery Count
- Total Revenue
DAX Concepts Used
- CALCULATE() for context modification
- COUNTROWS() for dynamic counts
- FILTER() for conditional logic
- DIVIDE() for safe percentage calculations

## Visualizations & Report Design
Visual Elements:
- KPI Cards (Total Orders, On-Time Delivery %)
- Bar & Column Charts (Orders by Date / Location)
- Tables for detailed order-level analysis
- Slicers for Date, Location, and Status

## Conclusion
This Power BI report demonstrates a complete analytics workflow:
Data Cleaning → Data Modeling → DAX Calculations → Visualization → Business Insights
It reflects strong fundamentals in Power BI, DAX, and data storytelling, making it suitable for both operational analysis and stakeholder reporting.

## Conclusion  
This analysis helps HR teams identify risk factors and improve employee retention strategies.
