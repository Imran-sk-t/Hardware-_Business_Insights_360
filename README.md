# Business Insights 360

## Project Overview

AtliQ Hardware is growing rapidly in the recent years, and they have decided to implement the data analytics using PowerBi in their company for the first time to surpass their competitors in the market and to make data driven decisions. This project is to give answers to the questions of stakeholder in terms all the aspects like finance, sales, marketing and supply chain.

## Tech stacks

- SQL
- PowerBi Desktop
- Excel
- DAX studio (for optimizing the report)
- Project charter file

### Dataset **Understanding**

Dimension table : It will have the static data like details of customer and products

Fact table : It will have the data about the transactions  

- gdb041:
    - dim_customer
        - **27** distinct markets (ex India, USA, spain)
        - **75** distinct customers thorough out the market
        - **2** types of platforms
            - Brick & Motors - Physical/offline store
            - E-commerce - Online Store (Amazon, flipkart)
        - Three channels
            - Retailer
            - Direct
            - Distributors
    - dim_market
        - **27** distinct markets (ex India, USA, spain)
        - 7 sub-zones
        - 4 regions
            - APAC
            - EU
            - nan
            - LATAM
    - dim_product
        - Divisions
            - P & A
                - Peripherals
                - Accessories
            - PC
                - Notebook
                - Desktop
            - N & S
                - Networking
                - Storage
        - There are 14 different categories, Like Internal HDD, keyboard
        - There are different variants available for the same product
    - fact_forecast_monthly
        - This table is used to forecast the customer’s need in advance, which can help in
            - Higher customer satisfaction
            - Reduced cost in warehouses for storage purpose
        - The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
        - All the date of the month will be replaced by the start date of the month
        - It will have all the column names and in the end it will have the forecast quantity need of the customer
    - fact_sales_monthly
        - This table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value.
- gdb056
    - freight_cost
        - This table has details of travel cost and other cost for each market with fiscal year
    - gross_price
        - Has the details of gross prices with product code
    - manufacturing_cost
        - Has the details of manufacturing cost with product code with year
    - Pre_invoice_dedutions
        - Has the details of pre invoice deductions percentage for each cutomer with year
    - Post_invoice_deductions
        - Post invoice deductions and other deductions details

## Importing data into PowerBi

- As the database is MySQL in this project, we need to import the datasets from Mysql database to PowerBi by providing the Database access credential

## Data Model

- In this project, we have followed Snowfall data modeling method.

<img src="https://github.com/Imran-sk-t/Hardware-_Business_Insights_360/blob/main/Business_Insights_360-main/Resources/Data_model.png" class="center">

## Home view

In Home view, all the views button will be available. User will land on specific view page by clicking the button 

- Info
- Finance View
- Sales View
- Marketing View
- Supply chain View
- Executive View
- Products
- Support

## Overall Report

![Overall Report.gif](https://github.com/Imran-sk-t/Hardware-_Business_Insights_360/blob/main/Business_Insights_360-main/Resources/Overall.gif)

## Info Page

![Info.gif](https://github.com/Imran-sk-t/Hardware-_Business_Insights_360/blob/main/Business_Insights_360-main/Resources/Info.gif)

## Finance View

![Finace.gif](https://github.com/Imran-sk-t/Hardware-_Business_Insights_360/blob/main/Business_Insights_360-main/Resources/Finace.gif)

## Sales View

![Sales.gif](https://github.com/Imran-sk-t/Hardware-_Business_Insights_360/blob/main/Business_Insights_360-main/Resources/Sales.gif)

## Marketing View

![Marketing.gif](https://github.com/Imran-sk-t/Hardware-_Business_Insights_360/blob/main/Business_Insights_360-main/Resources/Marketing.gif)

## Supply chain View

![Supply chain.gif](https://github.com/Imran-sk-t/Hardware-_Business_Insights_360/blob/main/Business_Insights_360-main/Resources/supply%20chain.gif)

## Executive View

![Executive.gif](https://github.com/Imran-sk-t/Hardware-_Business_Insights_360/blob/main/Business_Insights_360-main/Resources/Executive.gif)

## Products

![Products](https://github.com/Imran-sk-t/Hardware-_Business_Insights_360/blob/main/Business_Insights_360-main/Resources/Products%20View.gif)

## Project Outcome

By using this report, decisions can be taken based on the data. Further it will help in answering n number of 'why' questions based on the situations.
