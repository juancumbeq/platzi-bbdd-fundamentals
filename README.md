# BBDD with SQL

<p align="center">
  <img src="https://img.shields.io/badge/Curso%20-Finalizado-brightgreen"/>
</p>

<br>

# INDEX

<br>
<br>
<br>

# INTRODUCCTION TO RELATIONALS BBDD
  ## [BBDD GOOD PRACTICES WITH SQL]()
Database normalization is essential to ensure data integrity, organize data properly, and manage relationships between tables.

  ### What is the First Normal Form (1NF)?
The first normal form (**1NF**) is based on three fundamental steps:

  - **Atomic data**: Information must be indivisible.
  - **Primary key**: A unique identifier for each record.
  - **Centralization of data by column**: Do not separate information by commas, except for descriptions.

A bad example would be having a student, Marco, with courses listed in a single column. The correct solution is to create an individual record for each course and student, ensuring that each course is properly referenced.

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-bbdd-with-sql/blob/main/readme_images/raw.png?raw=true" width= "75%" alt="raw">
</p>

  ### How is the Second Normal Form (2NF) applied?
The second normal form (**2NF**) requires that all non-key attributes depend on the primary key. To comply with 2NF, you must first satisfy the requirements of 1NF. This involves separating information into additional tables and using foreign keys to establish relationships. For example, creating a separate table for courses and referencing it from the student table using a foreign key.

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-bbdd-with-sql/blob/main/readme_images/course-table.png?raw=true" width= "65%" alt="course-table">
</p>

  ### What does the Third Normal Form (3NF) entail?
The third normal form (3NF) adds that all non-key attributes must be independent of each other and comply with the previous two forms. Any redundancy and unnecessary dependency should be eliminated. In this case, an intermediate table between students and courses can help maintain the independence of attributes, relating students and courses through unique identifiers.

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-bbdd-with-sql/blob/main/readme_images/3fn.png?raw=true" width= "65%" alt="3fn">
</p>

  ### What are other examples of normalization?
A common example is addresses. An address record can be more atomic if it is divided into separate tables for countries, cities, and departments. Although some companies prefer a single address table, the normalization process always seeks the most efficient and organized structure.

Understanding these forms of normalization and applying them correctly improves the quality and management of data in any database.

<br>
<br>

  ##  [DATATYPES IN SQL]()
Optimizing data processes and improving their quality is possible thanks to the correct definition of data types. These are crucial for specifying the kind of information to be inserted into columns, variables, and parameters.

  ### What are data types?
Data types are used in columns, variables, and parameters to define the kind of information that will be inserted into an object. This helps to identify the type of content in a column in a table, a parameter in a stored procedure, or a variable.

  ### What are the categories of data types?
Data types are grouped into three main categories: numeric, text, and date types.

  ### What numeric data types exist?
  - **Integer**: Classified into three types:
    - **Int**: 4 bytes of capacity.
    - **Smallint**: 2 bytes of capacity.
    - **Bigint**: 8 bytes of capacity.
    -  Used in primary keys and quantities.
  
  - **Decimal**: Specified with "decimal" and two values in parentheses.
    - Example: decimal(10, 2) for 10 digits with 2 decimal places.
  - **Float**: Similar to decimal but with unlimited precision.

  ### What text data types are most commonly used?
  - **Char**: Specified with fixed length.
    - Example: char(10).
    - Occupies the full length regardless of the stored text.
  - **Varchar**: Variable length.
    - Example: varchar(10).
    - Occupies only the space of the stored text.
  - **Text**: No length limitation.
    - Ideal for long descriptions.

  ### What are the date data types?
  - **Time**: Specifies the time.
  - **Date**: Specifies the date.
  - **Datetime**: Combines date and time.

  ### Other data types
  - Boolean data types:
    - **BOOLEAN**: Almacena valores TRUE o FALSE.
      - Tamaño: 1 byte (aunque esto puede variar según el sistema de bases de datos).

  - Spatial Data Types
    - **GEOMETRY**: Stores geometric data.
      - Size: Variable, depends on the content.
    - **POINT**: Stores a point in geometric space.
      - Size: Variable, depends on the content.
    - **LINESTRING**: Stores a line in geometric space.
      - Size: Variable, depends on the content.
    - **POLYGON**: Stores a polygon in geometric space.
      - Size: Variable, depends on the content.

  - JSON and XML Data Types
    - **JSON**: Stores data in JSON format.
      - Size: Variable, depends on the content.
    - **XML**: Stores data in XML format.
      - Size: Variable, depends on the content.
  - UUID Data Types
    - **UUID**: Stores universally unique identifiers.
      - Size: 16 bytes.

Analyzing and choosing the correct data type is vital to avoid extensive data cleaning and transformation processes. Share your knowledge or questions in the comments.

<br>
<br>

  ##  [HOW TO CREATE A DATABASE?]()
