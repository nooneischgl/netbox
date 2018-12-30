# Local Dev Notes

 - Starting PostgresSQL
For PostgresSQL starting 
To have launchd start postgresql now and restart at login:
  brew services start postgresql
Or, if you don't want/need a background service you can just run:
  pg_ctl -D /usr/local/var/postgres start
  
 - Logging onto postgres
 psql -d postgres


- DB Creation 
```
CREATE DATABASE netbox;
CREATE USER netbox WITH PASSWORD 'Jity9sD2F0';
GRANT ALL PRIVILEGES ON DATABASE netbox TO netbox;
\q
```

```
DROP DATABASE netbox;
DROP USER netbox;
```

```
postgres=# CREATE DATABASE netbox;
CREATE DATABASE
postgres=# CREATE USER netbox WITH PASSWORD 'J5brHrAXFLQSif0K';
CREATE ROLE
postgres=# GRANT ALL PRIVILEGES ON DATABASE netbox TO netbox;
GRANT
postgres=# \q
```
