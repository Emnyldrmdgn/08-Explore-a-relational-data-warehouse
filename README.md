# 08-Explore-a-relational-data-warehouse
In this lab, the data warehouse is hosted in a dedicated SQL pool in Azure Synapse Analytics.

# Lab08 - Analyze Data with Transact-SQL in Azure Synapse Analytics

## 📘 Overview

This lab is part of the **DP-203: Data Engineering on Microsoft Azure** certification. You will learn how to use Transact-SQL (T-SQL) in **Azure Synapse Analytics** to explore and analyze large volumes of data. The lab focuses on advanced querying techniques including **aggregation**, **window functions**, and **approximate aggregations**.

---

## 🛠️ Prerequisites

- Active Azure subscription
- Azure Synapse Analytics workspace and dedicated SQL pool (sqlxxxxxxx)
- Access to Synapse Studio
- Sample data already loaded (e.g., `FactInternetSales`, `DimDate`, `DimGeography`, etc.)

---

## 📌 Purpose  
This lab focuses on analyzing sales data stored in a data warehouse using fact and dimension tables. You'll explore database schemas, write analytical queries, and manage Azure resources efficiently.

---

## 2. View Database Tables  

### 🎯 Why?  
To understand the schema of the data warehouse and distinguish between **fact** and **dimension** tables.

---

## ⭐ 3. Examine Fact and Dimension Tables  

Data warehouses typically include two types of tables:

- **Fact Tables**  
  Store measurable data used for numerical analysis.  
  _Examples: `FactInternetSales`, `FactResellerSales`_

- **Dimension Tables**  
  Contain descriptive attributes related to facts.  
  _Examples: `DimProduct`, `DimCustomer`, `DimTime`, `DimGeography`_

---

## 🎯 4. Introduction to Data Warehouse Queries  

### Objective  
Analyze internet sales from the `FactInternetSales` table using various dimensions such as time, geography, and product.

### Tasks  
- Join `FactInternetSales` with appropriate dimension tables (e.g., `DimTime`, `DimProduct`, `DimGeography`).
- Group and summarize total sales.
- Save and **publish** your query script.
- Rename the script to:  
  **`Analyze Internet Sales`**

---

## 🎯 5. Challenge: Reseller Sales Analysis  

### Create a new script:  
**`Analyze Reseller Sales`**

### Write SQL queries to analyze the following:

1. **Total quantity of items sold per fiscal year and quarter.**
2. **Total quantity of items sold per fiscal year, quarter, and sales territory** associated with the employee who made the sale.
3. **Total quantity of items sold per fiscal year, quarter, and sales territory region by product category.**
4. **Rank of each sales territory per fiscal year** based on total sales amount.
5. **Approximate number of sales orders per year in each sales territory.**

---

## 🧹 6. Clean Up Azure Resources  

To avoid incurring further costs:

1. Go to the **Resource groups** section in the Azure portal.
2. Select the resource group used for this lab.
3. Click **Delete resource group**.
4. Confirm the resource group name and proceed with deletion.

---

## ✅ Completion  
You’ve successfully completed Lab08 by exploring the structure and analysis capabilities of a data warehouse in Azure Synapse. Great job!


## screenshots


https://github.com/user-attachments/assets/51bacaf0-a358-44a6-afa5-e0dc93db08eb


![lab8](https://github.com/user-attachments/assets/0c1ea281-6ec3-49cf-a670-641c4e617702)
![lab82](https://github.com/user-attachments/assets/f8052b89-1e91-401d-9b55-dc1635dc5632)
![lab83](https://github.com/user-attachments/assets/be6107ec-15ac-41eb-b2bd-702bebe79819)
![lab84](https://github.com/user-attachments/assets/db4685a1-d4cb-4f84-9a2f-1f52a2cf68de)



https://github.com/user-attachments/assets/8967bc2e-927c-432e-ac57-d0562ce5c4cd
