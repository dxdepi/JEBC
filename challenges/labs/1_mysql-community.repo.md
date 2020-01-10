## Hostname MySQL Server
```
mysql> select @@hostname;
+--------------------------------------------------+
| @@hostname                                       |
+--------------------------------------------------+
| ip-172-31-25-172.ap-southeast-1.compute.internal |
+--------------------------------------------------+
1 row in set (0.00 sec)

mysql> show variables where Variable_name like '%host%';
+-------------------------------+--------------------------------------------------+
| Variable_name                 | Value                                            |
+-------------------------------+--------------------------------------------------+
| host_cache_size               | 342                                              |
| hostname                      | ip-172-31-25-172.ap-southeast-1.compute.internal |
| performance_schema_hosts_size | 100                                              |
| report_host                   |                                                  |
+-------------------------------+--------------------------------------------------+
4 rows in set (0.00 sec)
```
## MySQL Version
```
[centos@ip-172-31-25-172 mysql-connector-java-5.1.48]$ mysql --version
mysql  Ver 14.14 Distrib 5.6.46, for Linux (x86_64) using  EditLine wrapper
```
## MySQL Database 
```
ql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| amon               |
| hue                |
| metastore          |
| mysql              |
| nav                |
| navms              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
| sentry             |
+--------------------+
12 rows in set (0.00 sec)
```
