# A Complete Overview of SQL Concepts

## Introduction

SQL stands for Structured Query Language, and it is the standard language to store, manipulate, and maintain relational databases. SQL encompasses basic concepts that are essential for creating, designing, and optimizing databases. Key topics covered in this document include ACID properties, the CAP Theorem, Joins, Aggregations, Filters, Normalization, Indexes, Transactions, Locking Mechanism, Database Isolation Levels, and Triggers.

## ACID Properties

ACID (Atomicity, Consistency, Isolation, Durability) ensures that database transactions are processed reliably.

- **Atomicity**: Guarantees that database operations are completed as a single unit or not at all.
- **Consistency**: Ensures that transactions always maintain a valid state, preventing invalid data from being written.
- **Isolation**: Ensures concurrent transactions do not affect each other.
- **Durability**: Guarantees that committed transactions are permanent and will survive system failures.

## CAP Theorem

The CAP Theorem (Consistency, Availability, Partition Tolerance) states that not all three properties can be achieved simultaneously in a distributed database:

- **Consistency**: All nodes contain the same copy of data at the same time.
- **Availability**: Data is available and writable at all times.
- **Partition Tolerance**: The system continues to operate despite network partitions.

## Joins

Joins are used to retrieve data from two or more tables based on a related column.

- **Inner Join**: Returns only common rows between both tables.
- **Left Join**: Returns all rows from the left table and matched rows from the right table.
- **Right Join**: Returns all rows from the right table and matched rows from the left table.
- **Full Outer Join**: Returns all rows from both tables, including non-matching rows with NULL values.

## Aggregations and Filters

Aggregations and filters help in summarizing and restricting data.

- **Aggregations**: Perform calculations on data groups, e.g., `SUM`, `AVG`, `MAX`.
- **Filters**: Restrict data based on conditions using clauses like `WHERE`, `HAVING`, and `GROUP BY`.

## Normalization

Normalization is a method to decompose complex tables into simpler ones to minimize redundancy and dependency.

- **1NF (First Normal Form)**: Each table cell should have a single value.
- **2NF (Second Normal Form)**: Non-key attributes depend on the whole primary key.
- **3NF (Third Normal Form)**: Non-key attributes are not transitively dependent on the primary key.

## Indexes

Indexes are data structures that improve query performance by allowing fast look-ups.

- **Primary Index**: An index on a primary key column.
- **Secondary Index**: A non-unique index on a non-primary key column.

## Transactions

A transaction is a series of operations executed as a single unit or not at all.

- **Commit**: Makes changes permanent in a transaction.
- **Rollback**: Reverts any changes made during a transaction.

## Locking Mechanism

Locking mechanisms prevent concurrent transactions from interfering with each other.

- **Pessimistic Locking**: Locks data to prevent other transactions from accessing it.
- **Optimistic Locking**: Assumes transactions will complete without conflicts and checks for conflicts at commit time.

## Database Isolation Levels

Isolation levels define the extent to which transactions are isolated from each other.

- **Read Uncommitted**: Allows reading uncommitted data.
- **Read Committed**: Reads only committed data.
- **Repeatable Read**: Ensures the same query returns the same results within a transaction.
- **Serializable**: Ensures transactions appear to be performed sequentially.

## Triggers

Triggers are automatic actions executed in response to database events.

- **INSERT Trigger**: Fires when a new row is inserted.
- **UPDATE Trigger**: Fires when an existing row is updated.
- **DELETE Trigger**: Fires when a row is deleted.

## Conclusion

Understanding SQL concepts such as ACID properties, CAP Theorem, Joins, Aggregations, Filters, Normalization, Indexes, Transactions, Locking Mechanism, Database Isolation Levels, and Triggers is crucial for designing, developing, and optimizing databases. Mastery of these concepts enables developers and database administrators to create robust and high-performance databases.
