# My SQL DAC Project

## Overview
This project is designed to manage SQL Server database schemas using the Data-tier Application Framework (DAC). It includes scripts for defining tables, views, and stored procedures, as well as a post-deployment script for additional configuration.

## Project Structure
```
my-sql-dac-project
├── src
│   ├── schemas
│   │   └── dbo
│   │       ├── Tables
│   │       ├── Views
│   │       └── StoredProcedures
│   └── scripts
│       └── post-deployment.sql
├── dacpac
│   └── my-sql-dac-project.sqlproj
├── .github
│   └── workflows
│       └── deploy.yml
└── README.md
```

## Setup Instructions
1. Clone the repository to your local machine.
2. Open the project in your preferred SQL development environment.
3. Review the SQL scripts located in the `src/schemas/dbo` directory to understand the database structure.

## Deployment
To deploy the DACPAC, use the GitHub Actions workflow defined in `.github/workflows/deploy.yml`. This workflow will automate the build and deployment process to your target SQL Server.

## Post-Deployment
The `src/scripts/post-deployment.sql` file contains SQL commands that will be executed after the DACPAC deployment. This can include tasks such as data seeding or configuration adjustments.

## Contributing
Feel free to submit issues or pull requests to improve the project.