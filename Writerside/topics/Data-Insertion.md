# Data Insertion

1. On the Mongo client, run the command below to insert data into the catalog collection. Each data point is referred to as a **document** in MongoDB.
```MongoDB
db.catalog.insert({
  "_id":"clog1",
  "name":"product catalog"
})
```
The above command inserts the JSON document **{ "_id":"clog1", "name":"product catalog" }** into the collection.

2. Now, create the Category collection by running the following command on the MongoClient.
```MongoDB
db.createCollection("category")
```

3. On the Mongo client, run the following command, to insert a document inside the catalog collection.
```MongoDB
db.category.insert({
  "category_name":"Smart Phone",
  "child_categories":[],
  "parent_categories":[],
})
```

4. To insert multiple documents, you can enclose them in square brackets. On the Mongo client, run the command below to insert two documents at a time.
```MongoDB
db.category.insert([
{
  "category_name":"Apple Products",
  "child_categories":[],
  "parent_categories":[],
},
{
  "category_name":"Apple Phones",
  "child_categories":[],
  "parent_categories":["ct001","ct002"],
}])
```

5. On the Mongo client, run the command below to count the number of documents.

```MongoDB
db.category.countDocuments()
```
This command gives you the number of documents in the collection. You inserted one document first and then two document as an array. The output should reflect 3 documents.

6. On the Mongo client, run the command below to list all documents in the category collection.

```MongoDB
db.category.find()
```
This command lists all the documents in the collection **category**.

Notice that MongoDB automatically adds an **_id** field to every document in order to uniquely identify the document.

7. To find a particular document, you can specify the search criteria in the **find** command.

```MongoDB
db.category.find({category_name:"Apple Products"})
```

This command lists all the documents in the collection **category** which match the condition.

