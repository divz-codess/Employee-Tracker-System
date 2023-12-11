# Employee Tracking System using Hibernate

## Overview
Employee Tracking System is a comprehensive project that effectively manages an employee database through the use of Hibernate, an Object-Relational Mapping (ORM) tool. This project encompasses all fundamental CRUD (Create, Read, Update, Delete) operations along with advanced search functionalities on the database.

## Project Components

### 1. `hibernate.cfg.xml`
The `hibernate.cfg.xml` file serves as the configuration hub for Hibernate. It includes essential details for the Session Factory and the resource location of the Hibernate mapping file. This file encapsulates crucial database connection parameters such as connection URL, username, password, dialect, and the driver class. In this project, Oracle Driver has been employed.

### 2. `employee.hbm.xml`
The `employee.hbm.xml` file is a Hibernate mapping file responsible for defining the mapping details between Java objects and the corresponding database tables. Key elements in this file include:
- `class`: Mapping of Java class to a database table.
- `property`: Mapping of Java class properties to database columns.
- `id`: Mapping of the primary key of the table to the Java class.
- `meta`: An optional element used for creating class descriptions.
- `generator`: An `id` element employed for automatic generation of primary key values.

### 3. `Employee.java`
The `Employee.java` file represents a JavaBean class, equipped with setter and getter methods for the properties of the Employee class. This encapsulation ensures proper encapsulation and interaction with employee data.

### 4. `EmployeeDataManager.java`
The `EmployeeDataManager.java` class acts as the core component for interacting with the employee database using Hibernate queries. The primary methods include:

- **`addEmployee`**: Adds a new employee record to the database. The `save()` method in Hibernate is utilized to queue the addition, and the record is committed to the database once the transaction is completed.

- **`getById`**: Retrieves employee details based on the provided employee ID using the `get()` method in Hibernate.

- **`updateById`**: Updates employee details based on the provided employee ID using the `update()` method in Hibernate.

- **`removeById`**: Deletes an employee record based on the provided employee ID using the `delete()` method in Hibernate.

- **`HQL`**: Executes a Hibernate Query Language (HQL) query to retrieve selected employee records using `createQuery()`.

- **`getAllEmployees`**: Retrieves all employee records by invoking an HQL query using `createQuery()`.

- **`criteriaQueries`**: Utilizes Criteria to retrieve selected employee records by invoking `createQuery()`.

## Project Developer
**Divyangi Raghav**
- Course: B. Tech CSE AI/ML

Feel free to explore and contribute to this Employee Tracking System project!
