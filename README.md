# dbms-sql
-- Create the table 'dss' with appropriate column definitions
/*CREATE TABLE dss (
    id INT(4),
    Name VARCHAR(25),
    no INT(1)
);
-- Insert data into the 'dss' table using the INSERT INTO ... VALUES syntax for multiple rows
INSERT into dss VALUES (1, 'aa', 2),(2, 'aaa', 7);
Alter table dss ADD  (AGE int(3),COURSE varchar(40));
Alter table dss 
Drop column id;
ALTER TABLE dss
ADD ids INT(10) FIRST; -- ALSO USED AFTER ANY_COLUMN NAME
select *from dss;
*/
create database  Db;
use Db;
create table emp_info(id int (10) not null , Primary key(id), Name varchar(24), Salary int  default(20));
insert into emp_info(id, Name, Salary) 
values(1, 'aadam', 25000),
(2,'bob',30000),
(3,'casey', 40000),
(4,'anaya', 2900),
(5,'aaya', 2900),
(6,'anya', 2900);
ALTER table emp_info ADD (age int(4), address varchar(100), details int default 20000) ;
/*--drop database Db;
Truncate table emp_info;*/
ALTER table emp_info
RENAME to onnn; /* change table name*/
ALTER TABLE onnn ADD
(info varchar(100), itm varchar(100) default 1, taxam int(100));
Update onnn Set Name='bb' where Salary=30000;/*update  tablename set column='updatevale' where column='value beforehavein table'; */


/*select *from onnn where Salary >2500 LIMIT 2; -- select student in salary  above 2500 only 2 student*/

select *from onnn order by salary DESC LIMIT 4;  /* ORDER BY clasue used asc-> ascending order or desc->descending order   LIMIT-> ONLY ACCESS VALUE 4*/


