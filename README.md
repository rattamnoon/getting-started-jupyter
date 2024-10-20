# Data Analysis Project

This project contains a set of Jupyter notebooks for data analysis and visualization using various databases and Python libraries.

## Setup

1. Install the required Python packages:

```bash
pip install pyodbc pymssql clickhouse-driver clickhouse-connect pandas seaborn matplotlib numpy python-dotenv
pip install --upgrade pip
pip install --upgrade lz4
```

2. Create a `.env` file in the project root directory with the following content:

```bash
SERVER=your_server
DATABASE=your_database
USERNAME=your_username
PASSWORD=your_password
DSN=your_dsn
```

Replace the placeholder values with your actual database credentials.

## Notebooks

### create_engine.ipynb

- Connects to a SQL Server database using SQLAlchemy
- Performs data analysis on employee data
- Creates visualizations for marital status distribution

### init.ipynb

- Sets up connections to ClickHouse database
- Imports data from SQL Server to ClickHouse
- Performs various data analyses and visualizations on employee data

### pyodbc_mssql.ipynb

- Demonstrates connection to SQL Server using pyodbc
- Executes a simple query to fetch employee data

### pymssql_mssql.ipynb

- Demonstrates connection to SQL Server using pymssql
- Executes a simple query to fetch employee data

## Key Features

- Database connections (SQL Server and ClickHouse)
- Data import and transformation
- Data visualization using seaborn and matplotlib
- Analysis of employee demographics, including:
  - Birth month distribution
  - Marital status
  - Gender distribution
  - Employee bands
  - Top positions by number of employees

## Usage

1. Ensure all required packages are installed and the `.env` file is set up correctly.
2. Open the desired Jupyter notebook.
3. Run the cells in order to perform the analysis and generate visualizations.

## Note

Make sure you have the necessary permissions and access to the databases mentioned in the notebooks. Adjust connection strings and queries as needed for your specific environment.
