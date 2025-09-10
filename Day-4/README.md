# 🚂 Day 4 – Database Table Definitions and Data Insertions 🛤️

This document outlines the creation of **four master and transactional tables** for managing department, division, and employee information in Oracle 11g, along with **sample data insertions**.

---

## 🎯 Objectives

- Define master and transactional tables in Oracle 11g  
- Create table structures using SQL  
- Insert sample records to simulate real-world data  
- Understand primary keys, foreign keys, and relational data structure

---

## 🧱 1. Department Master Table

### ✅ Table Creation Syntax
```sql
CREATE TABLE Dept (
    dept_id   NUMBER(3) NOT NULL,
    dept_name VARCHAR2(50),
    Divn_id   NUMBER(3)
);
```
#### 🖥️ **Output**

