# Datatypes

1. String Datatypes:
   1. Char(0 - 255)
   2. Varchar(0 - 65535) 
   3. Text(0 - 65535)
   4. Enum(65535)
   5. Blob(65535)
2. Numeric Datatypes:
   1. Int (255)
   2. Integer
   3. Float
   4. Double
   5. Bool 
3. Date and Time Datatypes
   1. Date
   2. DateTime
   3. TimeStamp
   4. Time
   5. Year
   - Format: 
     - Date= YYYY-MM-DD 
     - Time= HH:MM:SS  
     - DateTime= YYYY-MM-DD hh:mm:ss
     - TimeStamp:TimeZone- UTC+05:30
  
# SQL Commands :- 
   ### DDL - Data Definiton Language 
      (CREATE, DROP, ALTER, TRUNCATE, RENAME)
   ### DML - Data Manipulation Language 
      (INSERT, UPDATE, DELETE, CALL, LOCK)
   ### TCL - Transaction Control Language 
      (COMMIT, SAVEPOINT,ROLLBACK, SET TRANSACTION, SET CONSTRAINT)
   ### DQL - Data Query Language 
      (SELECT)
   ### DCL - Data Control Language 
      (GRANT, REVOKE) 

# CRUD :- Create, Read, Update, Delete
   ```sh
   1. Create Database Database_Name;
   2. Create Table Table_Name(Column1_Name datatype, Column2_Name datatype, Column3_Name datatype, ......);
   3. Insert into Table_Name(Column1_Name datatype, Column2_Name datatype, Column3_Name datatype, ......) values(Column1_Value, Column2_Value, Column3_Value, ......);
   4. Insert Multiple rows in single querry: () <- A single Tupple == Row
      1. Insert into Table_Name(Column1_Name datatype),(Column1_Name datatype),(Column1_Name datatype);
   5. Select * from Table_Name;
   6. Update Table_Name set column_name=value where condition;
   7. Delete from Table_Name where condition;
   ```

## Practice Activity:
   ```sh
      Create Database Rushi;
      Use Rushi;
      Create TABLE Student(id int(10), name varchar(100));
      Insert into Student(id, name) values(101,"abcd");
      Select * from Student;
      Update student set name="xyz" where id=101;
      Delete from Student where id=101;
      DROP TABLE Student;
      DROP DATABASE rushi;
   ```