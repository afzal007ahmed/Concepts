# NOSQL DATABASES AND THEIR TYPES

## What is NoSQL ?

* NoSQL is a term used to describe a category of database management systems that are designed to handle a wide variety of data models and are optimized for performance and scalability. 
  Unlike traditional relational databases (SQL databases), which use structured query language and predefined schemas, NoSQL databases offer more flexibility in how data is stored and retrieved.

## Types of NoSQL Databases 

### 1. Document-oriented databases

* A document-oriented database stores data in documents similar to JSON (JavaScript Object Notation) objects. Each document contains pairs of fields and values.
  The values can typically be a variety of types, including things like strings, numbers, booleans, arrays, or even other objects. A document database offers a flexible data model, much suited for semi-structured and typically unstructured data sets.
  They also support nested structures, making it easy to represent complex relationships or hierarchical data.

#### Example 

{
  "_id": "12345",
  "name": "foo bar",
  "email": "foo@bar.com",
  "address": {
    "street": "123 foo street",
    "city": "some city",
    "state": "some state",
    "zip": "123456"
  },
  "hobbies": ["music", "guitar", "reading"]
}

#### Use Cases

* **Content Management Systems** : Flexible schema for diverse content types,fast retrieval.
* **E-commerce**: Scalable for large catalogs,supports real-time analytics.
* **Real-time Analytics** : Handles high data volume efficiently,quick read/write operations.
* **Mobile Apps** : Adapts to changing user data,enhances responsiveness.
* **IoT** : Manages large data influx from devices,efficient ingestion.

### 2. Key-value databases

* A key-value store is a simpler type of database where each item contains keys and values. Each key is unique and associated with a single value. They are used for caching and session management and provide high performance
  in reads and writes because they tend to store things in memory.


#### Example

Key: user:12345
Value: {"name": "foo bar", "email": "foo@bar.com", "designation": "software developer"}

#### Use Cases

* **Session Management** : Fast user session access,scales for many users.
* **Caching** : Quick data retrieval,handles high traffic.
* **Real-time Analytics** : Rapid metric processing,supports large data volumes.
* **Shopping Carts** : Fast updates,manages traffic spikes.
* **User Profiles** : Quick data retrieval,adapts to user growth.
* **IoT Data** : Efficient device data storage,scales for vast data.

### 3. Wide-column stores

* Wide column stores are a type of NoSQL database designed to handle large volumes of data across many rows and columns. Unlike traditional relational databases, wide column stores allow for a flexible schema where each row can have a different number of columns.

#### Example

![Screenshot 2024-11-02 at 15-40-18 What Is NoSQL NoSQL Databases Explained MongoDB](https://github.com/user-attachments/assets/e0c2c19d-8430-47a5-a2db-378909bd6e1a)

#### Use Cases

* **Data Warehousing**: Fast analytics,handles large datasets.
* **Real-time Analytics** : Immediate processing,manages high data volume.
* **IoT Data** : Efficient storage,scales for massive data.
* **Content Management** : Quick retrieval,adapts to growth.
* **Social Networks**: Complex queries,supports user growth.


### 4. Graph Databases

* A graph database stores data in the form of nodes and edges. Nodes typically store information about people, places, and things (like nouns), while edges store information about the relationships between the nodes. They work well for highly connected data, where the relationships or patterns may not be very obvious initially. Examples of graph databases are Neo4J and Amazon Neptune. MongoDB also provides graph traversal capabilities using the $graphLookup stage of the aggregation pipeline.


 #### Example

 ![Screenshot 2024-11-02 at 15-48-05 What Is NoSQL NoSQL Databases Explained MongoDB](https://github.com/user-attachments/assets/ab8920d1-165f-458d-b926-8faf9734edc4)


#### Use Cases

* **Data Warehousing** : Fast analytics,large datasets.
* **Real-time Analytics** : Immediate insights,high data volume.
* **IoT Storage** : Manages massive time-series data.
* **Content Management** : Quick retrieval,scales with growth.
* **Social Networks** : Handles complex queries,rapid user growth

### 5. Multi-model databases

* A type of database that supports multiple data models (such as document, key-value, graph, and column-family) within a single integrated system, allowing users to store, retrieve, and manage diverse types of data efficiently without the need for separate databases. This flexibility enhances data management and scalability while accommodating various application requirements.

#### Example

![image](https://github.com/user-attachments/assets/95192754-9b97-4b19-b682-d5ee83777e4b)

#### Use Cases

* **E-Commerce** : Manages product catalogs and user sessions,fast searches and retrieval.
* **Social Networking** : Handles user profiles and relationships,efficient complex queries.
* **Content Management** : Stores diverse content types,quick access to various formats.
* **IoT Applications** : Collects time-series and device data,real-time processing.
* **Data Analytics** : Combines structured and unstructured data,fast aggregation and querying.



### REFERENCES

* https://chatgpt.com/
* https://www.mongodb.com/resources/basics/databases/nosql-explained
* https://aws.amazon.com/nosql/
