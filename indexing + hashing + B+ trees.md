# Database Systems – Assignment 5 (Indexing & Hashing Techniques)

# Overview

In this assignment, I worked on advanced database indexing and hashing techniques, including B+ trees, extensible hashing, and linear hashing. I also analyzed index structures and calculated storage requirements for dense and sparse indexing.

This assignment helped me understand how databases efficiently store and retrieve data at scale.


# What I Worked On

 I implemented step-by-step construction of B+ trees with insert and delete operations.
 I analyzed extensible hashing and how directory expansion works.
 I implemented linear hashing and tracked bucket splitting dynamically.
 I calculated index sizes and storage requirements for dense and sparse indexes.
 I understood how indexing improves database performance.

# How I Implemented the Assignment

# B+ Tree Construction

I manually constructed a B+ tree by:

 Inserting values step by step
 Handling node splits when capacity is exceeded
 Maintaining sorted order and tree balance
 Performing deletion operations and restructuring the tree
This helped me understand how indexing structures maintain efficiency for search operations. 

# Extensible Hashing

I implemented extensible hashing by:

 Using a directory with global depth
 Splitting buckets when overflow occurs
 Increasing directory size dynamically
 Mapping binary hash values to buckets
I tracked how local and global depths change as new values are inserted.

# Linear Hashing

I simulated linear hashing by:

 Monitoring load factor (U)
 Expanding buckets when threshold is exceeded
 Incrementally splitting buckets instead of full rehashing

This helped me understand how databases handle dynamic growth efficiently.

# Indexing (Dense vs Sparse)

I calculated storage requirements for different indexing strategies:

 Dense Index:

   One index entry per record
   Higher storage but faster lookup

 Sparse Index:

   One index entry per block
   Lower storage but slightly slower lookup

I computed:

 Number of entries per block
 Total blocks required
 Trade-offs between space and performance

# Technologies Used

 Database Concepts (Indexing, Hashing)
 B+ Tree Algorithms
 Hashing Techniques (Extensible, Linear)

# Key Learnings

 I understood how B+ trees maintain balanced indexing structures.
 I learned how hashing techniques dynamically manage data growth.
 I gained insight into how indexing improves query performance.
 I learned how to calculate storage and block usage in databases.
 I developed a strong understanding of database internals.

# How to Run

This assignment is conceptual and simulation-based:

1. Follow step-by-step insert/delete operations
2. Construct tree and hashing structures manually
3. Verify structure correctness after each step

# What Makes This Work Strong
 I implemented core database indexing structures manually
 I understood how real databases optimize search and storage
 I worked with multiple hashing strategies
 I combined theoretical understanding with step-by-step execution

---
