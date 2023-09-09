# EXP 1: DATA DEFENITION LANGUGE COMMANDS IN RDBMS

## AIM:
To create a student database and execute DDL queries using SQL.

## DDL (Data Definition Language)
DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. DDL is a set of SQL commands used to create, modify, and delete database structures but not data. These commands are normally not used by a general user, who should be accessing the database via an application.

## List of DDL commands: 

CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
DROP: This command is used to delete objects from the database.
ALTER: This is used to alter the structure of the database.
TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed.
RENAME: This is used to rename an object existing in the database.

## Query:
1) Create a table student with the following fieds rollno,name,age,address,phoneno.

### SQL QUERY: 
CREATE TABLE stu ( rollno INT PRIMARY KEY,name VARCHAR(255),age INT,address VARCHAR(255),phoneno VARCHAR(15));

### OUTPUT:
![image](https://github.com/MarellaDharanesh/I2_DBMS/assets/118707669/223579b5-413c-4ed3-9590-8ea4791e8428)


2) Change the above student table by adding another attribute department


### SQL QUERY: 
ALTER TABLE student
ADD department VARCHAR(50);

### OUTPUT:
![image](https://github.com/MarellaDharanesh/I2_DBMS/assets/118707669/7fe74064-8795-4397-a9ba-7a5a65b681b2)



3) Drop the student table

### SQL QUERY: 
 DROP TABLE stu;

### OUTPUT:
![image](https://github.com/MarellaDharanesh/I2_DBMS/assets/118707669/e6b532bd-4c99-47c1-8054-c57a1ed74884)


4) Delete the student table using truncate keyword

### SQL QUERY: 
TRUNCATE TABLE stu;

### OUTPUT:
![image](https://github.com/MarellaDharanesh/I2_DBMS/assets/118707669/791b623d-4a5c-4388-a008-0b6cdb352a87)




5) Rename the student table to mystudent

   
### SQL QUERY: 
ALTER TABLE stu RENAME TO mystudent;


### OUTPUT:
![image](https://github.com/MarellaDharanesh/I2_DBMS/assets/118707669/88fc3d82-2fd5-4a75-8280-e1cd1164d16d)
