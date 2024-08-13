 User Management System - CRUD Operations

This repository contains a Jupyter Notebook that implements CRUD operations for a user management system using a MySQL relational database. The `users` table includes the following fields:
- `id`: Primary Key
- `name`: String
- `email`: String (unique)
- `created_at`: Timestamp

## Tasks

1. **Create a New User**: Insert a new user into the `users` table.
2. **Read User Details by ID**: Fetch and display details of a user based on their ID.
3. **Update a User's Email**: Update the email address of a user by their ID.
4. **Delete a User by ID**: Remove a user from the `users` table by their ID.


## Usage

1. **Connect to the MySQL Database**:
   Ensure that your MySQL server is running and that you have created a database named `user_management`. Update the connection details in the notebook as needed.

2. **Run the Jupyter Notebook**:
   Launch Jupyter Notebook in the project directory:
Connect to the MySQL Database:
Update the database connection details in the Jupyter Notebook with your MySQL server configuration.

3. **Create the users Table**:
Run the cell in the Jupyter Notebook that creates the users table with the necessary schema.

4. **Perform CRUD Operations**:

    **Create a New User**: Run the cell that defines the create_user function and provides an example usage.
    **Read User Details by ID**: Run the cell that defines the read_user function and provides an example usage.
    **Update a User's Email**: Run the cell that defines the update_user_email function and provides an example usage.
    **Delete a User by ID**: Run the cell that defines the delete_user function and provides an example usage.

5. **Close the Connection**:
Run the final cell to close the database connection.

   Open the notebook and execute the cells to perform CRUD operations on the `users` table.

## Strengths and Weaknesses of Relational Databases

### Strengths
- **ACID Compliance**: Ensures reliable transactions and data integrity.
- **Data Integrity**: Strong data integrity through foreign keys, constraints, and normalization.
- **Complex Queries**: Supports complex SQL queries and joins across multiple tables.
- **Standardization**: SQL is a widely adopted standard for database queries.

### Weaknesses
- **Scalability**: Vertical scaling can become expensive and challenging for very large datasets.
- **Rigid Schema**: Schema changes can be difficult and time-consuming.
- **Performance**: May suffer in write-heavy applications or with large volumes of unstructured data.

## Handling Scalability Beyond 10TB

To handle large datasets beyond 10TB, consider the following techniques:

- **Partitioning**:
  - **Horizontal Partitioning (Sharding)**: Split large tables across multiple databases or servers.
  - **Vertical Partitioning**: Split tables into smaller tables with fewer columns.

- **Sharding**:
  - Distribute data across multiple servers based on a shard key.

- **Indexing**:
  - Use indexes on frequently queried columns.

- **Caching**:
  - Implement caching layers (e.g., Redis, Memcached) to reduce database load.

- **Data Archiving**:
  - Move old data to an archive or data warehouse.

- **Database Optimization**:
  - Regularly optimize queries and monitor performance.



