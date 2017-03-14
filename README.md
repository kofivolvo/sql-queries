#SQL Queries

## Overview
Today we are going to explore the language with which we will persist the data for our applications, SQL, or Structured Query Language.

I'll talk a bit about the concept behind SQL, the relational database, but we will also be playing around with the database as we go over these major concepts. 

To do that, we'll begin with the Microsoft Chinook database, available at https://chinook.ml. This database comes loaded with data, but we'll delete all of that data for our purposes this morning. This afternoon you'll be using the built-in data to practice queries. 

## Getting Started
If you haven't already done so, open https://chinook.ml in another tab. You can look at the schema on the left side of the site to see the data that comes with chinook, but when you are ready, us the scripts in the drop_table.sql script to remove the standard data. Then we can start fresh. 

We will be building a few tables together to cover queries, but we can also use the world data, originally provided by the MySQL foundation, for more complex data. I have modified the data to work with the dialect used by Chinook, and I have removed a few data points from the records. I believe the statistics are a few years out of date, but they are still interesting.  

## Create
We'll cover database and table creation in more depth tomorrow, but we need to do a few basic create statements to get things running. 

### Table Creation
Chinook creates the database schema for us, but we still need to create a table. The basic format is as follows: 

```
CREATE TABLE table_name (
    col_name data_type options,
    col_name data_type options
)
```

Don't worry too much about the data types yet. We'll mostly be using some form of text and some numeric type for most of our data. 

Create a table of your own. Feel free to use this as a model: 
```
CREATE TABLE expenses (
    id integer,
    name text,
    amount real
)
```

### Record/Row Creation
Now that we have a table, we need to insert some records. These become rows in the tables. Here's the basic format: 

```
INSERT INTO table_name (col_name, col_name) VALUES (value1, value2);
```

For the expense table above, we'd need to insert the data as follows: 

``` 
INSERT INTO expenses (id, name, amount) VALUES (1, 'Coffee', 3.78)
```

Okay, that's enough for creation today. Let's spend our time today focusing on existing data. 

## Read
To retrieve data from our database, we use the `SELECT` statement. 

### The Basics
#### SELECT statements


#### Tables Names, Aliases, and Wildcards


#### WHERE clauses


#### ORDER BY clauses


#### LIMIT clauses


#### Calculated Values and Built-In Functions

### Joining Data Across Tables

## Update

## Delete