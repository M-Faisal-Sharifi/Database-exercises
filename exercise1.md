# Review Questions

## 1.1 Define the following terms: data, database, DBMS, database system, database catalog, program-data independence, user view, DBA, end user, canned transaction, deductive database system, persistent object, meta-data, and transaction-processing application.

**Answer:**

Data: Raw facts and figures.
Database: A collection of related data.
DBMS: Software that manages databases.
Database system: Database and DBMS together.
Database catalog: Stores metadata about the database.
Program-data independence: Programs are not affected by changes in data structure.
User view: The part of database seen by a user.
DBA: Person who manages the database system.
End user: Person who uses the database.
Canned transaction: Predefined database operation.
Deductive database system: Database that can infer new data using rules.
Persistent object: Data stored permanently in database.
Meta-data: Data about data.
Transaction-processing application: System that handles transactions like banking.

---

## 1.2 What four main types of actions involve databases? Briefly discuss each.

**Answer:**

Retrieval: Getting data from database.
Insertion: Adding new data.
Deletion: Removing data.
Modification: Updating existing data.

---

## 1.3 Discuss the main characteristics of the database approach and how it differs from traditional file systems.

**Answer:**

Database approach reduces redundancy, supports data sharing, provides security, ensures data independence, and supports multiple users.
Traditional file systems have high redundancy, inconsistency, poor security, and difficult data access.

---

## 1.4 What are the responsibilities of the DBA and the database designers?

**Answer:**

DBA: Security, backup, recovery, user management, performance control.
Database designers: Design tables, relationships, and database structure.

---

## 1.5 What are the different types of database end users? Discuss the main activities of each.

**Answer:**

Naive users: Use predefined applications.
Casual users: Access database occasionally.
Sophisticated users: Write SQL queries.
Stand-alone users: Use personal databases.

---

## 1.6 Discuss the capabilities that should be provided by a DBMS.

**Answer:**

Data storage and retrieval, security, backup and recovery, concurrency control, integrity constraints, query processing, multiple user access.

---

## 1.7 Discuss the differences between database systems and information retrieval systems.

**Answer:**

Database systems manage structured data and use SQL queries.
Information retrieval systems manage unstructured data and use keyword search.

---

# Exercises


## 1.8 Identify some informal queries and update operations that you would expect to apply to the database shown in Figure 1.2.

**Answer:**

Informal queries:

* List all employees
* Find department of employee
* List all projects
* Find employees in a project
* Show department manager

Update operations:

* Insert new employee
* Update salary
* Delete employee
* Add project
* Assign employee to project

---

## 1.9 What is the difference between controlled and uncontrolled redundancy? Illustrate with examples.

**Answer:**

Controlled redundancy is managed duplication of data to avoid inconsistency.
Example: Central employee database.

Uncontrolled redundancy is unmanaged duplication causing inconsistency.
Example: Same employee data in multiple files.

---

## 1.10 Specify all the relationships among the records of the database shown in Figure 1.2.

**Answer:**

Employee works in Department.
Department manages Employees.
Employee works on Project.
Project belongs to Department.
Department has Manager.
Employee has Supervisor.

---

## 1.11 Give some additional views that may be needed by other user groups for the database shown in Figure 1.2.

**Answer:**

HR view, Manager view, Finance view, Admin view, Employee view.

---

## 1.12 Cite some examples of integrity constraints that you think can apply to the database shown in Figure 1.2.

**Answer:**

Employee ID must be unique.
Department must exist.
Salary must be positive.
Project must belong to department.
Manager must be employee.

---

## 1.13 Give examples of systems in which it may make sense to use traditional file processing instead of a database approach.

**Answer:**

Small personal system, simple student records, embedded systems, temporary data storage, small business system.

---

## 1.14 Consider Figure 1.2.

### (a) If the name of the CS department changes to CSSE, identify the columns to update.

**Answer:**

Department name column, course prefix in COURSE table, SECTION table, PREREQUISITE table.

### (b) Can you restructure the columns so only one column needs update?

**Answer:**

Yes. Create separate DepartmentID and DepartmentName columns so only DepartmentName needs updating.
