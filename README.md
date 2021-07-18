# mysqldump
mysqldump

C1
```
mysqldump --user='myusername' --password='mypassword' -h MyUrlOrIPAddress databasename > myfile.sql
```

C2
```
mysqldump -u root -p databasename > myfile.sql
```


Import
```
mysql --user='username' --password='pass' --host="ip_host" db < db.sql
```
