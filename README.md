## Working with MongoDB

MongoDB is a source-available cross-platform document-oriented database program. Classified as a NoSQL database program, MongoDB uses JSON-like documents with optional schemas. 
### Features of MongoDB

**i. Rich JSON Documents-**

* The most natural and productive way to work with data.
* Supports arrays and nested objects as values.
* Allows for flexible and dynamic schemas.
* The document model maps to the objects in your application code, making data easy to work with.

```JSON
{
 "name": "notebook",
 "qty": 50,
 "rating": [ { "score": 8 }, { "score": 9 } ],
 "size": { "height": 11, "width": 8.5, "unit": "in" },
 "status": "A",
 "tags": [ "college-ruled", "perforated"]
}
```

**ii. Powerful query language-**
* Rich and expressive query language that allows you to filter and sort by any field, no matter how nested it may be within a document.
* Support for aggregations and other modern use-cases such as geo-based search,  graph search, and text search.
* Queries are themselves JSON, and thus easily composable. No more concatenating strings to dynamically generate SQL queries.
```
> db.collection.find( { qty: { $gt: 4 } } )
```
OUTPUT:
```JSON
{ "_id": "apples", "qty": 5 }
{ "_id": "bananas", "qty": 7 }
```
**iii. power of a relational database, and more...**

* Full ACID(Atomicity, Consistency, Isolation, Durability) transactions.
* Support for joins in queries.
* Two types of relationships instead of one: reference and embedded.
**v. BI Connector**
* Allow any BI tool that can speak the MySQL protocol to work with your MongoDB data.
* Leverage the BI tools your organization already uses.
* Perform federated analytics, combining data from MongoDB and other databases.

### MongoDBAtlas(Online, Cloud) vs MongoDB Compass(Offline)

 - MongoDB Atlas belongs to "MongoDB Hosting" category of the tech stack, while MongoDB Compass can be primarily classified under "Database Tools".
 - MongoDB Atlas is a global cloud database service built and run by the team behind MongoDB. Enjoy the flexibility and scalability of a document database, with the ease and automation of a fully managed service on your preferred cloud.
* Atlas is a mongoDB service on cloud. It uses AWS, Azure and GCP cloud services to cater developers all around the globe for managing mongoDB databases.
* Its a globally available cloud database service for all kinds of modern applications.
* Visit [ATLAS HOMEPAGE](https://www.mongodb.com/cloud/atlas) for more details.

### Installing MongoDB (Community Edition)

  * Link to Download MongoDB - [Download Link](https://www.mongodb.com/try/download/community2)
  * Offical Documentation to Install - [Official Documents](https://docs.mongodb.com/manual/administration/install-community/)

### Installing MongoDB Python package

```
    !python -m pip install pymongo
```
