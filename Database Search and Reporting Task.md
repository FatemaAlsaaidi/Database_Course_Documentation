# Database Search and Reporting Task
## Objective
###  *Flat File Systems vs Relational Databases*
| Storage Type             | Structure                     | Data Redundancy |  Relationships | Drawbacks |
| -------------------------| --------------------------                | ----------------          | --------------                | ----------|
| 1. Flat File Systems     | file that contains a single table of data |  High Data Redundancy     |  no relationship              | Harder to Change Data Format, Poor at Complex Queries, requiring all records to have the same fields, less data consistency,one user can access data at a time.     |          
| 2. Relational Databases  | database with one or more tables          |  Low Data Redundancy      | relationship between tables   | more complex with varying costs, huge size     |

### *DBMS Advantages Mind Map*
![DBMS Advantages Mind Map](./images/DBMSAdantages.PNG)

###  Roles in a Database System 
Explaining each of the following roles: 
• System Analyst: 
  - A system analyst is responsible for collection requirements and analyzing business needs. They work closely with stakeholders, they analysis requirements to ensure that the system aligns with organizational goals.
• Database Designer: 
  - A database designer is responsible for design the structure and organization of a database. They design the schema, define relationships between tables, and ensure data integrity and efficiency in data storage. 
• Database Developer: 
  - A database developer is responsible for codeing and optimizing SQL queries, creating stored procedures, and implementing database solutions. They work on the technical aspects of database development and ensure that the database meets performance and scalability requirements.
• DBA (Admin): 
  - A DBA (Database Administrator) is responsible for managing and maintaining the database system. They handle tasks such as installation, configuration, backup and recovery, performance tuning, and security management. DBAs ensure that the database operates smoothly and efficiently.
• Application Developer: 
  - An application developer is responsible for creating software applications that interact with the database. They design and develop user interfaces, implement business logic, and ensure that the application can effectively retrieve and manipulate data from the database.
• BI Developer: 
  - A BI (Business Intelligence) developer is responsible for designing and implementing data analysis and reporting solutions. They work with data warehousing, ETL (Extract, Transform, Load) processes, and create dashboards and reports to provide insights into business performance.

## Additional Research Topics to Include in the Report
### Types of Databases 
• Relational vs Non-Relational (e.g., MongoDB, Cassandra)
- Relational: 
  - Structuring information in tables, rows, and columns.
  - Uses SQL for querying
  - Examples: MySQL, PostgreSQL, Oracle
- Non-Relational: 
  - store data as individual, unconnected files and can be used for complex, unstructured data types, such as documents or rich media files.
  - Uses various query languages (e.g., MongoDB uses BSON)
  - Examples: MongoDB, Cassandra, Couchbase

• Centralized vs Distributed vs Cloud Databases 
- Centralized database: 
  - All data is stored in a single location, typically on a server.
  - Easier to manage and secure but can be a single point of failure.
- Distributed database: 
  - Data is distribute across multiple locations or servers.
  - Provides redundancy and improved performance but can be more complex to manage.
- Cloud database: 
  - Data is stored in the cloud and accessed over the internet.
  - Offers scalability and flexibility but may raise concerns about data security and privacy.
• Use case examples:
	-  Relational: 
		- Banking systems, e-commerce platforms, and any application requiring complex queries and transactions.
	-  Non-Relational: 
		- Social media platforms, content management systems, and applications with large volumes of unstructured data.
	-  Centralized: 
		- Small businesses with limited data needs and resources.
	- Distributed: 
		- Large organizations with multiple locations or data centers.
	-  Cloud: 
		- Startups and businesses looking for cost-effective and scalable solutions.
### Cloud Storage and Databases
**What is Cloud Storage and how does it relate to databases?**

