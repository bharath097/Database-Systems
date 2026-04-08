# Database Systems Assignment – SQL Query Implementation

# Overview
In this project, I worked on writing advanced SQL queries using a relational database schema involving students, courses, departments, and enrollments. The goal was to extract meaningful insights from the data by combining multiple tables and applying different SQL concepts.


# Concepts I Applied

1. worked with relational database structures involving multiple tables like `student`, `enroll`, `course`, `major`, and `department`.
2. used SQL joins to combine data across tables based on relationships.
3. applied aggregation functions like `AVG`, `MAX`, and `MIN` to compute results.
4. used filtering techniques such as `WHERE`, `HAVING`, and `DISTINCT`.
5. implemented subqueries and nested queries for complex conditions.
6. used `GROUP BY` to organize data and perform grouped calculations.
7. applied set operations like `UNION` and `EXCEPT`.
8. used `LEFT JOIN` and `COALESCE` to handle missing data.

# How I Implemented the Queries

# Joining Multiple Tables

I combined tables like `enroll`, `student`, and `course` using joins to compute values such as the average GPA per course section. This helped me understand how relational data is connected and how to extract combined insights.

# Aggregations and Grouping

I used aggregation functions like `AVG(s.gpa)` and grouped results using `GROUP BY` to calculate metrics such as:

1. Average GPA per course
2. Average GPA per department
3. Age differences among students

# Filtering Data

I applied conditions using:

`WHERE` to filter rows before grouping
`HAVING` to filter grouped results (like courses with fewer than 6 students)

# Handling Missing Data

I used `LEFT JOIN` along with `COALESCE` to ensure that even students without a declared major were included in the results, replacing null values with empty strings.

# Subqueries and Nested Logic

I implemented nested queries to solve complex problems such as:

Finding departments not associated with certain courses
Identifying students who satisfy multiple conditions
Using `NOT EXISTS` and `EXCEPT` to compare sets of data

# Set Operations

In Part B, I used `UNION ALL` to combine results from multiple tables (PC and Laptop) and compute overall averages.

# Technologies Used

* SQL (PostgreSQL / MySQL style queries)
* Relational Database Concepts

# Key Learnings

1. learned how to write complex SQL queries involving multiple joins and conditions.
2. gained hands-on experience with aggregation and grouping operations.
3. understood how to structure nested queries for real-world scenarios.
4. improved my ability to think in terms of relational data and dependencies.
5. learned how to handle incomplete data using joins and null-handling techniques.

# How to Run

1. Create the database schema with required tables (`student`, `enroll`, `course`, etc.)
2. Insert sample data into each table.
3. Run the SQL queries provided in the assignment.
4. Verify outputs similar to the results shown in the screenshots.


# What Makes This Work Strong

1. handled complex multi-table relationships correctly.
2. used advanced SQL features like subqueries, set operations, and conditional filtering.
3. ensured queries return meaningful and accurate results based on the problem requirements.
4. validated outputs with actual query results.
