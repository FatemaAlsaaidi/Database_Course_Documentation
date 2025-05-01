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
