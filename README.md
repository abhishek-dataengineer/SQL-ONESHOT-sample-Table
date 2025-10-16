# SQL-ONESHOT-sample-Table


Table-1
-------
CREATE TABLE EMPLOYEE (
	EMP_ID INT,
	NAME VARCHAR,
	DEPT VARCHAR,
	SALARY INT
)

INSERT INTO EMPLOYEE 
	(EMP_ID, NAME, DEPT, SALARY)
	VALUES
	 (101, 'ROHAN', 'HR', 20000),
	 (102, 'ABHISHEK', 'IT', 80000),
	 (103, 'MOHAN', 'MARKETTING', 50000),
	 (104, 'KUMAR', 'HR', 25000),
	 (105, 'MADHAV', 'IT', 90000)




Table-2
-------
-- Create Departments table
CREATE TABLE Departments (
    dept_id INT PRIMARY KEY,
    dept_name VARCHAR(50)
);

-- Create Employees table
CREATE TABLE Employees (
    emp_id INT PRIMARY KEY,
    emp_name VARCHAR(50),
    dept_id INT,
    salary DECIMAL(10,2)
);

-- Insert into Departments
INSERT INTO Departments (dept_id, dept_name) VALUES
(1, 'HR'),
(2, 'Finance'),
(3, 'IT'),
(4, 'Sales');

-- Insert into Employees
INSERT INTO Employees (emp_id, emp_name, dept_id, salary) VALUES
(101, 'Alice', 1, 50000),
(102, 'Bob', 2, 60000),
(103, 'Charlie', 3, 70000),
(104, 'David', NULL, 45000),   
(105, 'Eva', 3, 72000),
(106, 'Frank', 5, 55000);      





Table-3 (String & Date Functions)
---------------------------------

-- Create Employees_Info table
CREATE TABLE Employees_Info (
    emp_id INT PRIMARY KEY,
    emp_name VARCHAR(50),
    joining_date DATE,
    designation VARCHAR(50)
);

-- Insert sample data
INSERT INTO Employees_Info (emp_id, emp_name, joining_date, designation) VALUES
(1, 'Alice Johnson', '2020-01-15', 'Manager'),
(2, 'Bob Smith', '2019-05-20', 'Analyst'),
(3, 'Charlie Brown', '2021-07-10', 'Developer'),
(4, 'David Miller', '2023-02-01', 'Intern'),
(5, 'Eva White', '2022-11-25', 'Tester');



Table-4 (Window Functions)
-----------------------------
CREATE TABLE Sales (
    sale_id INT PRIMARY KEY,
    emp_name VARCHAR(50),
    department VARCHAR(50),
    sale_amount DECIMAL(10,2),
    sale_date DATE
);

INSERT INTO Sales VALUES
(1, 'Alice', 'IT', 500, '2023-01-05'),
(2, 'Bob', 'Finance', 300, '2023-01-06'),
(3, 'Alice', 'IT', 700, '2023-01-07'),
(4, 'Charlie', 'Finance', 400, '2023-01-07'),
(5, 'Bob', 'Finance', 200, '2023-01-08'),
(6, 'Alice', 'IT', 600, '2023-01-09'),
(7, 'Charlie', 'Finance', 900, '2023-01-10'),
(8, 'David', 'IT', 1000, '2023-01-11');




   
