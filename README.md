# 🌍 Global Health Database (SQL Project)

### 📊 Data and SQL | By **Avril Childs**

This project was created as part of the **Code First Girls Data & SQL** module to demonstrate end-to-end database design, querying, and analytical insight generation using real-world health data from [Our World in Data](https://ourworldindata.org/).

---

## 🧠 Project Overview

The **Global Health Database** models key health indicators across World Health Organization (WHO) regions.  
It explores relationships between **health expenditure**, **life expectancy**, and **child mortality**, using structured relational design, SQL joins, stored functions, and data visualisation.

---

## 🗂️ Database Design

### **1. WHO_Regions**
- Contains WHO region identifiers and total population (in millions)  
- `Region_ID` set as **Primary Key**  
- Serves as the reference table for regional classification  

### **2. Representative_Countries**
- Represents countries linked to their WHO region  
- Uses **Foreign Key (`Region_ID`)** for referential integrity  

### **3. Country_HealthEx_Pop**
- Stores **health expenditure ($ per capita)** and **population (millions)** per country  
- Linked via **Country_ID (FK)**  

### **4. Life_Expectancy**
- Contains male and female life expectancy (in years) for each country  

### **5. Child_Mortality**
- Records infant and child mortality rates (% of births), comparing 1969 vs 2019  

---

## 🧩 SQL Concepts & Tools Used

| SQL Concept | Description |
|--------------|-------------|
| **Database Design** | Normalised schema with primary and foreign keys |
| **ENUM Types** | Used to specify WHO region categories |
| **JOINS** | `LEFT JOIN` and `INNER JOIN` to combine multi-table data |
| **Subqueries** | Used for region-specific filtering (e.g., South-East Asia) |
| **Aggregate Functions** | `AVG()`, `SUM()` for regional insights |
| **Stored Functions** | Custom SQL function to compute *average health expenditure per region* |
| **Views** | Combined multiple base tables for summary reports |
| **Formatting** | Rounded results to two decimal places for clarity |

---

## 🔍 Example Analytical Queries

- **Average Health Expenditure by WHO Region**  
  → Implemented using a stored function combining `JOIN` and `AVG()`  

- **Child Mortality (South-East Asia)**  
  → Subquery filtered by `Region_ID = R3`  

- **Lowest Combined Life Expectancy by Region**  
  → `INNER JOIN` + average of male/female columns  

- **Top 10 Countries by Child Mortality**  
  → Query used to explore correlation between mortality and healthcare spend  

---

## 📈 Visualisation

Health data was visualised in **Tableau** to examine correlations between:  
> 💡 *Child Mortality (%) vs. Health Expenditure ($ per capita)*  

**Findings:**  
Countries investing more in healthcare tend to have **lower child mortality rates** — showing an inverse relationship between expenditure and mortality.

---

## 🧰 Tools & Technologies

- 🐘 **SQL (MySQL / PostgreSQL syntax)**  
- 📊 **Tableau** – data visualisation and analytics  
- 🌐 **Our World in Data** – source dataset  
- 👩‍💻 **Code First Girls** – learning and project framework  

---

## 🧩 Key Skills Demonstrated

- Relational database design & normalisation  
- Query optimisation and data joining  
- Creating and using stored SQL functions  
- Data aggregation and transformation  
- Analytical insight generation using queries  
- Data storytelling and presentation in Tableau  

---

## 📜 Author

**👩‍💻 Avril Childs**  
_Data Scientist | SQL Developer | Health Researcher_  

📍 [GitHub: AvChilds](https://github.com/AvChilds)  
🔗 [LinkedIn: Avril Childs](https://linkedin.com/in/avrilechilds)

---

> *“Turning data into insights that improve health outcomes globall
