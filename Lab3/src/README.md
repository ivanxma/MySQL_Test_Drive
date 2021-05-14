
## Creating the "demo" database with fruitmart table

1. Ensure "mysqld" service is up and running

# sudo systemctl status mysqld

if it is not up and running, start the service as follows :

`` 
# sudo systemctl start mysqld
``

2. Download the sql files using wget
# cd /tmp
# wget https://github.com/kuanrcl/MySQL_Test_Drive/blob/master/Lab3/src/demo-schema.sql
# wget https://github.com/kuanrcl/MySQL_Test_Drive/blob/master/Lab3/src/demo-data.sql

# mysql -uroot -h127.0.0.1 -P3306 -pMySQL1sGreat! -e “create database if not exists demo;”
# mysql -uroot -h127.0.0.1 -P3306 -pMySQL1sGreat! demo < demo-schema.sql
# mysql -uroot -h127.0.0.1 -P3306 -pMySQL1sGreat! demo < demo-data.sql





