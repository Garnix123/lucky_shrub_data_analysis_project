# 🌿 Lucky Shrub – Client Persona Data Analysis (End of Course 4 Project)

This repository contains the **end-of-course project for Course 4** of the Meta Database Engineer track.  
It focuses on **advanced SQL data analysis** using a simulated database for the landscaping and gardening company **Lucky Shrub**.  

The project demonstrates database design, advanced queries, functions, stored procedures, triggers, JSON handling, common table expressions (CTEs), and views to generate actionable business insights.  

---

## 📂 Project Structure
- **LuckyShrub_DB.sql** → Creates and seeds the Lucky Shrub database with tables, relationships, and sample data.  
- **data_analysis_client_persona_lucky_shrub.sql** → Contains all analysis tasks (functions, stored procedures, triggers, and queries).  

---

## 🗂️ Database Schema
The project includes **eight main tables**:
- **Clients** → Customer details  
- **Employees** → Staff info with job titles & departments  
- **Products** → Inventory and pricing  
- **Orders** → Transactions data  
- **Addresses** → Client & employee addresses  
- **Activity** → Logs of online client activities (JSON column)  
- **Audit** → Tracks inserted orders with timestamps  
- **Notifications** → Stores system messages  

These are connected via **primary and foreign keys**, reflecting a real-world relational structure.  

---

## 📝 Tasks & Solutions

### **Task 1 – Average Sales Price**
- Function: `FindAverageCost(YearInput)`  
- Calculates the average product sale price for a given year.  

---

### **Task 2 – Product Evaluation Procedure**
- Procedure: `EvaluateProduct(product_id)`  
- Outputs the total items sold for a product across **2020, 2021, and 2022** into variables.  

---

### **Task 3 – Trigger for Audit**
- Trigger: `UpdateAudit`  
- Automatically inserts a timestamped record into the **Audit** table whenever a new order is added.  

---

### **Task 4 – Client & Employee Addresses**
- Query with `UNION` to return the full names and addresses of **both clients and employees**.  

---

### **Task 5 – Sales Performance with CTE**
- Original union query refactored into a **Common Table Expression (CTE)** to calculate yearly totals for product **P2 (Wood panels)**.  

---

### **Task 6 – JSON Activity Log**
- Extracts `ClientID` and `ProductID` directly from the JSON column in the **Activity** table, joined with Clients.  

---

### **Task 7 – Profit Calculation**
- Procedure: `GetProfit(product_id, YearInput)`  
- Computes the **total profit** for a product in a given year using sales and cost data.  

---

### **Task 8 – Data Summary View**
- View: `DataSummary`  
- Combines **Clients, Addresses, Orders, and Products** into one virtual table for easy analysis of orders in 2022.  

---

## 🎯 Why This Matters
- 🔑 **Real-world simulation**: Replicates common business reporting tasks.  
- 🏗 **Advanced SQL practice**: Functions, triggers, procedures, CTEs, JSON, and views in one project.  
- 📊 **Actionable insights**: Revenue, profit, sales trends, and customer data all in one place.  
- 💡 **Optimization focus**: Shows how to refactor queries (e.g., with CTEs) for clarity and performance.  

---

## 🚀 How to Use
1. Run **LuckyShrub_DB.sql** to create and seed the database.  
2. Execute **data_analysis_client_persona_lucky_shrub.sql** step by step.  
3. Test procedures and functions with different parameters (e.g., product IDs or years).  

---

## 📬 Contact
If you have questions or want to collaborate:  

- **LinkedIn**: [Dominik Vyleta](https://www.linkedin.com/in/dominik-vyleta-mba-a566511b2/)  
- **GitHub**: [Garnix123](https://github.com/Garnix123)  
- **Email**: vyleta.dom@gmail.com  
