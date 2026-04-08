# Database Systems – Assignment 4 (Storage Design & Advanced Functions)

# Overview

In this assignment, I worked on understanding how data is physically stored inside a database and how complex hierarchical logic can be implemented using database functions. This assignment helped me move beyond query writing and explore database internals and advanced procedural logic.

# What I Worked On

 I analyzed record storage structure including fixed-length and variable-length fields.
 I calculated storage size for database records based on field types.
 I compared different storage strategies using direct storage vs pointer-based storage.
 I implemented recursive database functions using PL/pgSQL.
 I worked on hierarchical traversal and counting logic inside the database.

# How I Implemented the Assignment

# Record Storage Design

I analyzed how a patient record is stored in a database by dividing it into:

 Fixed-length fields (like DOB, SSN, ID)
 Pointers to variable-length fields
 Record length field

I calculated the total size required for storing a record, which helped me understand how databases optimize memory usage. 

# Storage Strategy Comparison

I compared two approaches for storing cholesterol test data:

1. Storing data inside the record

   Record size increases with number of tests
   Formula: `42 + 16n`

2. Storing data using pointers

   Record size remains fixed
   Uses pointers to external storage

This helped me understand trade-offs between space efficiency and data access. 

# Recursive Function for Part Counting

I implemented a recursive PL/pgSQL function (`leafpart`) that:

Takes a parent part and a target sub-part
Traverses the hierarchy recursively
Computes total count of required sub-parts
This involved multiplying quantities across levels, which is similar to solving tree/graph problems inside a database. 


# Recursive Traversal Function

I also implemented a traversal function that:

 Starts from a root part
 Recursively visits all sub-parts
 Prints the traversal order
This helped me understand how recursion can be implemented directly inside the database using stored procedures. 

# Technologies Used

 SQL
 PL/pgSQL (PostgreSQL procedural language)
 Relational Database Concepts

# Key Learnings

 I understood how database records are physically structured in memory.
 I learned how storage design affects performance and scalability.
 I gained experience writing recursive functions inside the database.
 I improved my ability to solve hierarchical problems using database logic.
 I learned how pointers and variable-length fields are managed internally.

# How to Run

1. Create required tables (e.g., `Part_Structure1`)
2. Insert hierarchical data
3. Create functions (`leafpart`, `Traversal`)
4. Execute function calls:

   ```
   SELECT leafpart('P1', 'P6');
   SELECT Traversal('P1');
   ```

# What Makes This Work Strong

 I explored internal database storage concepts (not just queries)
 I implemented recursion inside the database using PL/pgSQL
 I solved hierarchical problems with quantity propagation
 I combined theory (storage design) with practical implementation
