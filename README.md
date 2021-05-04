# workshop

Summary

Workshop of b2b team blablabla


Setup:

> docker run -p 27018:27017 --name workshop-mongo -d mongo:4.0
> brew install mongodb-database-tools
> mongoimport --db workshop --collection people --file /data/configdb/people.json
> mongo --port 27018
> show dbs
> use workshop
> db.people.count({ "email" : {"$exists": 1} })

Comandos ++++

> docker exec -it workshop-mongo bash

> docker run -p 27019:27017 --name workshop-directoryperdb-mongo -d mongo:4.0 --directoryperdb

> docker run -p 27020:27017 --name workshop-directoryperdb-mongo -d mongo:4.0 --directoryperdb --wiredTigerDirectoryForIndexes

Baixar:

https://www.mongodb.com/products/compass
