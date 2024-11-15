# Connecting Dremio to MYSQL

## Creating a DB and USER

1. Create a database (for demo we area creating test_db)

    ![alt text](images/create-databse.png)

2. Creating a table and inserting values into it with the following queries

    ```sql
    CREATE TABLE demo_table(ID VARCHAR(10));

    INSERT INTO demo_table VALUES ('1');
    ```
3. Creating a user with access from all IP addresses and assigning all privilages. The `@'%'` represents access from all IPs. For demo purpose a sample password has been set, a strong password must be used in as we are providing access from all IPs.

    ```sql
    CREATE USER test_user@'%' IDENTIFIED BY 'test123'; 

    GRANT all on test_db.* to test_user@'%';
    ```


