## List Repository
```
[centos@ip-172-31-25-172 ~]$ for node in `cat serverlist`;   do     echo ------------- $node:;         ssh -i depipem.pem centos@$node ls -ltr /etc/yum.repos.d/; done;
------------- 172.31.25.172:
total 44
-rw-r--r--. 1 root   root   1060 Jan 29  2014 mysql-community-source.repo
-rw-r--r--. 1 root   root   1209 Jan 29  2014 mysql-community.repo
-rw-rw-r--. 1 centos centos  290 Dec 13  2018 cloudera-manager.repo
-rw-r--r--. 1 root   root   6639 Sep  5 13:05 CentOS-Vault.repo
-rw-r--r--. 1 root   root   1331 Sep  5 13:05 CentOS-Sources.repo
-rw-r--r--. 1 root   root    630 Sep  5 13:05 CentOS-Media.repo
-rw-r--r--. 1 root   root    314 Sep  5 13:05 CentOS-fasttrack.repo
-rw-r--r--. 1 root   root    649 Sep  5 13:05 CentOS-Debuginfo.repo
-rw-r--r--. 1 root   root   1309 Sep  5 13:05 CentOS-CR.repo
-rw-r--r--. 1 root   root   1664 Sep  5 13:05 CentOS-Base.repo
------------- 172.31.16.171:
total 44
-rw-r--r-- 1 root   root   1060 Jan 29  2014 mysql-community-source.repo
-rw-r--r-- 1 root   root   1209 Jan 29  2014 mysql-community.repo
-rw-rw-r-- 1 centos centos  290 Dec 13  2018 cloudera-manager.repo
-rw-r--r-- 1 root   root   6639 Sep  5 13:05 CentOS-Vault.repo
-rw-r--r-- 1 root   root   1331 Sep  5 13:05 CentOS-Sources.repo
-rw-r--r-- 1 root   root    630 Sep  5 13:05 CentOS-Media.repo
-rw-r--r-- 1 root   root    314 Sep  5 13:05 CentOS-fasttrack.repo
-rw-r--r-- 1 root   root    649 Sep  5 13:05 CentOS-Debuginfo.repo
-rw-r--r-- 1 root   root   1309 Sep  5 13:05 CentOS-CR.repo
-rw-r--r-- 1 root   root   1664 Sep  5 13:05 CentOS-Base.repo
------------- 172.31.30.88:
total 44
-rw-r--r-- 1 root root 1060 Jan 29  2014 mysql-community-source.repo
-rw-r--r-- 1 root root 1209 Jan 29  2014 mysql-community.repo
-rw-r--r-- 1 root root 6639 Sep  5 13:05 CentOS-Vault.repo
-rw-r--r-- 1 root root 1331 Sep  5 13:05 CentOS-Sources.repo
-rw-r--r-- 1 root root  630 Sep  5 13:05 CentOS-Media.repo
-rw-r--r-- 1 root root  314 Sep  5 13:05 CentOS-fasttrack.repo
-rw-r--r-- 1 root root  649 Sep  5 13:05 CentOS-Debuginfo.repo
-rw-r--r-- 1 root root 1309 Sep  5 13:05 CentOS-CR.repo
-rw-r--r-- 1 root root 1664 Sep  5 13:05 CentOS-Base.repo
-rw-r--r-- 1 root root  291 Jan 10 08:47 cloudera-manager.repo
```
## Prepare Database
```
[centos@ip-172-31-16-171 ~]$ sudo /usr/share/cmf/schema/scm_prepare_database.sh mysql -h 172.31.25.172 scm scm
Enter SCM password: 
JAVA_HOME=/usr/java/jdk1.7.0_67-cloudera
Verifying that we can write to /etc/cloudera-scm-server
Creating SCM configuration file in /etc/cloudera-scm-server
Executing:  /usr/java/jdk1.7.0_67-cloudera/bin/java -cp /usr/share/java/mysql-connector-java.jar:/usr/share/java/oracle-connector-java.jar:/usr/share/java/postgresql-connector-java.jar:/usr/share/cmf/schema/../lib/* com.cloudera.enterprise.dbutil.DbCommandExecutor /etc/cloudera-scm-server/db.properties com.cloudera.cmf.db.
[                          main] DbCommandExecutor              INFO  Successfully connected to database.
All done, your SCM database is configured correctly!
```

