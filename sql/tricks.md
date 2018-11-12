
### GroupBy Example
```
mysql> select * from customer ;
+-----------+---------+
| customers | product |
+-----------+---------+
|         1 | a       |
|         1 | b       |
|         2 | c       |
|         2 | d       |
|         3 | e       |
+-----------+---------+
5 rows in set (0.00 sec)

mysql> select customers,product, count(product) from customer group by customers ;
+-----------+---------+----------------+
| customers | product | count(product) |
+-----------+---------+----------------+
|         1 | a       |              2 |
|         2 | c       |              2 |
|         3 | e       |              1 |
+-----------+---------+----------------+
3 rows in set (0.00 sec)
```
