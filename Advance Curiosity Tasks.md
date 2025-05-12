# Advanced Curiosity Tasks (Style: "How Do Big Systems...")
## Task 1: "How Do Big Systems Store Data?" 
**Do apps like Instagram, Uber, or Amazon use SQL databases or something else?!**
Large-scale applications like Instagram, Uber, and Amazon manage big amounts of data and require databases that offer scalability, reliability, and performance. 
Here's an overview of the database structures these companies use and the rationale behind their choices:
### Instagram
Database Choice: Instagram utilizes a combination of PostgreSQL (a relational SQL database) and Cassandra (a NoSQL database).

Rationale:

PostgreSQL: Handles structured data such as user profiles, relationships, and metadata, benefiting from ACID compliance and complex querying capabilities.

Cassandra: Manages large-scale, unstructured data like user feeds and messages, offering high availability and horizontal scalability.

### Uber
Database Choice: Uber primarily relies on MySQL for its core transactional data. 
Docical

Rationale:

MySQL: Provides strong data consistency and integrity, essential for managing ride requests, driver details, and payment transactions.

Supplementary Systems: Uber complements MySQL with other technologies like Redis for caching and Apache Kafka for real-time data streaming, ensuring efficient data processing and scalability.

### Amazon
Database Choice: Amazon employs a diverse set of databases, including Amazon DynamoDB (a NoSQL database) and Amazon RDS (which supports SQL databases like MySQL and PostgreSQL).

Rationale:

DynamoDB: Designed for high-throughput applications, it handles key-value and document data structures, making it suitable for services requiring rapid scalability and low-latency access.

Amazon RDS: Facilitates traditional relational database functionalities, supporting applications that require complex queries and transactions.
Wikipedia

**Summarize the kind of database structure big companies use and why.**
### Summary of Database Structures Used by Big Companies
1. **Relational Databases (SQL)**:
   - **Examples**: PostgreSQL, MySQL
   - **Use Cases**: Structured data, complex queries, and transactions.
   - **Rationale**: ACID compliance ensures data integrity and consistency.
2. **NoSQL Databases**:
   - **Examples**: Cassandra, DynamoDB
   - **Use Cases**: Unstructured data, high scalability, and low-latency access.
   - **Rationale**: Designed for distributed systems, offering flexibility and horizontal scaling.
3. **Hybrid Approaches**:
   - **Examples**: Combination of SQL and NoSQL databases.
   - **Use Cases**: Applications with diverse data requirements.
   - **Rationale**: Leverage the strengths of both database types to meet specific needs.
4. **Caching Systems**:
   - **Examples**: Redis
   - **Use Cases**: Fast data retrieval and reduced load on primary databases.
   - **Rationale**: Improves performance by storing frequently accessed data in memory.
5. **Real-time Data Processing**:
   - **Examples**: Apache Kafka
   - **Use Cases**: Streaming data and real-time analytics.
   - **Rationale**: Enables efficient handling of large volumes of data in real-time.
	
**Try to find one that uses SQL Server specifically.**



