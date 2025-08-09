# Multi-Database File Ingestion Scripts

This repository contains Python scripts to automatically ingest CSV, Excel, and JSON files into different databases:
- **SQLite**
- **MySQL**
- **PostgreSQL**

Each script:
- Creates the database (if it does not exist)
- Reads all supported files from a `data/` directory
- Cleans column names to avoid database compatibility issues
- Loads data into database tables using **SQLAlchemy**
- Logs the process into a `logs/` directory

multi-db-file-ingestion/
│
├── SQL_ingestion.py # Script for SQLite ingestion
├── MySQL_ingestion.py # Script for MySQL ingestion
├── PostgreSQL_ingestion.py # Script for PostgreSQL ingestion
│
├── data/ # Place your CSV, Excel, JSON files here
│ ├── file1.csv
│ ├── file2.xlsx
│ └── file3.json
│
├── logs/ # Ingestion logs are stored here
│ └── mysql_ingestion.log
│
└── README.md # Project documentation
