### If you don't have MySQL installed on your droplet, you can quickly download it.

#####                                       sudo apt-get install mysql-server

### Once you have MySQL installed on your droplet, you can access the MySQL shell by typing the following command into terminal:

##### mysql -u root -p

### You can quickly check what databases are available by typing:

##### mysql> SHOW DATABASES;

### Creating a database is very easy:

 ##### CREATE DATABASE database name;

### In this case, for example, we will call our database "events."

 ##### mysql> SHOW DATABASES;

### Let’s open up the database we want to use:

##### USE events;

### In the same way that you could check the available databases, you can also see an overview of the tables that the database contains.

##### SHOW tables; 

### Let’s create a new MySQL table:

##### CREATE TABLE potluck (id INT NOT NULL PRIMARY KEY AUTO_INCREMENT, name VARCHAR(20),food VARCHAR(30),confirmed CHAR(1), signup_date DATE);

### If needed, you can also delete rows from the table with the following command:

##### DELETE from [table name] where [column name]=[field text];
