# Chapter 2 

---

## Review Questions

### 2.1. Define the following terms:

data model, database schema, database state, internal schema, conceptual schema, external schema, data independence, DDL, DML, SDL, VDL, query language, host language, data sublanguage, database utility, catalog, client/server architecture, three-tier architecture, and n-tier architecture.

**Answer:**

**Data model:**
A set of concepts used to describe the structure of a database.

**Database schema:**
The design or structure of the database.

**Database state:**
The actual data stored at a specific time.

**Internal schema:**
Describes physical storage of data.

**Conceptual schema:**
Describes logical structure of the database.

**External schema:**
User-specific view of the database.

**Data independence:**
Ability to change one schema level without affecting others.

**DDL:**
Language used to define schemas.

**DML:**
Language used to manipulate data.

**SDL:**
Language used for physical storage definition.

**VDL:**
Language used to define views.

**Query language:**
Used to retrieve data (e.g., SQL).

**Host language:**
General-purpose programming language.

**Data sublanguage:**
Database language embedded in host language.

**Database utility:**
Tool for maintenance tasks.

**Catalog:**
Metadata storage of the database.

**Client/server architecture:**
Clients request services from a server.

**Three-tier architecture:**
Presentation, application, and database layers.

**n-tier architecture:**
Multiple layered architecture.

---

### 2.2. Discuss the main categories of data models. What are the basic differences among the relational model, the object model, and the XML model?

**Answer:**

Categories:

* Conceptual
* Logical
* Physical

Relational model: uses tables
Object model: uses objects and classes
XML model: uses hierarchical structure

---

### 2.3. What is the difference between a database schema and a database state?

**Answer:**

Schema: structure of the database
State: actual data at a given time

---

### 2.4. Describe the three-schema architecture. Why do we need mappings among schema levels? How do different schema definition languages support this architecture?

**Answer:**

Three levels:

* External
* Conceptual
* Internal

Mappings:

* Connect levels
* Provide data independence

Languages:

* DDL → conceptual
* SDL → internal
* VDL → external

---

### 2.5. What is the difference between logical data independence and physical data independence? Which one is harder to achieve? Why?

**Answer:**

Logical: change conceptual schema without affecting users
Physical: change storage without affecting conceptual schema

Logical is harder because it affects applications.

---

### 2.6. What is the difference between procedural and nonprocedural DMLs?

**Answer:**

Procedural: specifies how
Nonprocedural: specifies what

---

### 2.7. Discuss the different types of user-friendly interfaces and the types of users who typically use each.

**Answer:**

Menu-based → casual users
Forms → naive users
GUI → general users
Natural language → beginners
Parametric → repetitive users

---

### 2.8. With what other computer system software does a DBMS interact?

**Answer:**

* Operating system
* File system
* Programming languages
* Network software

---

### 2.9. What is the difference between the two-tier and three-tier client/server architectures?

**Answer:**

Two-tier: client connects directly to database
Three-tier: client → application server → database

---

### 2.10. Discuss some types of database utilities and tools and their functions.

**Answer:**

* Backup and recovery
* Monitoring
* Performance tuning
* Data loading

---

### 2.11. What is the additional functionality incorporated in n-tier architecture (n > 3)?

**Answer:**

Provides scalability, flexibility, and better security.

---

# Exercises

---

### 2.12. Think of different users for the database shown in Figure 1.2. What types of applications would each user need? To which user category would each belong, and what type of interface would each need?

**Answer:**

Students → view results → casual users → GUI/forms
Teachers → update marks → parametric users → forms
Admin → manage system → DBA → command interface

---

### 2.13. Choose a database application with which you are familiar. Design a schema and show a sample database for that application. What types of additional information and constraints would you like to represent in the schema? Think of several users and design a view for each.

**Answer:**

Example: Student System

Schema:

* STUDENT(ID, Name, Age)
* COURSE(CID, Title)
* ENROLL(ID, CID)

Sample:

* (1, Ali, 20)
* (101, DBMS)

Constraints:

* ID unique
* Age > 0

Views:

* Student view → limited data
* Admin view → full data

---

### 2.14. If you were designing a Web-based system to make airline reservations and sell airline tickets, which DBMS architecture would you choose? Why?

**Answer:**

Three-tier architecture

Reason:

* Secure
* Scalable
* Efficient

Others are less scalable and less secure.

---

### 2.15. Identify the column or group of columns in the tables that must be unique across all rows.

**Answer:**

* STUDENT → Student_number
* COURSE → CID
* ENROLL → (ID, CID)

These must be unique to avoid duplication.

