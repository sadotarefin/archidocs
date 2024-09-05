| DB name       | #Type    | #Comment    |
| :-----------: | :---:    | :---: |
| Cassandra     | Key/Value      | N/A   |
| HBase     | Key/Value      | N/A   |
| CouchDB     | Document      | N/A   |
| MongoDB     | Document      | N/A   |
| Neo4j     | Graph      | N/A   |

NoSQL databases are ideal in the following scenarios:

**Super-Low Latency Requirements:**
If your application requires super-fast response times, NoSQL databases like Redis are ideal. Redis is an in-memory key-value store known for sub-millisecond latency, making it perfect for caching, real-time analytics, leaderboards, and session management.

**Unstructured Data:**
When you need to store unstructured or semi-structured data that doesn't fit a relational model, use a NoSQL database like MongoDB. MongoDB is a document-oriented database that stores data in JSON-like documents, allowing for flexibility when dealing with evolving data types or variable schema (e.g., storing user profiles, product catalogs, or logs).

**Serialization/Deserialization:**
If your application primarily works with serialized data formats like JSON, XML, or YAML, a NoSQL database like Couchbase works well. Couchbase is optimized for storing and retrieving JSON documents, making it easy to serialize/deserialize data, particularly in applications that use APIs to exchange data (e.g., mobile apps or web services).

**Massive Data Storage:**
For applications that need to store and process a massive amount of data, particularly in a distributed system, Cassandra is a great choice. Cassandra is designed for horizontal scaling and handles large amounts of data efficiently across multiple servers, making it ideal for big data use cases such as IoT platforms, real-time analytics, and event logging.