# Essential_SQL_for_Data_Engineers
Complete the following and submit your SQL Queries
Problems in a Word File:

Data Source: https://www.mysqltutorial.org/mysql-sample-database.aspx

Write queries of the following question using the database used in class


1. Order count for each productline where orders are more than 100 (Hint: Use Having)

2. Count of employees against each manager name (Hint: Use Self Join)

3. For each city, create individual columns of order count by each Order Status available in Database (Hint: Use CASE)

4. For each office total order sold (Using Multiple Joins)

5. For each Employee total order sold (Exclude those Employees which are in USA) (Use Sub-Query in Where)

6. 2nd highest selling product for each Productline. (Use Window Function & CTE Approach)



Section 2:  

You have already inserted Data from Financial Consumer Complaints ETL Assignment, use the same table to create some Procedures, Triggers and Views

Data Source: Financial Consumer Complaints Data inserted in Airflow Assignment. (Incase you haven't submitted the Airflow assignment then you can use the attached script to create table in your MySQL Database)

Create the Following Database Objects:

1.       Creating a View :

Create a view “complaints_last_3_months_sum” of Number of Complaints received against the following attributes in last three months use “date_received” column, use the Original Table & Data you have from Airflow Assignment Dump:

1.       state
2.       product
3.       issue
4.       sub_product
5.       sub_issue

2.       Creating a Procedure :

Create a procedure that intakes a Date Parameter and uses it to migrate data from Original table to another table for all the Complaints received in Last 3 Months use “date_received” column to replicate data into another table. Name the table as “complaints_last_3_months”

For Example if the Parameter Date is 28-Feb-2023 then the Data pulled from one table to the another must be between 01-DEC-22 to 28-FEB-23

Table to Migrate from: use the Original Table & Data you have from Airflow Assignment Dump

Table to Migrate to: “complaints_last_3_months”

3.       Creating a Trigger  

Create a trigger that updates “complaints_last_3_months” table with new record whenever the data is inserted in original financial consumer complaints table based on same criteria of Complaints received in Last 3 Months use “date_received” column. (Hint: On Insert Trigger will be used)


