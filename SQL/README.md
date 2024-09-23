SQL (Structured Query Language) is a standardized programming language used to manage and manipulate relational databases. It allows users to query, insert, update, delete, and manage data stored in a database.

### Key SQL Commands:
- SELECT: Retrieves data from a database.
- INSERT: Adds new data to a database.
- UPDATE: Modifies existing data.
- DELETE: Removes data.

```sql
-- Retrieve all users from a table named 'users'
SELECT * FROM users;

-- Insert a new record into the 'users' table
INSERT INTO users (name, email) VALUES ('John Doe', 'john@example.com');

-- Update a user's email in the 'users' table
UPDATE users SET email = 'john.new@example.com' WHERE name = 'John Doe';

-- Delete a user from the 'users' table
DELETE FROM users WHERE name = 'John Doe';
```

### More Resources
https://www.w3schools.com/sql/sql_examples.asp
