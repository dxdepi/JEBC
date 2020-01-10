## Output hdfs dfs -ls /user
```
[centos@ip-172-31-25-172 ~]$ hdfs dfs -ls /user
Found 6 items
drwxr-xr-x   - basuki   basuki            0 2020-01-10 13:36 /user/basuki
drwxrwxrwx   - mapred   hadoop            0 2020-01-10 12:55 /user/history
drwxrwxr-t   - hive     hive              0 2020-01-10 12:56 /user/hive
drwxrwxr-x   - hue      hue               0 2020-01-10 13:14 /user/hue
drwxr-xr-x   - hueadmin hueadmin          0 2020-01-10 13:35 /user/hueadmin
drwxr-xr-x   - purnama  purnama           0 2020-01-10 13:36 /user/purnama
```
## Output CM API call
```
{
  "items" : [ {
    "hostId" : "7a5a10b8-3941-49d9-995b-c6d8bf18304a",
    "ipAddress" : "172.31.16.171",
    "hostname" : "ip-172-31-16-171.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-16-171.ap-southeast-1.compute.internal:7180/cmf/hostRedirect/7a5a10b8-3941-49d9-995b-c6d8bf18304a",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 16655380480
  }, {
    "hostId" : "07fa7607-dd3d-4deb-a9cf-1abf99f3a0da",
    "ipAddress" : "172.31.25.172",
    "hostname" : "ip-172-31-25-172.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-16-171.ap-southeast-1.compute.internal:7180/cmf/hostRedirect/07fa7607-dd3d-4deb-a9cf-1abf99f3a0da",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 16655380480
  }, {
    "hostId" : "01236565-e77b-47f3-98fc-3e2af4b0a81f",
    "ipAddress" : "172.31.30.88",
    "hostname" : "ip-172-31-30-88.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-16-171.ap-southeast-1.compute.internal:7180/cmf/hostRedirect/01236565-e77b-47f3-98fc-3e2af4b0a81f",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 16655384576
  } ]
}
```
