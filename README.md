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
