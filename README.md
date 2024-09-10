# SQLite Friends Database Project

## Project Overview

This project showcases fundamental SQL operations using SQLite. It involves creating a database, manipulating data, and modifying table structures. The focus is on practical SQL skills applicable across various relational database systems.

## Key Features

- **Database Creation**: Set up an SQLite database and define a schema.
- **Data Management**: Insert, update, and delete records.
- **Schema Modification**: Alter table structures and manage new columns.
- **Data Retrieval**: Query and display data from the database.

## SQL Commands

### 1. Create Table

Define a table named `friends` with columns for `id`, `name`, and `birthday`.

```sql
CREATE TABLE friends (
  id INTEGER PRIMARY KEY,
  name TEXT NOT NULL,
  birthday DATE
);
```

### 2. Insert Data

Add sample records to the `friends` table.

```sql
INSERT INTO friends (id, name, birthday)
VALUES (1, 'Ororo Munroe', '1940-05-30'),
       (2, 'Mamademama', '1962-08-17'),
       (3, 'Jeroentje', '1989-07-05');
```

### 3. Update Records

Change the name of the friend with `id = 1`.

```sql
UPDATE friends
SET name = 'Storm'
WHERE id = 1;
```

### 4. Alter Table

Add an `email` column to the existing `friends` table.

```sql
ALTER TABLE friends
ADD COLUMN email TEXT;
```

### 5. Update Email

Assign an email address to the friend with `id = 1`.

```sql
UPDATE friends
SET email = 'storm@codecademy.com'
WHERE id = 1;
```

### 6. Delete Records

Remove the record with `id = 1` from the table.

```sql
DELETE FROM friends
WHERE id = 1;
```

### 7. Select Records

Retrieve all records from the `friends` table to view the current data.

```sql
SELECT * FROM friends;
```

## Learning Outcomes

- **Understanding SQL Syntax**: Gained proficiency in writing and executing SQL commands.
- **Data Management**: Experienced with inserting, updating, and deleting records.
- **Schema Design**: Practiced designing and modifying database schemas.
- **Practical Application**: Applied SQL concepts to manage and manipulate real data.

## How to Run

1. **Set Up SQLite**:
   - Download and install SQLite from [SQLite official site](https://www.sqlite.org/download.html).
   - Open the SQLite command-line interface.

2. **Create and Manage Database**:
   - Run `sqlite3 friends.db` to create and open the database.
   - Execute SQL commands to create tables, insert data, and perform other operations.

3. **View Results**:
   - Use `SELECT * FROM friends;` to view the data and verify operations.

## Conclusion

This project demonstrates essential SQL skills using SQLite, providing a practical foundation for managing relational databases. It highlights key operations from creating tables to data manipulation and schema modification.

Feel free to explore and extend this project to further your understanding of SQL and database management.
