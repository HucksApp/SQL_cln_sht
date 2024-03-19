# SQL Clean Sheet



A ***Database*** is a set of related informations. A collection of integrated records

A database management system (DBMS) is a set of programs used to define, administer, and process databases and their associated applications

## Database
Over the first several decades of computerized database systems, data was stored and represented to users in various ways
  *  hierarchical database system -> data is represented as one or more tree structures, this are now used in directory service (database for storing and maintaining           information about users and resources of a machine i.e computer) of  Microsoft’s Active Directory, the Red Hat Directory Server etc.
  *  network database system

## Common Database Models
* The Relational Model  -> 
* The object Model (Non relational) ->
* The object-relational model -> Most relational DBMS(extended) now have support for object models


## The Relational Model database system

Data are represented as sets of tables, redundant data is used to link records in different tables and this are used to navigate between related entities

* ***PRIMARY KEY*** -> Each row(line entries) has a unique identifier that can belong to no other entry
* ***FOREIGN KEY*** -> (This are the redundant data) This are *primary key* or unique identifier on another table serving as a *foreign* key on the present table, showing the relation between the two tables
* Schemas -> The structure of an entire database is its schema, or conceptual view
* Domains -> An attribute of a relation (A single column) ranges of possible values
* Constraints -> A restriction on what a column may contain

### Data Types
* Numerics data type
  * *INTEGER* 
  * *SMALLINT*
  * *BIGINT*
  * *NUMERIC*
  * *DECIMAL* 
  * *REAL* 
  * *DOUBLE PRECISION*
  * *FLOAT*
  
* Strings data type
  * *CHARACTER* ->  sample `CHARACTER (20)`
  * *VARCHAR* -> VARYING CHARACTERS. sample `VARCHAR (20)`
  * *CLOB* -> CHARACTER LARGE OBJECT. sample `CLOB (1000000)`
* media data type
   * *BLOB* -> BINARY LARGE OBJECT. sample `BLOB (1000000)`
 
* Booleans  data type
   * *BOOLEAN*
 
* *NULL* data type
  
* Datetimes data type
   * *DATE*
   *  *TIME WITH TIME ZONE* -> `TIME (3) WITH TIME ZONE`
   * *TIME WITHOUT TIME ZONE* -> `TIME (2) WITHOUT TIME ZONE`
   * *TIMESTAMP WITHOUT TIME ZONE*  -> `TIMESTAMP WITHOUT TIME ZONE (0)`
   * *TIMESTAMP WITH TIME ZONE* -> `TIMESTAMP WITH TIME ZONE (0)`
 
* Intervals
  * *INTERVAL* -> `INTERVAL DAY`
* *ROW* types -> Allows you nest a row within a row.`CREATE ROW TYPE <row type>(<nexted row 1> <nexted row 1> ...)` now use in table defination `CREATE TABLE <table name> ( <row defination>    <row defination : <row type>> ...)`
* Collection types
  * *ARRAY* -> `<Column Defination  ARRAY [size]>`
  * *MULTISET* ->

* *REF* types
* User-defined types (UDTs)
  * *DISTINCT* -> `CREATE DISTINCT TYPE <type_name> AS <Data_type_defination> ;`
* Structured types 
  * `CREATE TYPE <type name> AS <structure_member1_defination, structure_member2_defination, ...>`

## STRUCTURED QUERY LANGUAGE (SQL)

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


# Common Relational DBMS

## MYSQL
* server installation
   * macOS -> `$ brew install mysql`
* Client installation
   * python -> `$ pip install mysql`
* start server -> `$ brew services start mysql`
* start cmd interface -> `$ mysql -h <host> -u <user> -p`





# POSTGRESQL 

* server installation
   * macOS -> 
* Client installation
   * python -> 
* start server -> 
