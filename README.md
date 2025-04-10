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

## 📂 Lab Contents

### 1. Aggregate Data
Use T-SQL aggregate functions to summarize data.

```sql
SELECT CalendarYear, 
       SUM(SalesAmount) AS TotalSales 
FROM FactInternetSales AS i
JOIN DimDate AS d ON i.OrderDateKey = d.DateKey
GROUP BY CalendarYear;

