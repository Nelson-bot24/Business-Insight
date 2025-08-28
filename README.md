# Business-Insight
## Problem Statement :
AtliQ Hardware, a leading consumer electronics company, operates globally with a diverse customer base, similar to well-known brands like HP and Dell. While AtliQ Hardware has been experiencing rapid growth, it has encountered challenges in the Latin American market. These challenges stem from their reliance on Excel files for data management. Excel, although versatile, presents difficulties in terms of data comprehension, visualization capabilities, and scalability. These limitations have led to significant losses in the Latin American market." To address this, our objective is to implement an advanced analytics solution to enable efficient data analysis and drive informed decision-making.
## Data Source Details :
Understanding what data is available will be more helpful while doing analysis. before jumping on to the analysis get good understanding of what are data available.

Dimension table : It will have the static data like details of customer and products

Fact table : It will have the data about the transactions

❇️ gdb041
  ## ⚫ dim_customer
        👉 27 distinct markets (ex India, USA, spain) 
        👉 75 distinct customers thorough out the market
        👉 2 types of platforms
            ▫️ Brick & Motors - Physical/offline store
            ▫️ E-commerce - Online Store (Amazon, flipkart)
        👉 Three channels
            ▫️ Retailer
            ▫️ Direct
            ▫️ Distributors
  ## ⚫dim_market
        👉 27 distinct markets (ex India, USA, spain)
        👉 7 sub-zones
        👉 4 regions
            ▫️ APAC
            ▫️ EU
            ▫️ nan
            ▫️ LATAM
   ## ⚫ dim_product
        👉 Divisions
             ◾ P & A
                 ▫️ Peripherals
                 ▫️ Accessories
             ◾ PC
                 ▫️ Notebook
                 ▫️ Desktop
             ◾ N & S
                 ▫️ Networking
                 ▫️ Storage
         👉 There are 14 different categories, Like Internal HDD, keyboard
         👉 There are different variants available for the same product
   ## ⚫ fact_forecast_monthly
         👉 This table is used to forecast the customer’s need in advance, which can help in 
               ▫️ Higher customer satisfaction 
               ▫️ Reduced cost in warehouses for storage purpose
         👉 The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
         👉 All the date of the month will be replaced by the start date of the month
         👉 It will have all the column names and in the end it will have the forecast quantity need of the customer
   ## ⚫ fact_sales_monthly
         👉 This table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value.
❇️ gdb056
  ## ⚫ freight_cost
          This table has details of travel cost and other cost for each market with fiscal year
  ## ⚫ gross_price
         Has the details of gross prices with product code
  ## ⚫ manufacturing_cost
         Has the details of manufacturing cost with product code with year
  ## ⚫ Pre_invoice_dedutions
         Has the details of pre invoice deductions percentage for each cutomer with year
  ## ⚫ Post_invoice_deductions
         Post invoice deductions and other deductions details
Note : Target values/Bench mark values were only given for 2022 fiscal year,only withrespective market column.
## Data Model :
<img width="970" height="683" alt="Screenshot 2025-08-28 145627" src="https://github.com/user-attachments/assets/c8896617-68b6-4611-b8e4-d09c6234c8c0" />
In this project, we have followed Snowfall data modeling method.

## Objective :
    To Deploy an advanced analytics solution for AtliQ Hardware to enhance data analysis efficiency. which will offer comprehensive insights tailored to meet the needs of business leaders across various domains, such as Sales, Finance, Marketing, Supply Chain, and Execution.

👉 Sales View
