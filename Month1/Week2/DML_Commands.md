# Data Manipulation Commands in SSMS:
First, let's start with the `INSERT command.` The INSERT command is used to `add one or more rows` of data to a table. Here are `some examples` of how to use the `INSERT command` in SQL Server Management Studio (SSMS):

Inserting data with an `Identity column:`
An Identity column is a column that `automatically generates` a unique value for each row added to the table. To insert data into a table with an Identity column, you do not need to specify a value for the Identity column. The value will be `generated automatically.`

Here's an example of how to insert data into a table with an Identity column:

```sql
-- Create a table with an Identity column
CREATE TABLE ExampleTable (
   ID int IDENTITY(1,1) PRIMARY KEY,
   Name varchar(50),
   Age int
)

-- Insert data into the table
INSERT INTO ExampleTable (Name, Age) VALUES ('John', 30)
INSERT INTO ExampleTable (Name, Age) VALUES ('Jane', 25)

````
In this example, we first create a table called `ExampleTable` with an Identity column called `ID.` We then insert two rows of data into the table using the INSERT command. Notice that we do not `specify a value` for the ID column because it will be generated automatically.

## Creating a table from another table:
You can use the `SELECT INTO statement` to create a `new table` based on the results of a `SELECT statement.` Here's an example:
```sql
-- Create a table called NewTable based on the results of a SELECT statement
SELECT Name, Age
INTO NewTable
FROM ExampleTable
WHERE Age > 25
````
In this example, we create a new table called `NewTable` based on the results of a `SELECT statement.` The SELECT statement selects the `Name and Age` columns from the `ExampleTable` where the Age is greater than 25. The resulting data is then inserted into the NewTable.
## Inserting rows from one table to another:

You can use the INSERT INTO statement to insert data from one table into another. Here's an example:
```sql
-- Create a new table called OtherTable
CREATE TABLE OtherTable (
   ID int,
   Name varchar(50),
   Age int
)

-- Insert data from ExampleTable into OtherTable
INSERT INTO OtherTable (ID, Name, Age)
SELECT ID, Name, Age
FROM ExampleTable
WHERE Age > 25
````
In this example, we first `create a new table` called `OtherTable.` We then use the `INSERT INTO` statement to insert data from the `ExampleTable` into the `OtherTable.` The `SELECT` statement selects the `ID, Name, and Age` columns from the `ExampleTable` where the `Age` is greater than 25. The resulting data is then inserted into the OtherTable.

## UPDATE Command:
The `UPDATE` command is used to `modify` existing records in a table. Here's an example:

Suppose you have a table called `OtherTable` with the following columns: `ID, Name, and Age.` You want to update the Age for a specific customer with `ID 1.` Here's how you can do it:
```sql
UPDATE OtherTable
SET Age = '31'
WHERE ID = 1;
```
## DELETE Command:
The `DELETE` command is used to `remove one or more records` from a table. There are two variations of the DELETE command: `DELETE and TRUNCATE.` The main difference between the two is that `TRUNCATE` removes `all records` from a table, while `DELETE` can be used to remove `specific records.`
```sql
DELETE FROM OtherTable
WHERE Id = 1;
```
## Truncate:
The `TRUNCATE` command is used to delete `all the rows` from a table. Unlike the `DELETE` command, which deletes `rows one by one`,` TRUNCATE removes all the rows in one go. Here's the syntax for the TRUNCATE command:
```sql
TRUNCATE TABLE OtherTable;
```
