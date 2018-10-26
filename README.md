# import-export-db

This project contains scripts to Import/Export Database schemas


|Suported Databases|
|---|
|Cassandra|
|Couchbase|
|MariaDB|
|MongoDB|
|MSSQL|
|MySQL|
|PostgreSQL|

___

## Links to README

* [Cassandra](cassandra/README.md)
* [Couchbase](couchbase/README.md)
* [MariaDB](mariadb/README.md)
* [MongoDB](mongo/README.md)
* [MSSQL](mssql/README.md)
* [MySQL](mysql/README.md)
* [PostgreSQL](postgreSQL/README.md)

___

## Project Structure

```bash
├── README.md
├── cassandra
│   ├── README.md
│   ├── docker-entrypoint-initdb.d
│   │   └── init.cql
│   └── docker-entrypoint.sh
├── couchbase
│   └── README.md
├── docker-compose.yml
├── mariadb
│   └── README.md
├── mongo
│   └── README.md
├── mssql
│   └── README.md
├── mysql
│   ├── README.md
│   ├── conf
│   │   ├── docker-entrypoint-initdb.d
│   │   │   └── database.sql
│   │   └── my.cnf
│   ├── mysql-init.yml
│   └── mysql.yml
└── postgreSQL
    ├── README.md
    ├── postgres-initdb.sh
    ├── postgresql-init-db.yml
    ├── postgresql-volume.yml
    └── postgresql.yml
```


## Meet The Team

* **jbalu** - Project Owner - [JinnaBalu](https://github.com/JinnaBalu)
* **Tom Konidas** - Contributor - [tomkonidas](https://github.com/tomkonidas)
