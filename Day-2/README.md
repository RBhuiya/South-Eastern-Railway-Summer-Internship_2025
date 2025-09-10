# 🚂 Day 2 – Oracle 11g SQL*Plus: Creating Tablespace, User, and Granting DBA Access 🛤️

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
