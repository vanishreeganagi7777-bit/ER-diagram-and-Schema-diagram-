# ER-diagram-and-Schema-diagram-#
Company Database Design – ER Diagram & Schema

## Overview
This repository contains the database design for a **Company Management System**, including:

- **Entity Relationship (ER) Diagram**
- **Relational Schema Diagram**
- Core database structure for managing employees, branches, clients, suppliers, and sales relationships.

The project demonstrates how real-world business operations can be modeled using database concepts.

---

## Project Files
The ER Diagram represents the entities, attributes, and relationships in the company database.

Main Entities
Employee
Branch
Client
Branch Supplier
Relationships
Works For → Employee works for a branch
Manages → Employee manages a branch
Handles → Branch handles clients
Works With → Employee works with clients
Supplies → Supplier supplies branches
Supervision → Employee supervises other employees
Relational Schema

The schema converts the ER model into database tables.

Tables Included
Employee
emp_id (Primary Key)
first_name
last_name
birth_date
sex
salary
super_id (Foreign Key)
branch_id (Foreign Key)
Branch
branch_id (Primary Key)
branch_name
mgr_id (Foreign Key)
mgr_start_date
Client
client_id (Primary Key)
client_name
branch_id (Foreign Key)
Branch Supplier
branch_id (Foreign Key)
supplier_name
supply_type
Works On
emp_id (Foreign Key)
client_id (Foreign Key)
total_sales
Key Concepts Used
Primary Keys
Foreign Keys
One-to-One Relationships
One-to-Many Relationships
Many-to-Many Relationships
Recursive Relationships (Employee supervises Employee)
Purpose of This Project

This project is useful for learning:

Database Management Systems (DBMS)
ER Modeling
Schema Design
SQL Table Relationships
Normalization Basics
Tools Used
Draw.io / Lucidchart / DB Design Tools (for diagrams)
MySQL / PostgreSQL (for implementation)
Future Enhancements
Add SQL CREATE TABLE scripts
Insert sample records
Write JOIN queries
Build frontend dashboard
Integrate with backend APIs
