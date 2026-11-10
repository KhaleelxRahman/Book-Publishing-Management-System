📚 Book Publishing Company Management System

A Database Management System Project | Experiment 10

<p align="center">A Complete Relational Database Solution for Managing Book Publishing Operations

""Database" (https://img.shields.io/badge/Database-TiDB%20Cloud-00A6A6?style=for-the-badge)" (https://www.pingcap.com/tidb/)
""Backend" (https://img.shields.io/badge/Backend-Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)" (https://nodejs.org/)
""Framework" (https://img.shields.io/badge/Framework-Express.js-000000?style=for-the-badge&logo=express)" (https://expressjs.com/)
""SQL" (https://img.shields.io/badge/SQL-MySQL%20Compatible-4479A1?style=for-the-badge&logo=mysql&logoColor=white)" (https://www.mysql.com/)
""Deployment" (https://img.shields.io/badge/Deployment-Vercel-000000?style=for-the-badge&logo=vercel)" (https://vercel.com/)

</p>---

🌟 Project Overview

The Book Publishing Company Management System is a comprehensive Database Management System (DBMS) project designed to organize and manage the essential operations of a book publishing company through a structured relational database.

The system provides a centralized approach to managing publishing-related information, maintaining relationships between database entities, executing SQL queries, and retrieving meaningful business information.

The project demonstrates the practical application of relational database concepts, including:

- Database design and architecture.
- Entity Relationship (ER) modeling.
- Relational schema development.
- Functional dependencies.
- Database normalization (1NF, 2NF, and 3NF).
- SQL table creation and data manipulation.
- Constraints and relational integrity.
- Views and advanced SQL queries.
- Backend and database connectivity.
- Cloud database integration using TiDB Cloud.

The project also demonstrates the transition from a traditional local database implementation to a cloud-hosted, MySQL-compatible database architecture.

🎯 Project Objectives

1. Design a structured relational database for a book publishing company.
2. Identify entities, attributes, primary keys, and foreign keys.
3. Establish relationships and cardinalities between entities.
4. Apply normalization techniques to reduce redundancy.
5. Implement database tables using SQL.
6. Maintain data consistency through constraints and referential integrity.
7. Execute SQL queries for retrieving and analyzing publishing information.
8. Implement database views for reusable data retrieval.
9. Integrate the database with a Node.js and Express.js backend.
10. Configure cloud database connectivity using TiDB Cloud.

---

🏗️ System Architecture

The project follows a layered architecture that separates the user interface, backend application logic, and database infrastructure.

             BOOK PUBLISHING MANAGEMENT SYSTEM
                            |
                            |
                  Frontend / User Interface
                            |
                            |
                    Backend Application
                      Node.js + Express
                            |
                            |
                    Database Connection
                         mysql2
                            |
                            |
                     TiDB Cloud Serverless
                            |
                            |
                   Relational Database
                      book_publishing
                            |
             +--------------+--------------+
             |              |              |
          Tables           Views        SQL Queries
             |              |              |
             +--------------+--------------+
                            |
                  Structured Data Results

Architecture Components

Component| Technology| Responsibility
Frontend| Project UI| User interaction
Backend| Node.js| Application logic
API Framework| Express.js| API routing
Database Driver| mysql2| Database connectivity
Cloud Database| TiDB Cloud| Relational data storage
Database| book_publishing| Publishing information
Hosting| Vercel| Application deployment

---

🗄️ Database Architecture

The database is named:

"book_publishing"

The database implementation uses a MySQL-compatible relational architecture through TiDB Cloud Serverless.

Database Implementation Overview

Database Component| Implementation
Relational Tables| 6
Stored Records / Tuples| 61
Database Views| 5
Canonical SQL Queries| 19
Database Platform| TiDB Cloud
Database Compatibility| MySQL

These figures represent the recorded database implementation results.

Database Design Principles

- Primary Key constraints for unique identification.
- Foreign Key constraints for maintaining relationships.
- Appropriate data types for attributes.
- Referential integrity between related tables.
- Normalized relational structures.
- SQL views for reusable database operations.

---

🧩 Core DBMS Concepts Implemented

1. Entity Relationship Modeling

The database design uses an Entity Relationship model to represent the entities, their attributes, and the relationships between them.

2. Relational Schema

The ER model is translated into relational tables using primary keys, foreign keys, and appropriate relational constraints.

3. Database Normalization

The database design considers the following normalization stages:

Normal Form| Purpose
1NF| Eliminate repeating groups and ensure atomic values
2NF| Eliminate partial dependencies
3NF| Eliminate transitive dependencies

4. SQL Implementation

The project includes SQL operations for:

- CREATE – Creating database objects.
- INSERT – Inserting records.
- SELECT – Retrieving information.
- UPDATE – Modifying existing records.
- DELETE – Removing records.
- JOIN – Combining related tables.
- GROUP BY – Grouping records.
- ORDER BY – Sorting results.
- Aggregate Functions – Analyzing database information.
- Views – Creating reusable query structures.

---

☁️ Oracle to TiDB Cloud Migration

An important part of this project is its database migration and cloud integration.

The project began with an Oracle-based DBMS implementation and was extended to a MySQL-compatible TiDB Cloud Serverless architecture.

Migration Overview

Parameter| Implementation
Original Database| Oracle Database
Cloud Database| TiDB Cloud Serverless
Database Name| book_publishing
Backend Runtime| Node.js
Database Driver| mysql2
Connection Security| TLS
Cloud Database Port| 4000
Local Backend Port| 5000

Migration Objectives

- Establish a cloud-hosted relational database.
- Preserve the original local Oracle database.
- Maintain a separate local MySQL environment.
- Configure secure cloud connectivity.
- Connect the backend to TiDB Cloud.
- Maintain compatibility with MySQL-oriented SQL operations.

Important: The Oracle and local MySQL environments are retained independently. The TiDB Cloud implementation provides an additional cloud database environment.

---

⚙️ Backend API Architecture

The backend uses Node.js, Express.js, and the mysql2 database driver.

The recorded API endpoints include:

API Endpoint| Purpose
"/api/health"| Backend health information
"/api/dashboard"| Dashboard data
"/api/books"| Book-related information
"/api/database/integrity"| Database integrity information

Local backend testing was recorded for these endpoints.

---

📁 Project Deliverables

The repository includes the project's implementation and academic documentation.

Deliverable| Description
Database SQL Files| Database creation and SQL implementation
Backend Source Code| Server and API implementation
Database Documentation| Database design and architecture
ER Diagram| Entity Relationship representation
Project Report| Complete academic project documentation
Presentation PDF| Final presentation document
Presentation PPTX| Editable PowerPoint presentation
SQL Query Inventory| Organized SQL query reference
Final Deliverables| Consolidated project submission materials

---

🚀 Getting Started

Prerequisites

Install the following software before running the project:

- Node.js and npm
- Git
- Visual Studio Code
- TiDB Cloud account
- MySQL-compatible database client

Step 1: Clone the Repository

git clone YOUR_GITHUB_REPOSITORY_URL

cd YOUR_PROJECT_DIRECTORY

Step 2: Install Dependencies

Navigate to the backend directory and install dependencies:

npm install

Step 3: Configure Environment Variables

Create a ".env" file in the backend directory.

Example configuration:

PORT=5000

DB_HOST=your_tidb_host
DB_PORT=4000
DB_USER=your_tidb_username
DB_PASSWORD=your_tidb_password
DB_NAME=book_publishing

DB_SSL=true

Use the actual connection details provided by TiDB Cloud. Configure TLS certificate verification according to the provider's connection instructions.

Security: Never upload ".env", database passwords, private certificates, or other credentials to GitHub.

Step 4: Start the Backend

Use the development command defined in the backend's "package.json".

For example:

npm run dev

Alternatively, if a start script is configured:

npm start

Step 5: Access the Application

The local backend is configured to use port "5000" in the recorded development setup.

http://localhost:5000

The frontend should be started separately using its configured development command.

---

🔐 Security Considerations

Database credentials and application secrets must be protected.

Recommended security practices:

- Store credentials in environment variables.
- Never commit ".env" files.
- Use encrypted TLS connections.
- Validate incoming API requests.
- Use parameterized SQL queries.
- Avoid exposing database credentials in frontend code.
- Apply appropriate database access permissions.
- Keep production and development credentials separate.

---

📊 Project Significance

This project demonstrates how academic database concepts can be applied to a practical publishing management scenario.

It combines database modeling, SQL implementation, relational integrity, backend integration, and cloud database infrastructure into a single project.

The Oracle-to-TiDB extension also demonstrates the importance of database compatibility, secure connectivity, and cloud-based database architecture.

---

🎓 Academic Information

Project: Book Publishing Company Management System
Experiment: Experiment 10
Subject: Database Management Systems (DBMS)
Project Category: Academic Database Project
Institution: Lords Institute of Engineering and Technology

---

👨‍💻 Contributors

Name| Roll Number
MD Khaleel ur Rahman| 160925748042
Mohd Uzair Ali| 160925748025
Syed Mustafa| 160925749022

---

📚 Learning Outcomes

Through this project, the implementation demonstrates practical understanding of:

- Relational database design.
- ER diagrams and relational mapping.
- Database normalization.
- SQL queries and operations.
- Primary and foreign key constraints.
- Database views.
- Backend database connectivity.
- Cloud database migration.
- Secure database configuration.
- Software project documentation.

---

🔮 Future Enhancements

Potential future improvements include:

- Advanced publishing analytics.
- Role-based access control.
- Enhanced reporting and visualization.
- Automated database backups.
- Improved API security.
- Advanced search and filtering.
- Scalable cloud infrastructure.

---

📄 Project Documentation

Refer to the repository's presentation, SQL inventory, source-code documentation, and final project report for detailed implementation information.

---

⭐ Acknowledgements

This project was developed as part of the Database Management Systems academic curriculum to demonstrate the practical application of database concepts and modern database infrastructure.

If you find this project useful, consider giving the repository a ⭐ on GitHub.

---

<p align="center">BOOK PUBLISHING COMPANY MANAGEMENT SYSTEM

Structured Data. Reliable Relationships. Smarter Publishing Management.

</p>
