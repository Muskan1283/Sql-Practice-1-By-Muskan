# Sql-Practice-1-By-Muskan

 create database Detail
 use Detail
 create table Employee_Detail(id int primary key identity(101,1),F_Name varchar(80),L_Name varchar(50),
 salary int,Department_Name varchar(60),Gender varchar(20))

 INSERT INTO Employee_Detail values
 ('Raju','Singh',20000,'IT','Male'),
('nittu','kUMARI',25000,'HR','Female'),
 ('Mohan','Ram',20000,'IT','Male'),
 ('Rajiv','Gopal',15000,'HR','Male'),
 ('Devika','Kumari',10000,'IT','Female'),
 ('Vikas','Kumar',9000,'IT','Male'),
 ('Rubi','Rani',8000,'IT','Female')

 ALTER TABLE Employee_Detail ADD DEPT_NO INT 

 UPDATE Employee_Detail SET DEPT_NO=8 WHERE id=101
  UPDATE Employee_Detail SET DEPT_NO=9 WHERE id=102
   UPDATE Employee_Detail SET DEPT_NO=10 WHERE id=103
  UPDATE Employee_Detail SET DEPT_NO=12 WHERE id=104
   UPDATE Employee_Detail SET DEPT_NO=13 WHERE id=105
    UPDATE Employee_Detail SET DEPT_NO=14 WHERE id=106
	 UPDATE Employee_Detail SET DEPT_NO=15 WHERE id=107

 select*from Employee_Detail

 select*from Employee_Detail where salary<10000

 select*from Employee_Detail where salary>=9000 AND salary<15000 


 select*from Employee_Detail where salary NOT BETWEEN 9000 AND 15000


 select*from Employee_Detail where F_Name LIKE 'r%'

select*from Employee_Detail where F_Name LIKE '%u'

select*from Employee_Detail where F_Name LIKE '%a%'

select*from Employee_Detail where F_Name LIKE '____'

select*from Employee_Detail where F_Name LIKE '%r%' AND salary>9000 

select*from Employee_Detail where salary>
(select salary from Employee_Detail where F_Name='raju')

select*from Employee_Detail where id like '1%1'


 UPDATE Employee_Detail SET DEPT_NO=10 WHERE id IN(101,103,107)

UPDATE Employee_Detail SET DEPT_NO=8 WHERE id=101


-----UPDATE Employee_Detail SET DEPT_NO=NULL WHERE id=101-------

UPDATE Employee_Detail SET DEPT_NO=20 WHERE  DEPT_NO=null

UPDATE Employee_Detail SET SALARY=20000 WHERE DEPT_NO>10 and F_Name LIKE 'R%'

UPDATE Employee_Detail SET DEPT_NO=30 WHERE F_Name LIKE 'm%'

UPDATE Employee_Detail SET salary=8500 WHERE dept_no not between 10 and 30

select*from Employee_Detail

 UPDATE Employee_Detail SET SALARY=15000 WHERE DEPT_NO>10 and F_Name LIKE 'R%'

  UPDATE Employee_Detail SET SALARY=5500 WHERE DEPT_NO<20 and id>105


UPDATE Employee_Detail SET SALARY=25000 WHERE SALARY<10000 and F_Name LIKE '%R%' and  DEPT_NO<20 


UPDATE Employee_Detail SET SALARY=10000 WHERE SALARY>=8500 and  SALARY<=15000
