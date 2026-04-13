# 📚 Advanced SQL Notes

Personal reference notes from an Advanced SQL course using PostgreSQL and the `general_hospital` database. Covers advanced querying, schema design, database programming, and performance tooling.

---

## 🗂️ Topics

| #  | Topic                     | Key Concepts |
|----|--------------------------|-------------|
| 00 | Database Setup           | Schema overview, table relationships |
| 01 | Subqueries & CTEs        | FROM/JOIN subqueries, WITH clauses, EXISTS, ANY/ALL, Recursive CTEs |
| 02 | Window Functions         | OVER, PARTITION BY, ORDER BY, WINDOW clause, RANK, LAG, ROW_NUMBER |
| 03 | Advanced Joins           | Self Join, Cross Join, Full Join, USING, Natural Joins |
| 04 | Set Operations           | UNION, INTERSECT, EXCEPT |
| 05 | Grouping Sets            | GROUPING SETS, CUBE, ROLLUP |
| 06 | Schema Structures        | information_schema, COMMENT, Constraints, Foreign Keys |
| 07 | Transactions             | BEGIN/COMMIT/ROLLBACK, SAVEPOINT, Database Locks, UPDATE/SET |
| 08 | Table Partitioning       | Range, List, Hash Partitioning, Table Inheritance |
| 09 | Views                    | Creating/Modifying Views, Updatable Views, Materialized Views, Recursive Views |
| 10 | Useful Tools & Methods   | EXPLAIN, TRUNCATE, COPY, Arrays, JSON, Extensions |
| 11 | User-Defined Functions   | CREATE FUNCTION, PL/pgSQL, calling notations, ALTER/DROP |
| 12 | Stored Procedures        | CREATE PROCEDURE, CALL, transaction control, vs functions |
| 13 | Triggers                 | BEFORE/AFTER triggers, NEW/OLD, FOR EACH ROW, enable/disable |

---

## 📁 Repo Structure

```
advanced-sql-notes/
│
├── README.md
│
├── 00-database-setup/
│   ├── README.md
│   └── general_hospital_setup.sql
│
├── 01-subqueries-and-ctes/
│   ├── README.md
│   └── scripts/
│       ├── lesson.sql
│       └── exercises.sql
│
├── 02-window-functions/
├── 03-advanced-joins/
├── 04-set-operations/
├── 05-grouping-sets/
├── 06-schema-structures/
├── 07-transactions/
├── 08-table-partitioning/
├── 09-views/
├── 10-useful-tools-methods/
├── 11-user-defined-functions/
├── 12-stored-procedures/
└── 13-triggers/
```

---

## 🗄️ Database

All queries run against the `general_hospital` PostgreSQL schema.

Set the search path at the start of any session:

```sql
SET search_path TO general_hospital;
```

### Key Tables

- patients
- encounters
- physicians
- departments
- hospitals
- surgical_encounters
- surgical_costs
- accounts
- vitals
- order_procedures
- practices

---

## 🛠️ Setup

### 1. Install PostgreSQL
Ensure PostgreSQL version 12 or higher is installed.

### 2. Restore the Database

```bash
psql -U postgres -f 00-database-setup/general_hospital_setup.sql
```

### 3. Start Learning

- Navigate to any topic folder  
- Read the `README.md`  
- Run queries from the `scripts/` folder  

---

## 🎯 Purpose

This repo is designed to:
- Reinforce advanced SQL concepts  
- Serve as a long-term reference  
- Provide reusable query patterns for real-world data work  
