# SQL Clean Sheet



A ***Database*** is a set of related informations. A collection of integrated records

A database management system (DBMS) is a set of programs used to define, administer, and process databases and their associated applications

## Database
Over the first several decades of computerized database systems, data was stored and represented to users in various ways
  *  hierarchical database system -> data is represented as one or more tree structures, this are now used in directory service (database for storing and maintaining           information about users and resources of a machine i.e computer) of  Microsoft’s Active Directory, the Red Hat Directory Server etc.
  *  network database system

## Common Database Models
* The Relational Model
* The object Model
* The object-relational model -> Most relational DBMS(extended) now have support for object models


## The Relational Model database system

Data are represented as sets of tables, redundant data is used to link records in different tables and this are used to navigate between related entities

* ***PRIMARY KEY*** -> Each row(line entries) has a unique identifier that can belong to no other entry
* ***FOREIGN KEY*** -> (This are the redundant data) This are *primary key* or unique identifier on another table serving as a *foreign* key on the present table, showing the relation between the two tables
* Schemas -> The structure of an entire database is its schema, or conceptual view
* Domains -> An attribute of a relation (A single column) ranges of possible values
* Constraints -> A restriction on what a column may contain




# STRUCTURED QUERY LANGUAGE (SQL)

SQL statements are divided into two major categories: data definition language (DDL) and data manipulation language (DML). 


## Data definition language

### CREATE
```
CREATE TABLE <table name> ( 
        <attribute name 1> <data type 1>,
        ...
        <attribute name n> <data type n>);
```

### ALTER

```
 ALTER TABLE <table name>
        ADD CONSTRAINT <constraint name> PRIMARY KEY (<attribute list>);
```


### DROP
```
  DROP TABLE <table name>;
```

