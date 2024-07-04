# BBDD with SQL

<p align="center">
  <img src="https://img.shields.io/badge/Curso%20-Finalizado-brightgreen"/>
</p>

<br>

# INDEX

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
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/scroll-final-render.webp?raw=true" width= "75%" alt="Scroll render">
</p>

  ### How is the Second Normal Form (2NF) applied?
The second normal form (**2NF**) requires that all non-key attributes depend on the primary key. To comply with 2NF, you must first satisfy the requirements of 1NF. This involves separating information into additional tables and using foreign keys to establish relationships. For example, creating a separate table for courses and referencing it from the student table using a foreign key.

  ### What does the Third Normal Form (3NF) entail?
The third normal form (3NF) adds that all non-key attributes must be independent of each other and comply with the previous two forms. Any redundancy and unnecessary dependency should be eliminated. In this case, an intermediate table between students and courses can help maintain the independence of attributes, relating students and courses through unique identifiers.

  ### What are other examples of normalization?
A common example is addresses. An address record can be more atomic if it is divided into separate tables for countries, cities, and departments. Although some companies prefer a single address table, the normalization process always seeks the most efficient and organized structure.

Understanding these forms of normalization and applying them correctly improves the quality and management of data in any database.

<br>
<br>

  ##  [DATATYPES IN SQL]()

<br>
<br>

  ##  [HOW TO CREATE A DATABASE?]()

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