# Data Analyst Portfolio Project - Sales Management (Power BI & SQL)
## Personal Project
## Business Request & User Stories
The business request for this data analyst project was an executive sales report for sales managers. Based on the request that was made from the business we following user stories were defined to fulfill delivery and ensure that acceptance criteria’s were maintained throughout the project.
| As a (role) | I want (request / demand) | So that I (user value)| Acceptance Criteria |
|--------------|-------|------|-------|
| Sales Manager | To get a dashboard overview of internet sales | Can follow better which customers and products sells the best | A Power BI dashboard which updates data once a day | 
| Sales Representative | A detailed overview of Internet Sales per Customers | Can follow up my customers that buys the most and who we can sell more to | A Power BI dashboard which allows me to filter data for each customer | 
| Sales Representative | A detailed overview of Internet Sales per Products | Can follow up my Products that sells the most | A Power BI dashboard which allows me to filter data for each Product | 
| Sales Manager | A dashboard overview of internet sales | Follow sales over time against budget | A Power Bi dashboard with graphs and KPIs comparing against budget. | 
## Data Warehouse
### Data Warehouse: 	AdventureWorksDW2019.bak
### Lightweight: AdventureWorksLT2019.bak
Note: We have Sales Amount data from December 29, 2019 to January 28, 2023. So we calculate by month from 1/1/2020 to 1/1/2023.
### Monthly budgets: FACT_Budget.xlsx (1/1/2020 - 1/1/2023)
### AdventureWorks DBs:: https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15&tabs=ssms
Note: After restoring to SQL Server, you must update Data Warehouse.
### Update SQL Data Script: https://github.com/techtalkcorner/SampleDemoFiles/blob/master/Database/AdventureWorks/Update_AdventureWorksDW_Data.sql
### Data Model
![image](https://user-images.githubusercontent.com/128765957/227419764-2c6c11d8-766d-4fb2-aaff-7e27b16fcc96.png)
## Data Cleansing & Transformation (SQL)
To create the necessary data model for doing analysis and fulfilling the business needs defined in the user stories the following tables were extracted using SQL.

One data source (sales budgets) were provided in Excel format and were connected in the data model in a later step of the process.

Below are the SQL statements for cleansing and transforming necessary data.
### DIM_Calendar:
![image](https://user-images.githubusercontent.com/128765957/227427538-882845ae-2aa6-4a22-a751-eac854de5973.png)
### DIM_Customers:
![image](https://user-images.githubusercontent.com/128765957/227427666-a5a75bf1-85ac-493c-9efe-68b8e17d9a4e.png)
### DIM_Products:
![image](https://user-images.githubusercontent.com/128765957/227427890-1e7aab5e-5388-4445-bd30-e4000b50ec71.png)
### FACT_InternetSales:
![image](https://user-images.githubusercontent.com/128765957/227428030-2eb436b7-2afa-4e82-b622-4f2486076fd3.png)
## Sales Management Dashboard
The finished sales management dashboard with one page with works as a dashboard and overview, with two other pages focused on combining tables for necessary details and visualizations to show sales over time, per customers and per products.
### Sales Overview
![image](https://user-images.githubusercontent.com/128765957/227428581-f936ed38-28e5-4518-a85e-3795ebd088fa.png)
### Customer Details
![image](https://user-images.githubusercontent.com/128765957/227428742-7f86ec77-fc17-47e5-ae25-877d0bc4a6f1.png)
### Product Details
![image](https://user-images.githubusercontent.com/128765957/227428797-685e8b15-d1f1-46d6-8332-93eab0ce8669.png)

