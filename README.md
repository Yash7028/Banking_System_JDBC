
1) Accounts Class:-
   - open_account()
   - get_account_number()
   - generate_account_number()
   - account_exists()
2) User Class :-
   - register()
   - login()
   - user_exist()
3) Account Manager Class:-
   - credit_money()
   - debit_money()
   - transfer_money()
   - check_balance()
4) Banking App Class :- Main Method
   - main menu
   - create instances
   - setup connection with db
   - load drivers

Database :-
1) create database banking_system;
2) create table accounts(
   -> account_number bigint PRIMARY KEY,
   -> full_name varchar(255),
   -> email varchar(255) UNIQUE,
   -> balance decimal(10, 2),
   -> security_pin char(4)
   -> );
   describe accounts;
   +----------------+---------------+------+-----+---------+-------+
   | Field          | Type          | Null | Key | Default | Extra |
   +----------------+---------------+------+-----+---------+-------+
   | account_number | bigint        | NO   | PRI | NULL    |       |
   | full_name      | varchar(255)  | YES  |     | NULL    |       |
   | email          | varchar(255)  | YES  | UNI | NULL    |       |
   | balance        | decimal(10,2) | YES  |     | NULL    |       |
   | security_pin   | char(4)       | YES  |     | NULL    |       |
   +----------------+---------------+------+-----+---------+-------+
3) create table user(
   -> full_name varchar(255),
   -> email varchar(255) PRIMARY KEY,
   -> password varchar(255)
   -> );
   describe user;
   +-----------+--------------+------+-----+---------+-------+
   | Field     | Type         | Null | Key | Default | Extra |
   +-----------+--------------+------+-----+---------+-------+
   | full_name | varchar(255) | YES  |     | NULL    |       |
   | email     | varchar(255) | NO   | PRI | NULL    |       |
   | password  | varchar(255) | YES  |     | NULL    |       |
   +-----------+--------------+------+-----+---------+-------+
   

