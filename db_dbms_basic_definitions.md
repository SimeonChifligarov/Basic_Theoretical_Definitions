
# Storage vs. Management
	[...]

# Databases and DBMS

 - A database is an organized collection of related information
	[...]

 - Data Base Management System 
	[...]

# DB Engine
	[...]

# Database Table Elements
	[...]

# Table Relations
	[...]

# Foreing key
 - The foreign key is an identifier of a record located in another table (usually its primary key)
 - By using relationships, we avoid repeating data in the database 
 - Relationships:
    One-to-many 	[...]
    Many-to-many 	[...]
    One-to-one 		[...]


# SQL
	[...]

 - Subdivided into several language elements
	- Queries, Statements, Clauses, Expressions, Predicates

# SQL
 - Logically divided into four sections
    - Data Definition Language – describe the structure of our data
       CREATE, ALTER, DROP
    - Data Manipulation Language – store and retrieve data
       SELECT, INSERT, UPDATE, DELETE
    - Data Control Language – define who can access the data
       GRANT, REVOKE, DENY
    - Transaction Control Language – bundle operations and allow rollback 
       COMMIT, ROLLBACK, SAVE

# SQL vs NoSQL
 - SQL:
	[...]
 - NoSQL:
	[...]

# Data Types
 - String Types - CHARACTER/CHAR[(M)], CHARACTER VARYING/VARCHAR[(N)], TEXT
 - Numeric Data Types:
	- Integer types - SMALLINT, INTEGER/INT, BIGINT
	- Arbitrary Precision Numbers - DECIMAL, NUMERIC
	- Floating-Point Types - REAL, DOUBLE PRECISION
	- Serial Types - SMALLSERIAL, SERIAL, BIGSERIAL
 - Date Types - DATE, TIME, TIMESTAMP, TIMESTAMPTZ

# Custom Column Properties
 - Primary Key
	[...]

 - Foreign Key
	[...]

 - Unique constraint – no repeating values in entire table
	[...]

 - Default value – if not specified (otherwise set to NULL)
	[...]


# Basic SQL Commands
 - Create, Read, Update, Delete


# PostgreSQL
 - Lexical structure in PostgreSQL

# Deleting Data
	[...]

# DELETE CASCADE statement
	[...]

# Retrieving Data => Using SQL SELECT
 - Capabilities of SQL SELECT Statements
    - Projection = Take a subset of the columns
    - Selection = Take a subset of the rows
    - Join = Combine tables by some column

 - Capabilities of SQL SELECT Statements
	[...]

# Filtering the Selected Rows
 - DISTINCT 	[...]
 - WHERE clause	[...]
 - Logical and comparison operators can be used

# Other Comparison Conditions
 - using NOT, OR, AND and brackets

 - Using BETWEEN operator to specify a range

 - Using IN / NOT IN to specify a set of values (*membership condition*)

 - The LIKE Condition
	[...]


# Null Values
	[...]

# Comparing with NULL
 - NULL is a special value that means missing value
    Not the same as 0 or a blank space
 - Checking for NULL values:
	WHERE manager_id = NULL (always false)
	WHERE manager_id IS NULL
	WHERE manager_id IS NOT NULL

# Sorting with ORDER BY
 - Sort rows with the ORDER BY clause
    - ASC: ascending order, default
    - DESC: descending order

# The ORDER BY Clause
	[...]


# Joins
	[...]

# #TODO
 - LEFT, RIGHT, INNER JOIN... !!!


# Views
	[...]

 - Usage
    - To simplify writing (complex) queries 
    - To limit access to data for (certain) users


# Aggregate Functions
 - Compute a single result from multiple input rows:
 - They are count(), sum(), avg(), max() and min()
	[...]

============================================================================

# Python and PostgreSQL

# Psycopg2
 - PostgreSQL database adapter for the Python
	[...]

# The connect() function
	[...]

import psycopg2

conn = psycopg2.connect(
    host="localhost",
    database="database_name",
    user="user_name",
    password="password")

conn.close()

# The cursor() method
	[...]

cur = conn.cursor()

cur.execute("CREATE TABLE employee(name varchar(20))")
conn.commit()

cur.close()
