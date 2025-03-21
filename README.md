

# Grocify

Grocify is a robust and efficient desktop-based Grocery Management System developed using Python and MySQL. Designed for grocery store owners and managers, Grocify streamlines inventory tracking, sales management, and customer transactions, ensuring smooth business operations.

# General Instructions
1. The database is to be created manually, tables will be created automatically after first run.

2. [tkinter](https://docs.python.org/3/library/tkinter.html) and [pillow](https://pypi.org/project/Pillow/) modules must be installed on your device to run the program. 

3. The admin account can only be created manually from the MySQL command line. You will need to at least create one admin account to get started with the system.

4. Host, Username, Password is set to the default value, change it according to your device to connect the program with the database.

*NOTE:- There is 23 database connector statement which all need to change according to your device.*

5. *Category, Sub-Category, Products* are to be manually added to the code as well as normally added to the database to execute further instructions in the system. (To manually add items jump to line no: *1538*.)

*NOTE:- Data added to the database is to be the same as the data entered in the source code. Also, space gap is not allowed in sub-categories and products, adding gap may result in an error. Use subtract symbol or underscore instead.*

# Database Information

Database name: *grocify*

```bash
CREATE DATABASE grocify;
```
*Note:- The database is to be created manually.*

# Tables Information

Tables: *admin, customers, employees, invoices, products*

1. admin 
```bash
CREATE TABLE admin (
id int primary key,
username varchar(20),
password varchar(50)
);
```
2. customers 
```bash
CREATE TABLE customers (
customer_name varchar(300),
date varchar(20),
bill_number int,
customer_phn varchar(10)
);
```
3. employees
```bash
CREATE TABLE employees (
employee_id int primary key,
username varchar(20),
password varchar(50),
employee_name varchar(300),
contact_num varchar(10),
address varchar(300),
aadhar_num varchar(12)
);
```
4. invoices
```bash
CREATE TABLE invoices (
bill_number int,
date varchar(20),
customer_name varchar(300),
customer_contact varchar(10)
);
```
5. products
```bash
CREATE TABLE products (
product_id int primary key,
category varchar(300),
sub_category varchar(300),
product_name varchar(300),
stock_quantity int,
MRP int
);
```
*Note:- Tables will be created automatically after first run.*


# Software Requrements
1. [Python 3.12.4](https://www.python.org)
2. [MySQL](https://www.mysql.com/)

## License

[MIT](https://choosealicense.com/licenses/mit/)

