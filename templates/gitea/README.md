# Gitea

Git Server with Web GUI

## Configuration


Now the database is up and running, we need to configure it. Make sure you remember the password for when Gitea starts.

$ docker exec -it gitea-db psql -U postgres
psql (9.6.1)
Type "help" for help.

postgres=# CREATE USER gitea WITH PASSWORD '<PASSWORD>';
CREATE ROLE
postgres=# CREATE DATABASE gitea OWNER gitea;
CREATE DATABASE
postgres=# \q
$
