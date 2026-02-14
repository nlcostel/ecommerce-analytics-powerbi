# E-Commerce Analytics & Customer Insights Dashboard (Power BI)
A complete Power BI analytics solution designed to uncover customer behavior patterns, sales performance, and operational insights within an e-commerce business.
This project includes a clean star-schema data model, fully documented DAX calculations, interactive drillthrough reports, and a comprehensive Customer Profile experience.

![Power BI](https://img.shields.io/badge/Tool-PowerBI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Made With](https://img.shields.io/badge/Made_With-DAX-blue?style=for-the-badge)
![Dataset Size](https://img.shields.io/badge/Data_Size-5_CSVs-orange?style=for-the-badge)
![Dashboard](https://img.shields.io/badge/Dashboard-E--Commerce_Insights-blueviolet?style=for-the-badge)
![Customer Profile](https://img.shields.io/badge/Feature-Customer_Profile-ff69b4?style=for-the-badge)

![License](https://img.shields.io/badge/License-MIT-green.svg?style=flat)
![Contributions](https://img.shields.io/badge/Contributions-Welcome-blue.svg)

# Project Overview 
This dashboard suite highlights:

✔ Executive Operations Dashboard

    Total Sales, Profit, and Orders

    Category performance

    Geographic insights

    Sales vs. Target comparison

    Monthly customer activity trends
    
  ✔ Customer Profile Drillthrough

    An interactive, dynamic customer detail page featuring:

    Full Name, Email, City/State, Signup Date

    Customer Lifetime Value (LTV)

    AOV (Average Order Value)

    First & Last Order Dates

    Total Orders, Total Sales, Return Count

    Purchase trend over time

    Category sales breakdown

✔ Behavioral Insights (Pattern-Based)

    Purchasing frequency

    Days between orders

    Seasonal trends

    Return behavior patterns

    Category preferences

    Early churn warning metrics

# Architecture & Data Model

The project follows a clean star schema, using five fact and dimension tables:

<img width="150" height="157" alt="image" src="https://github.com/user-attachments/assets/ec775d9c-42e4-4ac3-8d26-3dd48f9c2367" />

## Fact Table

    order_items (granular transaction data)

## Dimensions

  * customers

  * products

  * orders

  * returns

## Key Relationships

1. orders[order_id] → order_items[order_id]

2. products[product_id] → order_items[product_id]

3. customers[customer_id] → orders[customer_id]

4. orders[order_id] → returns[order_id]

<img width="803" height="380" alt="image" src="https://github.com/user-attachments/assets/1259c4c1-517d-4dbf-adae-624fb38d3239" />

# DAX Measures

<img width="145" height="44" alt="image" src="https://github.com/user-attachments/assets/1d0a17c5-6b35-42ff-9849-46298be3e4df" />

### This Includes

  * Total Sales

  * Gross Profit

  * Total Orders

  * Customer Lifetime Value

  * AOV

  * Customer Return Count

  * New Customers YTD

  * Dynamic customer name & location display

  * Drillthrough-specific measures

<img width="241" height="746" alt="image" src="https://github.com/user-attachments/assets/c01c558f-18b9-49da-8f48-9774a5cbff15" />


# Report Files

<img width="321" height="42" alt="image" src="https://github.com/user-attachments/assets/2a4acea8-49fa-4e64-a397-7e70567f62b9" />

## The PBIX file contains:

    All dashboards

    All DAX measures

    All data modeling work

    Theme, layout, formatting, and bookmarks

    Drillthrough functionality

# Dashboard Previews



  ## Dashboard Overview

<img width="1294" height="802" alt="image" src="https://github.com/user-attachments/assets/719a5d7e-fbd3-4e7b-ba6d-38542ee91fa1" />

  ## Customer Profile

<img width="1408" height="769" alt="image" src="https://github.com/user-attachments/assets/032a7d72-06e2-4d16-a29e-e849dacd21a7" />
 
# Key Features

## Drillthrough Customer Profile

Select any customer in the report to view a personalized analytics page.

<img width="1406" height="767" alt="image" src="https://github.com/user-attachments/assets/da89fa5f-65d2-40a3-bcac-b26bc9495680" />


## Dynamic Cards

Cards update based on slicer selections using DAX logic such as:

<img width="1294" height="792" alt="image" src="https://github.com/user-attachments/assets/9f356f34-b84c-4181-ab93-0e85698e485a" />


## Fully Custom Visual Theme

Consistent styling, shape backgrounds, card formatting, and layout grid. 

## Behavioral Metrics

Designed to reflect real e-commerce analytics use cases, including:

      Purchase volatility

      Spend distribution

      Category biases

      Returns-to-orders ratio

# Getting Started

*1. Clone the Repository*

  * git clone https://github.com/nlcostel/ecommerce-analytics-powerbi.git

*2. Open in Power BI Desktop*

  * /report/ecommerce_customer_insights.pbix

*3. Explore the Dashboards*

  * Use slicers --> select customer --> explore insights
    

*Navigate across pages using navigation buttons and drillthroughs*

# Tools Used

    Power BI Desktop

    Power Query

    DAX (Data Analysis Expressions)

    Star Schema Modeling

    GitHub for version control

    Synthetic e-commerce dataset (CSV)

# Contact

If you'd like to collaborate or discuss this project:

Coley Costello

🔗 GitHub: https://github.com/nlcostel

# Support

If this project helped you or you'd like to support the work:

    → Star the repository ⭐
    
    → Share with other Power BI learners or professionals

# License

This project is available under the MIT License – see LICENSE.md for details.






