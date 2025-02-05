# 📊 CSEN604 - Database Optimization Project (2022)

## 📌 Overview
This project is part of the CSEN604 - Databases II course, focused on optimizing SQL queries for performance tuning in PostgreSQL. The tasks include:
- Analyzing execution plans of provided queries.
- Creating and optimizing database schemas.
- Implementing indexing strategies.
- Writing optimized SQL queries and evaluating their performance.

## 📂 Repository Structure
```
CSEN604-Database-Optimization-Project/
│── 📂 schemas/                   # Database schemas and diagrams
│   ├── Schema-1.png
│   ├── Schema-2.png
│   ├── Schema-4.png
│── 📂 scripts/                    # SQL setup scripts
│   ├── script.sh
│── 📂 queries/                    # SQL queries (original and optimized)
│   ├── original-queries.txt
│   ├── new-queries.txt
│── 📂 docs/                       # Documentation and reports
│   ├── Report.pdf                #Final Report and Documentation of the project
│── 📜 README.md                    # Project introduction and setup guide
```

## 🚀 Getting Started
### 1️⃣ Setting Up the Database
Run the following command to create the databases and tables:
```sh
psql -U <your_username> -f scripts/script.sh
```

### 2️⃣ Running the Queries
Run the provided SQL queries:
```sh
psql -U <your_username> -d <database_name> -f queries/original-queries.txt
```
Run the optimized queries:
```sh
psql -U <your_username> -d <database_name> -f queries/new-queries.txt
```

### 3️⃣ Running Performance Analysis
The report (`Report.pdf`) includes:
- **Screencapture of output from PostgreSQL analyze for each query.**
- **Details of any special configuration/parameter adjustments made in PostgreSQL** to optimize execution plans. This includes traces from PostgreSQL shell or pgAdmin.
- **Discussion of optimized queries** explaining performance improvements and recommended indices.

## 📈 Performance Optimization Strategies
- **Using EXPLAIN ANALYZE** to inspect query execution plans.
- **Indexing Strategies:**
  - **B+ Tree Indexing** for efficient range queries.
  - **Hash Indexing** for faster exact-value lookups.
  - **BRIN Indexing** for large datasets with range-based queries.
  - **Mixed Indexing** to optimize performance dynamically.
- **Optimized Queries** were written to minimize execution costs.

## 🔧 Dependencies
- **PostgreSQL 13 or 14**
- **pgAdmin** (optional GUI for PostgreSQL)

---

### ⭐ Feel free to ⭐ star the repository if you find it useful!

