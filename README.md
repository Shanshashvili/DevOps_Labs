# **Database:**
## MySQL

### 1. **MySQL Installation and Basic Configuration**
   - **Lab 1: Install MySQL**
     - Install MySQL server and client.
     - Start the MySQL service and ensure it starts automatically on boot.
     - Secure the installation using `mysql_secure_installation` (set root password, remove test databases, disallow remote root login).

   - **Lab 2: Basic MySQL Configuration**
     - Explore and modify MySQL configuration files (`my.cnf`).
     - Configure memory settings, buffers, and log files in MySQL.
     - Create a backup of your configuration file before making changes.

### 2. **User Management and Privileges**
   - **Lab 3: Creating and Managing MySQL Users**
     - Create a new MySQL user with restricted privileges.
     - Grant the user specific privileges such as `SELECT`, `INSERT`, `UPDATE`, and `DELETE` for a specific database.
     - Test user permissions by logging in as the new user and attempting various SQL commands.

   - **Lab 4: Managing Privileges and Roles**
     - Create and assign roles in MySQL to group permissions.
     - Grant and revoke privileges dynamically using `GRANT` and `REVOKE` statements.
     - Use `SHOW GRANTS` to view the permissions of specific users.

### 3. **Database and Table Operations**
   - **Lab 5: Creating and Managing Databases**
     - Create a new database.
     - Create and manage tables using SQL `CREATE TABLE`, `ALTER TABLE`, and `DROP TABLE` commands.
     - Define primary keys, foreign keys, and indexes.

   - **Lab 6: Basic SQL Operations**
     - Insert data into tables using `INSERT INTO`.
     - Query data using `SELECT`, filtering results with `WHERE` clauses.
     - Perform simple joins between multiple tables using `INNER JOIN`, `LEFT JOIN`, and `RIGHT JOIN`.

   - **Lab 7: Updating and Deleting Records**
     - Use `UPDATE` queries to modify existing records in a table.
     - Delete records using `DELETE FROM` and test with `ROLLBACK` and `COMMIT` to practice transaction management.

### 4. **Database Design**
   - **Lab 8: Normalization and Database Design**
     - Design a relational database with normalized tables (1NF, 2NF, 3NF).
     - Create a simple relational database with foreign key constraints and relationships between tables.
     - Normalize a database and test inserting data into the normalized schema.

   - **Lab 9: Indexes and Optimization**
     - Create and manage indexes on frequently queried columns to optimize query performance.
     - Analyze the performance of queries before and after indexing using `EXPLAIN`.

### 5. **Advanced SQL Queries**
   - **Lab 10: Advanced SQL Queries**
     - Perform complex queries using `GROUP BY`, `HAVING`, and aggregate functions (`SUM`, `COUNT`, `MAX`, `MIN`).
     - Use `UNION` and `UNION ALL` to combine results from multiple queries.
     - Explore subqueries and correlated subqueries for more advanced querying.

   - **Lab 11: Using Stored Procedures and Functions**
     - Create and execute stored procedures to automate repetitive tasks.
     - Create custom MySQL functions to return specific calculations or results.
     - Test the procedures and functions using `CALL` and `SELECT`.

### 6. **Backup and Restore**
   - **Lab 12: Backing up Databases**
     - Use `mysqldump` to create backups of databases and individual tables.
     - Create full, incremental, and binary log-based backups.
     - Automate regular backups with cron jobs and practice creating scripts to manage backups.

   - **Lab 13: Restoring Databases**
     - Restore a MySQL database from a dump file.
     - Test restoring specific tables or schemas from larger backup files.
     - Verify the integrity of the restored data by comparing it to the original.

### 7. **Database Security**
   - **Lab 14: Securing MySQL Databases**
     - Enable SSL/TLS encryption between the MySQL server and clients.
     - Create secure user accounts with limited access and test remote logins.
     - Configure firewall rules and IP restrictions to limit access to the MySQL service.

   - **Lab 15: Data Encryption**
     - Explore MySQL’s built-in encryption functions (`AES_ENCRYPT()`, `AES_DECRYPT()`).
     - Encrypt sensitive data in a table and practice decrypting it with authorized users.
     - Set up MySQL Transparent Data Encryption (TDE) for tables and logs.

### 8. **Replication and Clustering**
   - **Lab 16: Setting Up MySQL Replication**
     - Configure master-slave replication on two MySQL instances.
     - Test data replication by making changes on the master and verifying the updates on the slave.
     - Troubleshoot replication issues by examining the MySQL error log.

   - **Lab 17: Setting Up MySQL Cluster**
     - Set up a MySQL InnoDB Cluster using multiple MySQL nodes.
     - Enable automatic failover between nodes using MySQL Shell.
     - Test the cluster by simulating a node failure and ensuring high availability.

