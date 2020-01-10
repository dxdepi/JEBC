Cloud Provider : AWS

## Instance List
|Instance Name | DNS | IP| OS |
|------|----|----|---|
|i-0402ee44da936525a|ec2-18-139-138-68.ap-southeast-1.compute.amazonaws.com|18.139.138.68| CentOS Linux 7|
|i-0402ee44da936525a|ec2-52-74-144-71.ap-southeast-1.compute.amazonaws.com|52.74.144.71| CentOS Linux 7|
|i-0f3d8f4a53031aa57|ec2-3-1-148-128.ap-southeast-1.compute.amazonaws.com|3.1.148.128| CentOS Linux 7|

## File System Capacity
```
[centos@ip-172-31-25-172 ~]$ for node in `cat serverlist`;   do     echo ------------- $node:;         ssh -i depipem.pem centos@$node df -h; done;
------------- 172.31.25.172:
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda1       30G  970M   30G   4% /
devtmpfs        7.8G     0  7.8G   0% /dev
tmpfs           7.8G     0  7.8G   0% /dev/shm
tmpfs           7.8G   17M  7.8G   1% /run
tmpfs           7.8G     0  7.8G   0% /sys/fs/cgroup
tmpfs           1.6G     0  1.6G   0% /run/user/1000
------------- 172.31.16.171:
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda1       30G  897M   30G   3% /
devtmpfs        7.8G     0  7.8G   0% /dev
tmpfs           7.8G     0  7.8G   0% /dev/shm
tmpfs           7.8G   17M  7.8G   1% /run
tmpfs           7.8G     0  7.8G   0% /sys/fs/cgroup
tmpfs           1.6G     0  1.6G   0% /run/user/1000
------------- 172.31.30.88:
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda1       30G  897M   30G   3% /
devtmpfs        7.8G     0  7.8G   0% /dev
tmpfs           7.8G     0  7.8G   0% /dev/shm
tmpfs           7.8G   17M  7.8G   1% /run
tmpfs           7.8G     0  7.8G   0% /sys/fs/cgroup
tmpfs           1.6G     0  1.6G   0% /run/user/1000

```
## Yum Repository

```
[centos@ip-172-31-25-172 ~]$ sudo yum repolist enabled
Loaded plugins: fastestmirror
Loading mirror speeds from cached hostfile
 * base: mirror.newmediaexpress.com
 * extras: mirror.newmediaexpress.com
 * updates: mirror.newmediaexpress.com
cloudera-manager                                                                                                                                                           |  951 B  00:00:00     
cloudera-manager/primary                                                                                                                                                   | 4.4 kB  00:00:00     
cloudera-manager                                                                                                                                                                              7/7
repo id                                                                                      repo name                                                                                      status
base/7/x86_64                                                                                CentOS-7 - Base                                                                                10,097
cloudera-manager                                                                             Cloudera Manager                                                                                    7
extras/7/x86_64                                                                              CentOS-7 - Extras                                                                                 307
updates/7/x86_64                                                                             CentOS-7 - Updates                                                                              1,010
repolist: 11,421

```
## /etc/passwd

```
centos:x:1000:1000:Cloud User:/home/centos:/bin/bash
purnama:x:2700:1002::/home/purnama:/bin/bash
basuki:x:2800:1001::/home/basuki:/bin/bash

```

## /etc/group

```
centos:x:1000:
hackers:x:1001:
crackers:x:1002:
```
