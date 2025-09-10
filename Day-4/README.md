# 🚂 Day 4 – Database Table Definitions and Data Insertions 🛤️

This document outlines the creation of **four master and transactional tables** for managing department, division, and employee information in Oracle 11g, along with **sample data insertions**.
- CREATE TABLE Dept
![CREATE TABLE Dept.png
](https://github.com/RBhuiya/South-Eastern-Railway-Summer-Internship_2025/blob/4bdf225a26614e5d07006b5fdb1906e1afbd78af/All%20Screenshots/Day-4/CREATE%20TABLE%20Dept.png)

- CREATE TABLE Division Master 
![CREATE TABLE Division Master.png](https://github.com/RBhuiya/South-Eastern-Railway-Summer-Internship_2025/blob/59231100ed2b3a44e94c14742b47dd43c6667883/All%20Screenshots/Day-4/CREATE%20TABLE%20Division%20Master.png)

- CREATE TABLE Employee_Info
![CREATE TABLE Employee_Info, Employ_details.png](https://github.com/RBhuiya/South-Eastern-Railway-Summer-Internship_2025/blob/2bee0d0d4b2f250909a2349cda529daf2d9b0af3/All%20Screenshots/Day-4/CREATE%20TABLE%20Employee_Info%2C%20Employ_details.png)

- Employee Details Table
![INSERT Employee_Details (2).png](https://github.com/RBhuiya/South-Eastern-Railway-Summer-Internship_2025/blob/adf85c112c66767bda0b9b72d717b5c1e4ef42d3/All%20Screenshots/Day-4/INSERT%20Employee_Details%20(2).png)


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
![INSERT Employee_Details (2).png](https://github.com/RBhuiya/South-Eastern-Railway-Summer-Internship_2025/blob/adf85c112c66767bda0b9b72d717b5c1e4ef42d3/All%20Screenshots/Day-4/INSERT%20Employee_Details%20(2).png)

# ✅ TABLE CREATION: COMPLETED

---

## 📝 Data Insertions

---


## 📌 5. Insert Records into Dept Table

### ✅ Syntax:
```sql
INSERT INTO Dept (dept_id, dept_name, Divn_id)
VALUES (<dept_id_value>, '<dept_name_value>', <Divn_id_value>);
```
### 💡 Examples:
```sql
INSERT INTO Dept VALUES (101, 'Human Resources', 1);
INSERT INTO Dept VALUES (102, 'Finance', 4);
INSERT INTO Dept VALUES (103, 'IT', 2);
INSERT INTO Dept VALUES (104, 'Corporate', 3);
```

#### 🖥️ **Output**
![INSERTT INTO Dept.png](https://github.com/RBhuiya/South-Eastern-Railway-Summer-Internship_2025/blob/869dfda11f71937a39c174f4eab93a40efa0c643/All%20Screenshots/Day-4/INSERTT%20INTO%20Dept.png)

---

## 📌 6. Insert Records into Division_Master Table

### ✅ Syntax:
```sql
INSERT INTO Division_Master (Divn_id, Divn_name, LOC)
VALUES (<Divn_id_value>, '<Divn_name_value>', '<LOC_value>');
```
### 💡 Examples:
```sql
INSERT INTO Division_Master VALUES (1, 'Human Resources', 'Howrah');
INSERT INTO Division_Master VALUES (2, 'IT', 'BNR');
INSERT INTO Division_Master VALUES (3, 'Corporate', 'Bandel');
```

#### 🖥️ **Output**
![INSERT Employee_Details.png](https://github.com/RBhuiya/South-Eastern-Railway-Summer-Internship_2025/blob/344f98a82b3d44696fc4373f9f8d5aa48c3b5ab2/All%20Screenshots/Day-4/INSERT%20Employee_Details.png)

---

## 📌 7. Insert Records into Employ_Details Table

### ✅ Syntax:
```sql
INSERT INTO Employ_Details (emp_id, divn_id, dept_id, Basic_Pay)
VALUES (<emp_id>, <divn_id>, <dept_id>, <Basic_Pay>);
```
### 💡 Examples:
```sql
INSERT INTO Employ_Details VALUES (101 ,2 ,103 , 61000.50);
INSERT INTO Employ_Details VALUES (102 ,2 ,103 , 61000.50);
INSERT INTO Employ_Details VALUES (103 ,2 ,103 , 50000.00);
INSERT INTO Employ_Details VALUES (104 ,2 ,103 , 70000.00);
INSERT INTO Employ_Details VALUES (105 ,2 ,103 , 75000.10);
INSERT INTO Employ_Details VALUES (106 ,2 ,103 , 96000.50);
INSERT INTO Employ_Details VALUES (107 ,3 ,104 , 72500.00);
INSERT INTO Employ_Details VALUES (108 ,3 ,104 , 72500.00);
INSERT INTO Employ_Details VALUES (109 ,3 ,104 , 66245.10);
INSERT INTO Employ_Details VALUES (110 ,3 ,104 , 42500.20);
INSERT INTO Employ_Details VALUES (111 ,3 ,104 , 57100.40);
INSERT INTO Employ_Details VALUES (112 ,3 ,104 , 79990.00);
INSERT INTO Employ_Details VALUES (113 ,1 ,101 , 22500.00);
INSERT INTO Employ_Details VALUES (114 ,1 ,101 , 40000.00);
INSERT INTO Employ_Details VALUES (115 ,1 ,101 , 22500.00);
INSERT INTO Employ_Details VALUES (116 ,1 ,101 , 42143.50);
```

#### 🖥️ **Output**
![INSERT Employee_Info (2).png](https://github.com/RBhuiya/South-Eastern-Railway-Summer-Internship_2025/blob/b343842da7e0da577093b79c220742d23480d5e7/All%20Screenshots/Day-4/INSERT%20Employee_Info%20(2).png)

---

# ✅ DATA INSERTION: COMPLETED

---

# 📌 Summary

- On Day 4, we successfully:
    - Created 4 database tables for managing employee, department, and division data
    - Inserted sample data into these tables
    - Understood the fundamentals of relational data structures and SQL DML operations

---

# 👨‍💼Author
Mr. Rahul Bhuiya | 4th year CSE-AIML student at MCKVIE'26🎓
