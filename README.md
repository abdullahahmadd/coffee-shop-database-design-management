# 🛢️Coffee Shop Database Design
### 🎓 IBM Data Engineering Specialization – Portfolio Project

![Visitors](https://visitor-badge.laobi.icu/badge?page_id=abdullahahmadd.coffee-shop-db-design)
![Database](https://img.shields.io/badge/Database-Relational-blue)
![SQL](https://img.shields.io/badge/SQL-lightgrey)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-blue?logo=postgresql)
![MySQL](https://img.shields.io/badge/MySQL-orange?logo=mysql)

---

## 📑 Table of Contents
1. [Overview](#-overview)
2. [Business Problem & Objective](#-business-problem--objective)
3. [Database Technologies](#-database-technologies)
4. [Skills Demonstrated](#-skills-demonstrated)
5. [Project Flow](#-project-flow)
6. [Results](#-results)
7. [About This Project](#-about-this-project)

---

## ☕ Overview
This project demonstrates the **design and implementation of a relational database system** for a coffee shop business.  
It focuses on building a clean, normalized database schema and enabling data access through SQL views and materialized views, with data shared across **PostgreSQL** and **MySQL** environments.

The project reflects real-world database design practices, emphasizing data integrity, scalability, and structured data sharing.

---

## 💼 Business Problem & Objective

A growing coffee shop business plans to expand operations and open multiple franchise locations. However, its data is currently scattered across different systems, including spreadsheets, point-of-sale outputs, supplier exports, and customer records. This fragmented setup makes it difficult to maintain data consistency, streamline operations, and support data-driven decision-making.

The objective of this project is to design and implement a **centralized relational database system** that consolidates these disparate data sources into a structured, normalized schema. The solution enables efficient storage, reliable relationships between entities, and the ability to share curated datasets with external stakeholders such as payroll and marketing teams.

---

## 🛠️ Database Technologies
- **SQL** — used for DDL, constraints, views, and materialized views
- **PostgreSQL** — primary DBMS for schema design, normalization, and data processing  
- **MySQL** — secondary DBMS for external data consumption    

---

## 🎯 Skills Demonstrated
- Relational database design
- Data normalization (up to 2NF)
- Primary key and foreign key implementation
- Entity Relationship Diagram (ERD) modeling
- SQL views and materialized views
- PostgreSQL and MySQL integration
- Data export and import between RDBMS

---

## 🔄 Project Flow

1. **Requirement Analysis**
- Reviewed operational data sources including staff, sales outlets, customers, products, and sales transactions.  
- Based on these sources, core entities, attributes, and relationships required for a centralized relational database were identified.

2. **Initial Schema Design (PostgreSQL)**
- Designed an initial relational database schema to model the identified business entities.  
- An Entity Relationship Diagram (ERD) was created in PostgreSQL to visually represent entities and their relationships.

3. **Normalization (PostgreSQL)**
- Normalized the database schema to reduce redundancy and ensure data consistency.  
- Transactional and descriptive data were separated into appropriate tables, and the ERD was updated to reflect the normalized structure.  
- The final design adheres to **Second Normal Form (2NF)** with clearly defined relationships.

4. **Schema Implementation (PostgreSQL)**
- Generated SQL scripts from the ERD and implemented the schema in PostgreSQL.  
- Database tables were created along with primary keys and foreign key constraints to enforce data integrity.  
- Sample data was then loaded into the schema to validate the design.

5. **View Creation (PostgreSQL)**
- Created a **SQL view** to provide staff and work location data while excluding executive roles, supporting payroll-related use cases.  
- Created a **materialized view** combining product and product type information to support marketing and reporting requirements.

6. **Data Export (PostgreSQL)**
- Exported the results of the SQL view and materialized view as CSV files.  
- These exports were prepared for consumption by external systems while maintaining a clean and structured format.

7. **Data Import (MySQL)**
- Imported the exported CSV files into separate MySQL databases for payroll and marketing use cases.  
- The imported tables were explored and verified to ensure data availability, structure, and consistency, completing the cross-database integration workflow.

---

## 📊 Results

The following results highlight the key stages of the database design and implementation process, including schema modeling, normalization, and data integration across PostgreSQL and MySQL.

## 🐘 PostgreSQL


| 1. Initial ERD |
|-------------|
| ![Initial ERD](Results/coffee_db_initial_ERD.png) |
| Initial entity-relationship diagram representing the raw schema design. |


| 2. Normalized Tables ERD |
|----------------|
| ![Normalized ERD](Results/normalize_tables_ERD.png) |
| Normalized tables ERD after restructuring tables and defining relationships. |


| 3. Coffee Shop Database Tables |
|-------------------|
| ![PostgreSQL Tables](Results/coffee_db_tables.png) |
| Coffee shop database tables successfully created in PostgreSQL. |


| 4. Sales Detail Data |
|-------------------|
| ![Sales Detail Data](Results/sales_detail_first_100_rows.png) |
| Sample transactional data from the sales_detail table. |


| 5. Staff Locations View |
|----------------------|
| ![Staff Locations View](Results/staff_locations_view.png) |
| SQL view displaying staff and work location data. |


| 6. Product Info Materialized View |
|--------------------------------|
| ![Product Info Materialized View](Results/product_info_materialized_view.png) |
| Materialized view combining product and product type information. |


---

## 🐬 MySQL


| 1. Staff Locations |
|-----------------------|
| ![MySQL Staff Locations](Results/staff_locations_table.png) |
| Staff location data imported into MySQL for payroll use. |


| 2. Product Information |
|---------------------------|
| ![MySQL Product Info](Results/product_info.png) |
| Product information imported into MySQL for marketing purposes. |

---

## ℹ️ About This Project

This project was developed as part of the **IBM Data Engineering Professional Specialization** and has been adapted and structured as a **general portfolio project** to demonstrate practical relational database design and implementation skills.

---
