# demo_login
e_banking login service
## install software required for running this project  
- Java17  
- intellij idea, version 2023.1.2  
- postman or any other api test platform  
## run the project  
1. open intellij idea  
2. check if the project associate with mysql or else run the following commends in mysql console  
create database login;
use login;
create table users(id int unsigned primary key auto increment, username varchar(20) unique not null, password varchar(20));  
3. use "insert into" to create users to the table  
4. run the project
5. open api test platform and send POST request to login  
6. an example POST request show as the following  
POST http://localhost:8800/login  
{
  "username":"tom1",
  "password":"123456"
}  
## validation
if the POST request sent successfully and the project sent back a jwt token in json format  
then the project is valid
