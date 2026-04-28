### Company Data Storage Requirements

TECHIMPACKT:

The company is organized into branches. Each branch has a unique number, a name, and a particular employee who manages it.

The company makes it’s money by selling to clients. Each client has a name and a unique number to identify it.

The foundation of the company is it’s employees. Each employee has a name, birthday, sex, salary and a unique number.

An employee can work for one branch at a time, and each branch will be managed by one of the employees that work there. We’ll also want to keep track of when the current manager started as manager.

An employee can act as a supervisor for other employees at the branch, an employee may also act as the supervisor for employees at other branches. An employee can have at most one supervisor.

A branch may handle a number of clients, with each client having a name and a unique number to identify it. A single client may only be handled by one branch at a time.

Employees can work with clients controlled by their branch to sell them stuff. If nescessary multiple employees can work with the same client. We’ll want to keep track of how many dollars worth of stuff each employee sells to each client they work with.

Many branches will need to work with suppliers to buy inventory. For each supplier we’ll keep track of their name and the type of product they’re selling the branch. A single supplier may supply products to multiple branches.



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
