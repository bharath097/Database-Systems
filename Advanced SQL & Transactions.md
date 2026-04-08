# 📊 Database Systems – Assignment 3 (Advanced SQL & Transactions)

# Overview

In this assignment, I worked on advanced database concepts including recursive queries, privilege management, and transaction isolation levels. This assignment helped me understand not just how to query data, but also how databases manage access control and ensure consistency in concurrent environments.

# What I Worked On

 I implemented recursive SQL queries to traverse hierarchical data.
 I analyzed and explained database privilege systems (GRANT and REVOKE).
 I studied transaction isolation levels and their real-world impact.
 I explored concurrency issues like dirty reads, phantom reads, and lost updates.

# How I Implemented the Assignment

# Recursive Query for Hierarchical Data

I used a recursive SQL query (`WITH RECURSIVE`) to traverse the `Part_Structure` table and generate a complete sequence of parts starting from a root part.

I started from a parent part (e.g., P1)
Recursively fetched all dependent sub-parts
Built a complete traversal path

This helped me understand how hierarchical or graph-like data can be processed using SQL itself. 

# Privilege Management (GRANT & REVOKE)

I analyzed how privileges are distributed and revoked in a database system.

 I explained the difference between:

   Standard Grant (cannot pass privilege)
   Grant Option (can pass privilege further)

 I tracked how privileges flow between users and how revoking access affects others.

 I studied the **cascade effect**, where revoking a privilege from one user removes access from dependent users.

This gave me a clear understanding of database security and access control. 

# Transaction Isolation Levels

I compared two important isolation levels:

 Read Uncommitted
 Serializable

For multiple scenarios, I analyzed:

 How concurrent transactions interact
 What kind of issues can occur:

   Dirty reads
   Lost updates
   Phantom reads

I also explained how stricter isolation levels prevent these issues by enforcing controlled execution order.

# Real-World Scenario Analysis

Instead of just theory, I evaluated different transaction combinations like:

 Read-only vs update transactions
 Delete vs insert conflicts
 Concurrent updates

This helped me understand how real database systems maintain consistency under concurrency.

# Technologies Used

 SQL (Advanced queries, recursive queries)
 Relational Database Concepts
 Transaction Management Theory

# Key Learnings

 I learned how to write recursive SQL queries for hierarchical data traversal.
 I gained a strong understanding of database security and privilege propagation.
 I understood how transaction isolation levels affect data consistency.
 I learned how concurrency issues arise and how databases handle them.
 I developed the ability to analyze real-world database scenarios.

# How to Run

1. Create required tables (like `Part_Structure`)
2. Insert hierarchical data
3. Execute recursive SQL queries
4. Observe outputs for traversal results

# What Makes This Work Strong

 I implemented recursion directly in SQL (advanced concept)
 I combined practical queries with theoretical understanding
 I analyzed real-world database behavior (not just syntax)
 I covered security, concurrency, and data consistency together

---
