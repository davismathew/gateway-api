

# NRM gateway Api

## Getting Started

git clone https://github.com/sinergiamedialabs/WestPharma_HTML.git

yarn

yarn start

### Prerequisites
node 9.0.*
mysql server

### db structure
db name :nrm
db user: root
db pwd: sinergialabs

#### table
1.user
2.login
3.dashboard

#### user
Field   | Type         | Null | Key | Default | Extra          |
+---------+--------------+------+-----+---------+----------------+
| ID      | int(11)      | NO   | PRI | NULL    | auto_increment |
| phone   | varchar(35)  | NO   | UNI | NULL    |                |
| email   | varchar(55)  | NO   | UNI | NULL    |                |
| address | varchar(255) | YES  | UNI | NULL    |                |
| name    | varchar(100) | NO   |     | NULL    |                |
+---------+--------------+------+-----+---------+------------

#### login
Field    | Type         | Null | Key | Default | Extra          |
+----------+--------------+------+-----+---------+----------------+
| ID       | int(11)      | NO   | PRI | NULL    | auto_increment |
| password | varchar(255) | NO   |     | NULL    |                |
| userid   | int(11)      | NO   | UNI | NULL    |                |
| username | varchar(100) | YES  | UNI | NULL    |         

#### dashboard

Field     | Type           | Null | Key | Default | Extra          |
+-----------+----------------+------+-----+---------+----------------+
| ID        | int(11)        | NO   | PRI | NULL    | auto_increment |
| userid    | int(11)        | NO   |     | NULL    |                |
| username  | varchar(100)   | NO   |     | NULL    |                |
| env       | varchar(100)   | YES  |     | NULL    |                |
| name      | varchar(100)   | YES  |     | NULL    |                |
| dashboard | varchar(10000) | YES  |     | NULL    |                

