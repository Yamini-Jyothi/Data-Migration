# Data-Migration

COMPANY:CODTECH IT SOLUTIONS

NAME:Yamini Polumolu

INTERN ID:CT12WMXI

DOMAIN:SQL

BATCH DURATION:January 15th, 2025 to April 15th, 2025

MENTOR NAME:NEELA SANTHOSH

DESCRIPTION OF THE TASK Here is the expanded text: Transferring Data from MySQL to PostgreSQL using pgLoader pgLoader is a powerful tool for transferring data between different databases, including MySQL and PostgreSQL. In this example, we will use pgLoader to transfer the employee table from a MySQL database to a PostgreSQL database.

Installing pgLoader: To use pgLoader, you need to install it on your system. You can install pgLoader using the following command: sudo apt-get install pgLoader Creating a PostgreSQL Database Before transferring the data, you need to create a PostgreSQL database to store the data. You can create a database using the following command: CREATE DATABASE employee_db; Creating a pgLoader Configuration File To transfer the data, you need to create a pgLoader configuration file that specifies the source and target databases, as well as the tables to be transferred. Create a file named pgloader.conf with the following contents:

LOAD DATABASE: FROM mysql://username:password@localhost/employee_db INTO postgresql://username:password@localhost/employee_db WITH include drop, create tables, constraints, indexes, reset sequences SET work_mem to '16MB', maintenance_work_mem to '64MB'; Replace the username, password, and localhost placeholders with the actual values for your MySQL and PostgreSQL databases. Running pgLoader To transfer the data, run the following command: pgloader pgloader.conf pgLoader will transfer the employee table from the MySQL database to the PostgreSQL database.

Verifying the Data Transfer: To verify that the data has been transferred successfully, you can use the following SQL command to retrieve the data from the PostgreSQL database: SELECT * FROM employee LIMIT 10; This command will retrieve the first 10 rows of the employee table from the PostgreSQL database. Troubleshooting Common Issues When using pgLoader, you may encounter some common issues. Here are a few troubleshooting tips:

Make sure that the username and password are correct for both the MySQL and PostgreSQL databases.
Ensure that the database names and table names match exactly between the two databases.
Check the pgLoader configuration file for any syntax errors or typos.
Conclusion: In this example, we used pgLoader to transfer the employee table from a MySQL database to a PostgreSQL database. pgLoader provides a powerful and flexible way to transfer data between different databases, making it an ideal tool for data migration and integration tasks. By following these steps and troubleshooting common issues, you can use pgLoader to transfer data between MySQL and PostgreSQL databases with ease.

#Output of the Task

![Image](https://github.com/user-attachments/assets/2e1d5c86-2410-424f-9c0b-f93501a2aab3)

![Image](https://github.com/user-attachments/assets/a5cc8905-3740-412d-96df-331f5fe78078)