- Cloud storage is a service that allows users to store and access data over the internet. It uses remote servers to save data, Users can access data in Cloud Storage through an internet connection and software .Thus, provides scalable and flexible storage solutions without the need for physical hardware.
- Cloud databases are databases that are hosted and managed in the cloud. They can be either relational or non-relational and provide similar benefits as cloud storage, such as scalability, flexibility, and cost-effectiveness. Cloud databases allow users to access and manage their data from anywhere with an internet connection.
- Cloud storage and databases are often used together to provide a complete data management solution. Cloud storage can be used to store large volumes of unstructured data, while cloud databases can be used to manage and query structured data. This combination allows organizations to leverage the benefits of both technologies for their data needs.

**Advantages and Disadvantages of using cloud-based databases (e.g., Azure SQL, Amazon RDS, Google 
Cloud Spanner):**

- Advantages:
	- Scalability: Cloud databases can easily scale up or down based on demand, allowing organizations to handle varying workloads without the need for physical hardware upgrades.
	- Cost-effectiveness: Cloud databases often operate on a pay-as-you-go model, reducing upfront costs and allowing organizations to only pay for the resources they use.
	- Accessibility: Cloud databases can be accessed from anywhere with an internet connection, enabling remote work and collaboration.
	- Automatic backups and updates: Many cloud database providers offer automated backup and update services, reducing the burden on IT teams and ensuring data security.
	- High Availability and Reliability: Cloud databases often come with built-in redundancy and failover mechanisms, ensuring that data is always accessible even in the event of hardware failures.
	- Flexibility and Agility: Cloud databases allow organizations to quickly adapt to changing business needs, enabling faster development and deployment of applications.
	
- Disadvantages:
	- Internet Dependency: Cloud databases require a stable internet connection for access, which can be a limitation in areas with poor connectivity.
	- Data Security: Storing sensitive data in the cloud raises concerns about data security and privacy, as organizations must trust third-party providers to protect their information.
	- Vendor Lock-in: Moving data from one cloud provider to another can be complex and costly, potentially leading to vendor lock-in.
	- Limited Control: Organizations may have limited control over the underlying infrastructure and configurations of cloud databases, which can be a concern for some businesses.
	- Performance Issues: The performance of cloud-based DBMS can be affected by factors such as network latency, bandwidth, and congestion.
	- Limited Offline Capabilities: Cloud-based DBMS require internet connectivity to access data, which can be a disadvantage in situations where connectivity is limited or unavailable. 
### **Database Engines and Languages**
**What is a Database Engine?**
A database engine, also known as a storage engine or database management system (DBMS), is a software component responsible for managing and organizing data in a database. It handles tasks such as data storage, retrieval, modification, and querying while ensuring data integrity and consistency. The database engine efficiently processes user requests, transactions, and database operations using various optimization techniques and algorithms.
**What are the different types of database engines?**
- Relational Database Engines: 
  - These engines are designed to manage structured data organized in tables with predefined relationships. They use SQL (Structured Query Language) for querying and manipulating data. Examples include MySQL, PostgreSQL, Oracle Database, and Microsoft SQL Server.
- NoSQL Database Engines: 
  - These engines are designed to handle unstructured or semi-structured data and provide flexible data models. They can be document-based, key-value stores, column-family stores, or graph databases. Examples include MongoDB, Cassandra, Couchbase, and Neo4j.
- In-Memory Database Engines: 
  - These engines store data in memory for faster access and processing. They are often used for real-time applications and analytics. Examples include Redis, Memcached, and SAP HANA.
- NewSQL Database Engines: 
  - These engines combine the scalability of NoSQL databases with the ACID (Atomicity, Consistency, Isolation, Durability) properties of traditional relational databases. They are designed for high-performance applications. Examples include Google Spanner, CockroachDB, and VoltDB.
- Object-Oriented Database Engines: 
  - These engines store data in the form of objects, similar to object-oriented programming. They are designed for applications that require complex data structures and relationships. Examples include db4o and ObjectDB.
- Time-Series Database Engines: 
  - These engines are optimized for handling time-stamped data, making them suitable for applications such as IoT, monitoring, and analytics. Examples include InfluxDB, TimescaleDB, and Prometheus.
- Graph Database Engines: 
  - These engines are designed to manage and query graph data structures, which consist of nodes and edges. They are used for applications involving complex relationships and connections. Examples include Neo4j, Amazon Neptune, and ArangoDB.
