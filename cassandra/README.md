# IMPORT 

Import schema (.cql file)

```bash
cqlsh -e "SOURCE '/path/to/schema.cql'"
```

OR

```bash
cqlsh

use keyspacename; 

source 'table_schema_file.cql';
```

## DOCKER 

```bash

```

# EXPORT

Export keyspace schema

```bash
cqlsh -e "DESC KEYSPACE user" > user_schema.cql
```

Export entire database schema

```bash
cqlsh -e "DESC SCHEMA" > db_schema.cql
```

## DOCKER

```bash
```

# Seeding cassandra for developer with default record

## DOCKER

Docker compose files with volume of db scripts mounted to docker-entrypoint-initdb.d

```bash
version: '2'
services:
    cassandra:
        image: cassandra:3.9
        restart: unless-stopped
        volumes:
            - /var/db/cassandra:/var/lib/cassandra
            - ./db-schema:/docker-entrypoint-initdb.d/
        ports:
            - 7000:7000
            - 7001:7001
            - 7199:7199
            - 9042:9042
            - 9160:9160
```

