# 09-Load-Data-into-Data-Warehouse.md
In this exercise, you're going to load data into a dedicated SQL Pool.

# Load Data into a Relational Data Warehouse - Lab Exercise 🚀

## 📌 Overview  
This lab guides you through loading data into a dedicated SQL pool in Azure Synapse Analytics. You'll practice:

- Using the COPY statement for efficient data loading  
- Creating tables with CTAS (CREATE TABLE AS SELECT)  
- Implementing slowly changing dimension (SCD) patterns  
- Performing post-load optimization  

## ⏳ Estimated Duration  
Approximately 30 minutes  

## 🛠️ Prerequisites  
- Azure subscription with admin access  
- Basic knowledge of SQL and data warehousing concepts  

## 🏗️ Lab Setup  

### Provision Azure Synapse workspace:  
- Run the provided PowerShell script in Azure Cloud Shell  
- Script will deploy:  
  - Synapse workspace  
  - Data Lake Storage Gen2  
  - Dedicated SQL pool  

### Prepare data:  
- Verify CSV files (Product.csv, Customer.csv) in the data lake  
- Start the dedicated SQL pool  

## 🔍 Key Tasks  

### 1. Load data using COPY statement  
- Load data from CSV files into staging tables  
- Handle errors with error files in `_rejectedrows` folder  

### 2. Create dimension tables  
- Use CTAS to create DimProduct table  
- Implement SCD patterns for DimCustomer:  
  - Type 1 changes (in-place updates)  
  - Type 2 changes (historical tracking)  

### 3. Post-load optimization  
- Rebuild table indexes  
- Create statistics for query optimization  

## 🧹 Cleanup  
Don't forget to:  
- Pause or delete the SQL pool when not in use  
- Delete the resource group to avoid ongoing charges  

## Screenshots
![lab91](https://github.com/user-attachments/assets/39f3bf9d-5229-4947-8d8e-b5c694fe36f6)
![lab92](https://github.com/user-attachments/assets/07f4bafc-33bd-4d8f-9335-a17dd912317d)
![lab93](https://github.com/user-attachments/assets/cfa055c3-951e-471e-b24a-7e19594575d9)
![lab94](https://github.com/user-attachments/assets/641d6b8f-8ae1-45e8-84d8-110b5fe2aab4)
![lab95](https://github.com/user-attachments/assets/701da7ee-34db-4ff8-b0cc-f612a068c22a)
![lab96](https://github.com/user-attachments/assets/6a37ca07-3a53-489a-8c57-febbe47fed56)
![lab97](https://github.com/user-attachments/assets/685b6b99-e8e7-428b-a64e-28a679b8d9bd)


