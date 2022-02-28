# Mysql-server-Installation---Ubuntu20.04

Sudo apt update

sudo apt install mysql-sever

mysql --version

sudo mysql_secure_installation

sudo mysql    no password ask

select user, authentication_string, plugin from mysql.user;

mysql> ALTER USER 'root'@'localhost' IDENTIFIED WITH caching_sha2_password BY 'root';

mysql> FLUSH PRIVILEGES;  to update the changes using command

select user, authentication_string, plugin from mysql.user; #to check authentication_string to caching_sha2_password BY in root

Now exit from and run sudo mysql ....And Access denied will pop up 

To go with password -----sudo mysql -u root -p

So, you are able to connect mysql and text Show Databases;

Next steps to conect MySQL Workbench using this database.

Now download MySQL Workbench Community edition from Ubuntu software.