Creating a database and designing related tables is fundamental for a data engineer. It is crucial to follow best practices to ensure efficiency and performance.

What are the best practices for creating relational databases?

Normalization: Apply the three normalization rules to avoid redundancies.
Keys: Understand primary keys, foreign keys, business keys, and surrogate keys.
Data types: Correctly identify the data types for each attribute.
How to create a database and tables in SQL?

Creation syntax: Use CREATE DATABASE database_name; for the database and CREATE TABLE table_name (attributes); for the tables.
Consistency in names: Maintain a uniform format (uppercase or lowercase) for table and attribute names.
What to consider when defining table attributes?

Primary key: Choose a unique key, such as an auto-incremental ID.
Business attributes: Use business keys for external identification.
Data types: Select appropriate types, such as INTEGER for IDs and VARCHAR for text.
Why is it important to record dates in tables?

Traceability: Include date_loaded and date_modified to monitor changes and support data-driven decisions.
Compliance: Ensure data is up-to-date and documented.
How to relate tables using foreign keys?

Foreign key: Define the relationship between tables using FOREIGN KEY pointing to the primary key of another table.
Example: Relate students and courses with an intermediate table containing the foreign keys student_id and course_id.
By following these practices, you will achieve efficient, well-structured, and easy-to-maintain databases.

<br>
<br>

  ##  [PRACTICE: YOUR FIRST QUERY]()

<br>
<br>

  ##  [SQL HISTORY AND EVOLUTION]()

<br>
<br>

  ##  [PRACTICE: ``CREATE TABLE``]()

<br>
<br>
<br>

# DATA MANIPULATION
  ##  [``INSERT`` DATA]()

<br>
<br>

  ##  [``SELECT`` DATA]()

<br>
<br>

  ##  [PRACTICE: ``SELECT`` IN SQL]()

<br>
<br>

  ##  [``UPDATE``DATA]()

<br>
<br>

  ##  [``DELETE``DATA]()

<br>
<br>

  ##  [PRACTICE: CRUD WITH SQL]()

<br>
<br>
<br>

# ADVANCED DATA MANIPULATION
  ##  [MYSQL SERVER AND MYSQL WORKBENCH INSTALLATION]()
  ##  [WHAT IS THE SQL ``WHERE``CLAUSE?]()
  ##  [FILTER AND ORDER DATA IN SQL (``LIKE``)]()
  ##  [TEXTUAL COMPARISON CLAUSES IN SQL (``AND``, ``NULL``, ``IN``, ``NOT``)]()
  ##  [BASIC ARITHMETIC FUNCTIONS IN SQL (``MIN``, ``MAX``)]()

<br>
<br>
<br>

# DATA GROUPING
  ## [SQL DATA GROUPING: ``GROUP BY``, ``HAVING`` AND ``CASE`` FOR ADVANCED ANALYTICS]()

<br>
<br>

  ## [PRACTICE: DATA GROUPING AND SORTING]()

<br>
<br>

  ## [HOW DO THE ``INNER JOIN``, ``LEFT JOIN``, ``RIGHT JOIN`` AND ``FULL JOIN`` WORK]()

<br>
<br>

  ## [PRATICE: SQL LEFT JOIN]()


<br>
<br>
<br>

# DATA TRANSFORMATION
  ##  [SQL MATERIALIZED VIEWS: HOW TO OPTIMIZE YOUR QUERYS AND REPORTS]()

<br>
<br>

  ##  [PRATICE: CREATE SQL MATERIALIZED VIEWS]()

<br>
<br>

  ##  [SQL DATABASE OPTIMIZATION: ``CREATE INDEX`` AND ``TRIGGER``]()

<br>
<br>

  ##  [SQL MATERIALIZED AND TEMPORARY VIEWS]()

<br>
<br>

  ##  [SQL COMMON TABLE EXPRESSIONS]()

<br>
<br>
<br>

# STORED PROCEDURES
  ##  [SQL STORED PROCEDURES]()

<br>
<br>

  ##  [SQL STORED PROCEDURES: VARIABLE MANAGEMENT AND EXCEPTION HANDLING]()

<br>
<br>

  ##  [DATABASE BACKUPS AND RESTORATION]()

<br>
<br>

  ##  [SQL DATABASE SECURITY]()

<br>
<br>
<br>

# ADVANCED DATA ANALYTICS 
  ##  [POWERING DATA IN THE CLOUD: DATA SCIENCE, BIG DATA, ML AND AI]()

<br>
<br>

  ## [SQL FOR DATA ANALYTCS: FIRST STEPS WITH POWER BI]()

<br>
<br>
<br>

# AUTHOR
This project was developed by *Juan Cumbe*. If you have any questions or suggestions about the project, feel free to contact me via [e-mail](mailto:hello@juancumbe.com) or my [Linkedin](https://www.linkedin.com/in/juancumbeq/) profile.