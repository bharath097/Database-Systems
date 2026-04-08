# Database Systems – Assignment 2 (SQL + Java Integration)

# Overview

In this assignment, I worked on integrating SQL with Java to interact with a relational database and perform operations programmatically. I implemented both database-side logic (SQL) and application-side logic (Java using JDBC), which helped me understand how backend systems interact with databases.

# What I Worked On

created and populated relational tables such as `Part_Structure` and `Students1`.
wrote SQL queries to retrieve and manipulate hierarchical and structured data.
implemented Java programs to connect to the database and execute queries.
worked on recursive and traversal-based logic using database relationships.
built a menu-driven Java application to perform CRUD operations.

# How I Implemented the Assignment

# Table Creation and Data Handling

I created tables like `Part_Structure` with attributes such as major part, minor part, and quantity, and inserted sample data to simulate a hierarchical structure. 

# Java + Database Connection (JDBC)

I wrote Java programs where I:
Connected to the database using credentials
Executed SQL queries from Java
Retrieved and displayed results in the console

This helped me understand how applications communicate with databases in real-world systems.

# Implementing Traversal Logic (Recursive Behavior)

I implemented logic to traverse the `Part_Structure` hierarchy.
This involved:

 Starting from a parent part
 Recursively finding all dependent sub-parts
 Printing the traversal order
This gave me exposure to solving graph-like problems using database tables.

# Stored Procedures / Functions

I implemented database-side logic using functions (like traversal functions) to process hierarchical data directly inside the database.

# Menu-Driven CRUD Application

I built a Java-based interactive program that allows users to:

 Execute SQL queries
 Insert data
 Update records
 Delete records
 Create tables

The program takes user input and dynamically executes SQL commands, simulating a simple database management interface. 

# Data Validation and Output Handling

I ensured:

 Correct query execution
 Proper output formatting
 Handling cases where no records are found

# Technologies Used

SQL (PostgreSQL / relational database)
Java
JDBC (Java Database Connectivity)

# Key Learnings

I learned how to connect Java applications with databases using JDBC.
I gained hands-on experience executing SQL queries programmatically.
I understood how hierarchical data can be modeled and traversed using database tables.
I implemented CRUD operations through a real interactive program.
I improved my problem-solving skills by combining database logic with programming.

# How to Run
1. Set up the database and create required tables.
2. Insert sample data into the tables.
3. Compile Java files:

   ```
   javac QuestioncodeX.java
   ```
4. Run the program:

   ```
   java QuestioncodeX <dbname> <username> <password>
   ```
5. Follow menu options or program output.

# What Makes This Work Strong

 I combined SQL with Java, which reflects real backend development.
 I implemented traversal logic, not just basic queries.
 I built an interactive system instead of writing static queries.
 I handled real-world database operations like insert, update, and delete.
