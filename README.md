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


## mysqldump only table
```
mysqldump -u root -p databasename tableName  > myfile.sql
```

replace all table name in vim
```
:%s/foo/bar/g
:%s/`CustomersBackup2017`/`tableName`/g
```

## mysql import table from backup file
```
CREATE TABLE tableName LIKE original_table;
mysql -u root -p databasename < myfile.sql
```

##
normal way to clone table
```
CREATE TABLE CustomersBackup2017 LIKE original_table;
INSERT INTO CustomersBackup2017  SELECT * FROM original_table;
```
