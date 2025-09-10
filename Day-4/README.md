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
![CREATE TABLE Dept.png
](https://github.com/RBhuiya/South-Eastern-Railway-Summer-Internship_2025/blob/4bdf225a26614e5d07006b5fdb1906e1afbd78af/All%20Screenshots/Day-4/CREATE%20TABLE%20Dept.png)

---

## 🧱 2. Division Master Table

### ✅ Table Creation Syntax
```sql
CREATE TABLE Division_Master (
    Divn_id   NUMBER(3) PRIMARY KEY,
    Divn_name VARCHAR2(50),
    LOC       VARCHAR2(100)
);
```
#### 🖥️ **Output**
![CREATE TABLE Division Master.png](https://github.com/RBhuiya/South-Eastern-Railway-Summer-Internship_2025/blob/59231100ed2b3a44e94c14742b47dd43c6667883/All%20Screenshots/Day-4/CREATE%20TABLE%20Division%20Master.png)

---

## 🧱 3. Employee Information Table

### ✅ Table Creation Syntax
```sql
CREATE TABLE Employee_Info (
    Emp_id      NUMBER(10) PRIMARY KEY,
    Group_name  VARCHAR2(50),
    DOB         DATE,
    Mob_NO      VARCHAR2(15),
    email_id    VARCHAR2(100)
);
```
#### 🖥️ **Output**
![CREATE TABLE Employee_Info, Employ_details.png](https://github.com/RBhuiya/South-Eastern-Railway-Summer-Internship_2025/blob/2bee0d0d4b2f250909a2349cda529daf2d9b0af3/All%20Screenshots/Day-4/CREATE%20TABLE%20Employee_Info%2C%20Employ_details.png)

---

## 🧱 4. Employee Details Table

### ✅ Table Creation Syntax
```sql
CREATE TABLE Employ_Details (
    emp_id     NUMBER(5),
    divn_id    NUMBER(3),
    dept_id    NUMBER(3),
    Basic_Pay  NUMBER(10, 2)
);
```
#### 🖥️ **Output**
![]()
