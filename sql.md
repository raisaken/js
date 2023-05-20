# What are the different subsets of SQL?
Data Definition Language (DDL) – It allows you to perform various operations on the database such as CREATE, ALTER, and DELETE objects.
Data Manipulation Language(DML) – It allows you to access and manipulate data. It helps you to insert, update, delete and retrieve data from the database.
Data Control Language(DCL) – It allows you to control access to the database. Example – Grant, Revoke access permissions.

# Implementation of the ACID principle

- The atomicity, consistency, isolation, and durability (ACID) concept is not used by DBMSs for data storage. RDBMSes, on the other hand, use the ACID model to organize their data and assure consistency.

# Normalization of databases is supported

A RDBMS can be normalized , but a DBMS cannot be normalized.

# Transaction

- A transaction is a unit of work that is performed against a database. Transactions are units or sequences of work accomplished in a logical order, whether in a manual fashion by a user or automatically by some sort of a database program.

A transaction is the propagation of one or more changes to the database. For example, if you are creating a record or updating a record or deleting a record from the table, then you are performing a transaction on that table. It is important to control these transactions to ensure the data integrity and to handle database errors.

Practically, you will club many SQL queries into a group and you will execute all of them together as a part of a transaction.

# Properties of Transactions

Transactions have the following four standard properties, usually referred to by the acronym ACID.

Atomicity − ensures that all operations within the work unit are completed successfully. Otherwise, the transaction is aborted at the point of failure and all the previous operations are rolled back to their former state.

Consistency − ensures that the database properly changes states upon a successfully committed transaction.

Isolation − enables transactions to operate independently of and transparent to each other.

Durability − ensures that the result or effect of a committed transaction persists in case of a system failure.

# Transaction Control

The following commands are used to control transactions.

COMMIT − to save the changes.

ROLLBACK − to roll back the changes.

SAVEPOINT − creates points within the groups of transactions in which to ROLLBACK.

SET TRANSACTION − Places a name on a transaction.

    - The SET TRANSACTION command can be used to initiate a database transaction. This command is used to specify characteristics for the transaction that follows. For example, you can specify a transaction to be read only or read write.

# Normalization

- Normalization in SQL is the process of organizing data to avoid duplication and redundancy.

# What is the difference between DROP and TRUNCATE commands?

- DROP command removes a table and it cannot be rolled back from the database whereas TRUNCATE command removes all the rows from the table, can be rolled back.

# What is OLTP?

OLTP, or online transactional processing, allows huge groups of people to execute massive amounts of database transactions in real time, usually via the internet. A database transaction occurs when data in a database is changed, inserted, deleted, or queried.

