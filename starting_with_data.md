Question 1:  Explore the whole ecommerce database in a summarized way.

SQL Queries:
        SELECT table_name, column_name, data_type
        FROM information_schema.columns
        WHERE table_schema = 'public'
        Order by table_name

Answer: Can identify wrong data types in different tables and give you idea on how to relate the tables.
      
Question 2:  Look for dupplicate in the particular column:

SQL Queries: Compare the below query of columns with and witout DISTICNT.
        SELECT (DISTINCT) coumn_name FROM table_name

Answer: If there dupliates the number of rows in the output will be different.

Question 3: Check and verify how much of the table column has Null value:

SQL Queries: Check the column for both "is Null" and "not Null"
       SELECT column_name FROM table_name WHERE column_name is Null(not Null)

Answer: You can have an idea how much of the total rows actually have Null values and plan for the next action.

Question 4:  Change the irrelevant data types of certain columns to the data type that conforms to the values in the column.

SQL Queries: 
        ALTER TABLE table_name
        ALTER COLUMN column_name TYPE dat_type

Answer: The above will change data type of a column in to the desired data type.

Question 5: How to replace missing data or null value with relevant data value:
  

SQL Queries:
        UPDATE table_name 
        SET column_name = "value"
        WHEN column_name is Null.

Answer: Fills missing information or replace the previous values.
