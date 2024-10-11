# MongoDb-Basic-Commands-And-CRUD-Operation

## This repository is about the basic commands and CRUD operation using MongoDb . It is one of the popular No-SQL type database.

### 1) `use`

#### It is used to create and switch to a database. For example:-

```
use mydb
```

### 2) `db.createCollection("<collectionName>")`

#### It is used to create a collection. For example:-

```
db.createCollection("mycollection")
```

### 3) `db`

#### It is used to show current db. For example:-

```
db
```

### 4) `show dbs or databases`

#### It is used to show all available dbs. For example:-

```
show dbs;
show databases;
```

### 5) `show collections`

#### It is used to show all available collections in a database. For example:-

```
show collections
```

### 6) `drop()`

#### It is used to drop collection in a database. For example:-

```
db.mycollection.drop()
```

### 7) `dropDatabase()`

#### It is used to drop database. For example:-

```
db.dropDatabase()
```

## `CRUD Operation:-`

### 8) `.insertOne()`

#### It is used to create or add only one document in a collection. For example:-

```
db.mydb.mycollection.insertOne({"name":"Farooq"})
```

### 9) `.insertMany()`

#### It is used to create or add multiple documents in a collection. For example:-

```
db.mydb.mycollection.insertMany([{"name":"Farooq"},{"name":"Asad"}, {"name":"Faizan"}])
```

### 10) `.find()`

#### It is used to find many documents in a collection. For example:-

```
db.mydb.mycollection.findOne()
```

### 11) `.findOne()`

#### It is used to find only one document in a collection. For example:-

```
db.mydb.mycollection.findOne({"name":"Farooq"})
```

### 12) `.updateOne()`

#### It is used to update only one document in a collection. For example:-

```
db.mydb.mycollection.updateOne({"name":"Farooq"})
```

### 13) `.updateMany()`

#### It is used to update many documents in a collection. For example:-

```
db.mydb.mycollection.updateMany({"name":"Farooq"})
```

### 14) `.updateOne()`

#### Add a field with $set operator using updateOne(). For example:-

```
db.mydb.mycollection.updateMany({"name":"Farooq"}, {$set:{"section":""}})
```

### 15) `.updateOne()`

#### Remove a field with $unset operator using updateOne(). For example:-

```
db.mydb.mycollection.updateMany({"name":"Farooq"},{$unset:{"section":1}})
```

### 15) `.deleteOne()`

#### It is used to delete only one document in a collection. For example:-

```
db.mydb.mycollection.deleteOne({"name":"Farooq"})
```

### 16) `.deleteMany()`

#### It is used to delete many documents in a collection. For example:-

```
db.mydb.mycollection.deleteOne({"name":"Farooq"})
```
