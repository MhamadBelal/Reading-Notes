# Introduction to Databases and ERDs

## why this topic matters?

Understanding databases and ERDs (Entity-Relationship Diagrams) is essential for efficient data management, scalable application development, and data integrity. Databases serve as central repositories for organizing and retrieving data, ensuring accuracy and consistency. ERDs help visualize data relationships, aiding in proper database design. This knowledge enables effective data storage, retrieval, and manipulation, facilitates scalability and performance optimization, and ensures data security. Familiarity with databases and ERDs is crucial for building robust, scalable, and secure software applications that rely on well-structured data.

---

## Answering the questions

### Data Models (Review the DB Schema)

1. Database Schema Questions

    * What is a Schema?

        A database schema is a logical container or structure that organizes and defines database objects. It provides a way to group related objects, separate them from others, and facilitate organization, access control, and portability.

    * Why do we use them?

        Database schemas are used to organize and categorize database objects, reduce naming conflicts, provide access control to specific objects, and enable portability by offering self-contained units of related objects.

    * What do they look like?

        Database schemas are represented by named containers or namespaces in a database management system. The specific syntax and conventions for defining and working with schemas may vary across database systems.

2. What are the different types of Database Keys?

    Primary Key, Foreign Key, Composite Key/

    * What is a Primary Key?

        It uniquely identifies each record in a table and ensures data integrity.

    * What is a Foreign Key?

        It establishes relationships between tables by referencing the primary key of another table and maintains referential integrity.

    * What is a Composite Key?

        It consists of multiple columns that together uniquely identify a record in a table.

    * How are they different? When do you use 1 over the others?

        Primary keys are used to uniquely identify records in a table, foreign keys establish relationships between tables, and composite keys are used when a combination of columns is required for uniqueness. The choice of which key to use depends on the specific database design, data relationships, and normalization principles. Primary keys are fundamental, foreign keys maintain relationships, and composite keys are used when a combination of columns is necessary for uniqueness.


### DBMS

1. What are Relationships in a relational database?

    Relationships in a relational database represent connections between tables based on shared data values. They define how data in one table relates to data in another table.

    * What is a 1:1 relationship?

        A 1:1 (one-to-one) relationship occurs when each record in one table is associated with exactly one record in another table, and vice versa. It is used when the related data is conceptually distinct but still tightly connected.

    * What is a Many:Many relationship?

        A Many:Many (many-to-many) relationship occurs when multiple records in one table are associated with multiple records in another table. A junction table is used to represent this relationship, which allows for the mapping of combinations between records in both tables.

    * How about a 1: Many or a Many:1?

        A 1:Many (one-to-many) relationship occurs when a record in one table is associated with multiple records in another table, but each record in the second table is associated with only one record in the first table. It is commonly used to represent hierarchical or parent-child relationships.

        A Many:1 (many-to-one) relationship is the reverse of a 1:Many relationship. It occurs when multiple records in one table are associated with a single record in another table. It is often used to represent the reverse side of a 1:Many relationship.

---

## Things I want to know more about

1. What are some advanced relationship types in relational databases beyond the basic ones? 
2. What are the different integrity constraints that can be applied to relationships in a database?
3. How does relationship cardinality, such as one-to-one, one-to-many, and many-to-many, impact database design and data retrieval?
