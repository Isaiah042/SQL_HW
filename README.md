# SQL_HW

 use world
Database changed
mysql> show tables;
+-----------------+
| Tables_in_world |
+-----------------+
| city            |
| country         |
| countrylanguage |
+-----------------+
3 rows in set (0.00 sec)

mysql> Select COUNT(*) AS cities from city where CountryCode='USA';
+--------+
| cities |
+--------+
|    274 |
+--------+
1 row in set (0.02 sec)
