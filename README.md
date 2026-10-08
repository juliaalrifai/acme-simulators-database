# ACME Simulators | Database Design & SQL Analysis

## Project Overview

ACME Simulators is a database design project focused on supporting the operations of a company that develops customized driving simulators. Each customer project combines a vehicle model, simulator platform, and configuration-specific requirements.

Working collaboratively in a four-person team, we designed and implemented a relational database to organize customer projects, simulator configurations, technical documentation, approval workflows, and testing results.

The project involved translating business requirements into a structured data model, defining relationships and constraints, populating the database with sample records, and developing 20 SQL queries to support operational and reporting needs.

## Database Schema

The implemented database consists of 14 interconnected tables covering product and platform configurations, customer projects, document versioning, approval processes, change tracking, and testing.

![ACME Simulators Database Schema](acme_erd_clean.png)

*Database schema diagram based on the Phase 2 SQL implementation.*

## Tools & Skills

- SQL (MySQL)
- Relational Database Design
- Entity-Relationship Modeling
- Data Modeling and Normalization
- Primary and Foreign Keys
- SQL Joins, Aggregations, and Subqueries
- Business Requirements Analysis

## SQL Implementation

The project includes database table creation, integrity constraints, sample data, and 20 SQL queries.

[View SQL Implementation](acme_database.sql)

## Key SQL Applications & Business Value

### 1. Configuration-Specific Documentation

Developed a SQL query to retrieve the relevant instruction rows for a particular simulator release, including unconditional instructions and those matching selected configuration conditions.

**Business value:** Supports the generation of configuration-specific documentation without maintaining a separate manual for every simulator variation.

### 2. Document Version Control

Used a correlated subquery to identify the latest approved version of each document, based on its version number and approval status.

**Business value:** Helps teams identify the appropriate approved documentation and reduces reliance on manual version tracking.

### 3. Quality Assurance & Testing

Designed database structures to record test executions and associate testing outcomes with project configurations and document versions.

**Business value:** Supports traceability and provides a foundation for monitoring testing results and identifying quality issues.

## Key Takeaways

- Translated operational requirements into a relational database design.
- Applied normalization and integrity constraints to organize interconnected business data.
- Developed SQL queries to support documentation retrieval and version management.
- Connected technical database design decisions to operational needs such as consistency, traceability, and process efficiency.

**Project context:** Developed collaboratively as part of a four-person team in McGill University's Master of Management in Analytics program, with contributions across business requirements analysis, database design, SQL implementation, and query development.