- Columnar Database Engines: 
  - These engines store data in columns rather than rows, making them suitable for analytical workloads and data warehousing. Examples include Amazon Redshift, Google BigQuery, and Apache Cassandra.
- Multi-Model Database Engines: 
  - These engines support multiple data models (e.g., relational, document, graph) within a single database system, providing flexibility for various applications. Examples include ArangoDB, OrientDB, and MarkLogic.
**What is a Database Language?**
	- A database language is a programming language or query language used to interact with and manage databases. It allows users to perform operations such as creating, reading, updating, and deleting data within a database. Database languages provide a way to communicate with the database management system (DBMS) and execute various tasks related to data manipulation and retrieval.
**Examples: SQL Server, MySQL, Oracle, PostgreSQL**
	- SQL (Structured Query Language): 
		- SQL is the most widely used database language for relational databases. It provides a standardized way to query and manipulate data using commands such as SELECT, INSERT, UPDATE, DELETE, and CREATE TABLE.
	- PL/SQL (Procedural Language/SQL): 
		- PL/SQL is an extension of SQL used in Oracle databases. It allows users to write procedural code, including loops, conditionals, and error handling, within SQL statements.
	- T-SQL (Transact-SQL): 
		- T-SQL is an extension of SQL used in Microsoft SQL Server. It includes additional features such as procedural programming constructs, error handling, and built-in functions.
	- MySQL: 
		- MySQL is an open-source relational database management system that uses SQL as its query language. It is widely used for web applications and supports various storage engines.
	- PostgreSQL: 
		- PostgreSQL is an open-source relational database management system that supports advanced features such as JSON data types, full-text search, and custom data types. It uses SQL as its primary query language.
		
**What languages do they use? (e.g., T-SQL, PL/SQL, ANSI SQL)**
	- T-SQL (Transact-SQL): 
		- T-SQL is an extension of SQL used in Microsoft SQL Server. It includes additional features such as procedural programming constructs, error handling, and built-in functions.
	- PL/SQL (Procedural Language/SQL): 
		- PL/SQL is an extension of SQL used in Oracle databases. It allows users to write procedural code, including loops, conditionals, and error handling, within SQL statements.
	- ANSI SQL: 
		- ANSI SQL (American National Standards Institute SQL) is the standard version of SQL defined by the ANSI. It provides a common syntax and set of rules for querying and manipulating data across different relational database systems.
### **Database Design and Normalization**
**What is Database Design?**
- Database design is the process of defining the structure, organization, and relationships of data within a database. It involves creating a blueprint for how data will be stored, accessed, and managed to ensure data integrity, efficiency, and scalability. The goal of database design is to create a well-structured database that meets the needs of the application and its users.
- The database design process typically includes the following steps:
	1. Requirements Analysis: 
		- Understanding the data requirements of the application and its users.
	2. Conceptual Design: 
		- Creating a high-level model of the database, including entities, attributes, and relationships.
	3. Logical Design: 
		- Translating the conceptual model into a logical schema, defining tables, columns, and data types.
	4. Physical Design: 
		- Implementing the logical schema in a specific database management system (DBMS), including indexing and storage considerations.
	5. Implementation: 
		- Creating the database and populating it with data.
**What is Normalization?**
		- Normalization is the process of organizing data in a database to minimize redundancy and improve data integrity. It involves dividing large tables into smaller, related tables and defining relationships between them. The goal of normalization is to eliminate data anomalies, such as insertion, update, and deletion anomalies, by ensuring that each piece of data is stored in only one place.

**Is there a relationship between the engine and the language?**
**A programming language** (e.g., Python, JavaScript) is a way to write code.

**An engine** (or runtime/interpreter) executes code written in that language.

Example: The V8 engine runs JavaScript in Chrome.

Example: The CPython engine runs Python.

**A database engine** is a software component that manages data storage and retrieval.

**A database language** (e.g., SQL) is a way to interact with the database engine.
Example: SQL is used to query and manipulate data in a relational database engine (e.g., MySQL, PostgreSQL).

