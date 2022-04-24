# SQL-Practice-2-by-Muskan

CREATE DATABASE INSTITUDE
USE INSTITUDE

CREATE TABLE Employee_Detail(Emp_ID int primary key identity,Emp_Name varchar(30),
Emp_salary money, Emp_Dept varchar(30),Emp_Gender varchar(20),Dept_no int,Emp_job varchar(30))

INSERT INTO Employee_Detail values
('Vandana',25000,'Payroll','Female',1,'Clerk'),
('Rohini',35000,'HR','Female',4,'Manager'),
('Prakash',38000,'CA','Male',5,'Accountant'),
('Siya',40000,'IT','Female',3,'TM'),
('Om',44000,'IT','Male',6,'TL'),
('Shivay',45000,'HR','Male',8,'TM'),
('Punkaj',50000,'Transpotation','Male',7,'Driver')


select emp_name ,emp_salary/12  Monthly_salary from Employee_Detail

select * from Employee_Detail where dept_no=3or dept_no=6

select * from Employee_Detail where dept_no=5 and emp_salary>25000

select * from Employee_Detail where emp_Job not in ('Driver','Clerk')

select * from Employee_Detail where emp_Name in ('Prakash','Vandana','Om','Shivay')

select * from Employee_Detail where emp_name like 'r%' and emp_name like '______'

select * from Employee_Detail where emp_Name like '%y' 

select count(emp_salary/12) monthly_salry,COUNT(emp_salary) 
annual_salary from Employee_Detail

select emp_salary as Total_Salary from Employee_Detail

select * from  Employee_Detail where  emp_salary = any
(select emp_salary from Employee_Detail where emp_salary<45000)

select emp_Name,emp_salary from Employee_Detail where emp_salary<45000

select * from Employee_Detail where Emp_Salary<38000

