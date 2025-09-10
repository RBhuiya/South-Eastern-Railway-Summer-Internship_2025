# 🚂 Day 2 – Oracle 11g SQL*Plus Creating Tablespace, User and Granting DBA Access 🛤️

![Create Table.png](https://github.com/RBhuiya/South-Eastern-Railway-Summer-Internship_2025/blob/6c3d3959954027579af1249e9ecafb66e0231e28/All%20Screenshots/Day-2/Create%20Table.png)
---

## 🎯 Objectives
By the end of this session, you will have learned how to:
- Create a **tablespace** in Oracle 11g
- Create a new **database user**
- Grant **DBA privileges** to the user using SQL*Plus

---

## 🛠️ Step-by-Step Guide

---

### 📌 Step 1: Create a Tablespace
#### 🔤 **Syntax**
```sql
CREATE TABLESPACE <tablespace_name>
DATAFILE '<oracle_install_path>\orcl01.dbf'
SIZE 1024M 
AUTOEXTEND ON;
```
#### 🖥️ **Output**
 
![Create Table.png](https://github.com/RBhuiya/South-Eastern-Railway-Summer-Internship_2025/blob/6c3d3959954027579af1249e9ecafb66e0231e28/All%20Screenshots/Day-2/Create%20Table.png)

---

### 📌 Step 2: Create a New User
#### 🔤 **Syntax**
```sql
CREATE USER rahul_1 
IDENTIFIED BY Orcl123 
DEFAULT TABLESPACE t1 
TEMPORARY TABLESPACE temp;
```
#### 🖥️ **Output**
 
![Create User, Grand Permission to DBA.png](https://github.com/RBhuiya/South-Eastern-Railway-Summer-Internship_2025/blob/6c3d3959954027579af1249e9ecafb66e0231e28/All%20Screenshots/Day-2/Create%20Table.png](https://github.com/RBhuiya/South-Eastern-Railway-Summer-Internship_2025/blob/bfa2849a9ad9c61c0cac0c4d81e36b9aa74debf7/All%20Screenshots/Day-2/Create%20User%2C%20Grand%20Permission%20to%20DBA.png)
