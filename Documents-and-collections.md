## Create a document
```js
show dbs;
use cooker;
show collections;
doc = { "title":"Tacos", "desc"  : "Yummie Tacos", "cook_time" : "20"}
db.tacos.insertOne(doc);
db.tacos.find();
db.tacos.find().pretty();
```

## Using .find() to query documents

```js

```
