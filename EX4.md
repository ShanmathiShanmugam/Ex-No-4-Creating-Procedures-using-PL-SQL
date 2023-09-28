# Ex. No: 4 Creating Procedures using PL/SQL

### AIM: To create a procedure using PL/SQL.

### Steps:
1. Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);
2. Create a procedure named as insert_employee data.
3. Inside the procdure block, write the query for inserting the values into the employee table.
4. End the procedure.
5. Call the insert_employee data procedure to insert the values into the employee table.
6. Display the employee table

### Program:
## Create table:
create table employee_1(empid number,empname varchar(10),dept varchar(10),salary number);
## Create procedure:
create or replace procedure insert_employee_data as
begin
insert into employee_1(empid,empname,dept,salary)
values(1,'John','HR',50000);
insert into employee_1(empid,empname,dept,salary)
values(2,'Bob','Finance',55000);
insert into employee_1(empid,empname,dept,salary)
values(3,'Joe','IT',60000);
commit;
end;
/
## Procedure call:
begin
insert_employee_data;
end;
/
## Display table:
select * from employee_1;

### Output:
![image](https://github.com/dineshgl/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/121243595/1835b096-6049-4c21-8696-b7fc933d9dde)
![image](https://github.com/dineshgl/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/121243595/f19bb7c1-bbd3-4ca7-95e1-b797a45eccae)
![image](https://github.com/dineshgl/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/121243595/11f30d7e-d002-4663-9c8f-f520eeb199a9)

### Result:
The procedure is created using PL/SQL and got the output successfully.
