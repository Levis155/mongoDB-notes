# Working with Mongo CLI

1. On the Mongo client run the below command to check the version of the MongoDB Server.

```mongodb
db.version()
```

This will show the version of the mongodb server.

2. On the Mongo client, run the command below to get the list of databases on the server.

```mongodb
show dbs
```

This will print a list of the databases present on the server, including default and user-defined.

3. On the Mongo client run the command below to create a database.

```mongodb
use productCatalogDB
```
This will switch the context to the database named productCatalogDB. If the database productCatalogDB doesn't exist, MongoDB will create it for you. But that happens only when you create a collection inside the database. MongoDB creates databases and collections lazily i.e., it is created only when necessary.

4. On the Mongo client run the command below to create a collection named catalog inside the productCatalogDB.

```mongodb
db.createCollection("catalog")
```
This will create a collection name catalog inside the productCatalogDB database.

5. On the Mongo client run the command below to list the collections.

```mongodb
show collections
```
This will print the list of collections in your current database