# HTB: Sequel

┌──(xnc㉿xnc-v8tpure)-[~]
└─$ mysql -h 10.129.116.50 -u root

-h : Connect to host.
-u : User for log-in if not current user.

```
SHOW databases; : Prints out the databases we can access.
USE {database_name}; : Set to use the database named {database_name}.
SHOW tables; : Prints out the available tables inside the current
database.
SELECT * FROM {table_name}; : Prints out all the data from the table {table_name}.
```

Note that it is essential to end each command with the ; symbol, as it declares the end of the command

flag: 7b4bec00d1a39e3dd4e021ec3d915da8