**Can one language work across different engines?**
- Yes, many database languages, such as SQL, can work across different database engines. However, there may be variations in syntax and features between different engines. For example, while SQL is a standard language for relational databases, each database engine may have its own extensions or variations (e.g., T-SQL for SQL Server, PL/SQL for Oracle).

### **Database Security and Access Control**
**What is Database Security?**
- Database security refers to the measures and practices implemented to protect databases from unauthorized access, data breaches, and other security threats. It involves safeguarding sensitive data, ensuring data integrity, and maintaining the availability of database systems. Database security encompasses various aspects, including authentication, authorization, encryption, auditing, and backup and recovery.
- The goal of database security is to prevent unauthorized access to data, protect against data loss or corruption, and ensure compliance with regulatory requirements. Organizations implement database security measures to mitigate risks associated with data breaches, insider threats, and cyberattacks.
- Database security is essential for maintaining the confidentiality, integrity, and availability of data, which are critical components of information security.

### ** Can We Transfer a Database Between Engines?**
It is possible to transfer a database between different database engines such as from SQL Server to MySQL or Oracle to PostgreSQL, but the process is not as simple as a direct copy. 
It requires clear planning and transformation due to differences in SQL dialects, data types, features, and behavior between database systems.

**Is it possible to migrate a database from SQL Server to MySQL, or Oracle to PostgreSQL?** 
yes it is possible as we explaine in the previous paragraph.

**What are the challenges of engine-to-engine migration?**
1. Data Type Incompatibilities
- Each engine has its own type system. For example:

- DATETIME in SQL Server ≠ TIMESTAMP in PostgreSQL

- NUMBER in Oracle may not exactly match DECIMAL in MySQL

2. Stored Procedures, Triggers & Functions

- Written in different languages (T-SQL, PL/pgSQL, PL/SQL).

- Must be rewritten manually in the new engine's procedural language.

3. Constraints and Indexing

- Naming conventions and supported constraint types may differ.

- Index strategies can be different in behavior and performance.

5. Character Sets & Collation

- Unicode vs non-Unicode, collation orders may lead to issues with sorting/filtering.

5. Performance Optimization Differences

- Execution plans, query optimizers, and indexing behavior vary.

6. Application Compatibility

- Application logic depending on specific SQL dialects will likely need updating.

**What should we consider before transferring (data types, triggers, stored procedures, etc.)?**
|Area|	What to Do|
|Schema|	Map equivalent data types, table structures, and normalize where needed.|
|Stored Procedures|	Recode in the new DB's language.|
|Triggers & Views|	Review and rewrite to fit the new engine.|
|Data Volume|	Plan for large data migration (batching, compression, etc.).|
|Dependencies|	Check all application layers that interact with the database.|
|Security|	Recreate user roles, permissions, and access policies.|
|Testing|	Perform data validation, integrity checks, and performance tests post-migration.|
|Backup	|Always back up before attempting migration.|

**When Do We Need to Transfer a Database Between Engines?**
We might need to migrate a database from one engine to another in several common scenarios, including:
1. Cost Reduction
Moving from a commercial engine (like Oracle or SQL Server) to a free/open-source one (like PostgreSQL or MySQL) can significantly reduce licensing and maintenance costs.

2. Cloud Adoption or Vendor Change
Migrating from an on-premise engine to a cloud-based engine (e.g., SQL Server → Amazon Aurora).

Moving between cloud providers (e.g., Azure SQL → Google Cloud SQL).

3. Standardization
Unifying systems across departments to a single database platform (e.g., consolidating multiple systems into PostgreSQL).

4. Feature Requirements
Switching engines to gain access to features not available in the current system (e.g., better JSON handling in PostgreSQL compared to MySQL).

5. Performance Improvements
When the current engine doesn’t scale well for the workload, a different engine may offer better performance or tuning capabilities.

6. End of Support or Compatibility Issues
The current database version may no longer be supported, or it may not be compatible with newer applications or operating systems.

7. Integration with New Technologies
New tools or platforms (data lakes, machine learning, analytics tools) might integrate better with specific database engines.

