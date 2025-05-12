# Normalization
## What is normalization in DBMS?
In DBMS, normalization is the process of organizing data in a database to reduce redundancy and eliminating anomalies such as update, insertion, and deletion issues which guide us to improve data integrity.
It involves dividing a database into two or more tables and defining relationships between them. The main goals of normalization are to eliminate duplicate data, ensure data dependencies are logical, and simplify the structure of the database.
Normalization continues until the database follows the Single Responsibility Principle (SRP), ensuring that each table has a specific role for better efficiency and consistency.

### What is the Single Responsibility Principle (SRP) in this context?
In software engineering, the Single Responsibility Principle (SRP) means that each component (like a class or function) should have only one reason to change, meaning it handles one specific task.
When applied to databases:

Each table should serve one clear purpose or store one type of information.

For example:

A Students table stores only student information.

A Courses table stores only course details.

A Enrollments table links students to the courses they take.

### Why does Normalization continue until SRP is satisfied?
The idea is:

You keep breaking down tables and removing repeating groups or unrelated data until each table is focused on a single topic or role.

This helps in:

Avoiding update anomalies (e.g., needing to update the same data in multiple places).

Making the data more consistent and easier to maintain.

### Simple Example:
Imagine you have this table:

StudentID	StudentName	CourseName	InstructorName
1	Alice	Math	Dr. Smith
2	Bob	Math	Dr. Smith
3	Alice	History	Dr. Jones

This table mixes data about students, courses, and instructors — not following SRP.

Through normalization, you would split it into:

Students(StudentID, StudentName)

Courses(CourseID, CourseName, InstructorID)

Instructors(InstructorID, InstructorName)

Enrollments(StudentID, CourseID)

Now, each table has one responsibility, which aligns with SRP.

Normalization typically involves applying a series of rules or normal forms, which are guidelines for structuring data. 
## Different normal forms
!['Different normal forms'](images/normalizationType.PNG)

1. **First Normal Form (1NF)**: 
In 1NF, every database cell or relation contains an single value that can’t be further divided, for example the table shouldn’t have **multivalued attributes**.
Example:
The following table contains two phone number values for a single attribute.

| Emp_ID | Student Name | Phone Number |
|----|-----|------|
|1| Fatema | 12345678 |
|2| Noor | 12345678, 87654321 |

After applying normalization

|Emp_ID| Student Name |
|----|---|
|1| Fatema|
|2| Noor|

|Emp_ID| Phone Number |
|---|----|
|1| 12345678|
|2| 12345678|
|2| 87654321|



