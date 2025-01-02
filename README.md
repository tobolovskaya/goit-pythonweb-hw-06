# Database CRUD CLI Application

This project is a command-line interface (CLI) tool for performing CRUD (Create, Read, Update, Delete) operations on a PostgreSQL database using SQLAlchemy and Alembic.

## Features

- Perform CRUD operations on database models:
  - `Teacher`
  - `Group`
  - `Student`
  - `Subject`
  - `Grade`
- Uses `argparse` for parsing CLI commands.
- Supports creating, listing, updating, and removing records from the database.
- Easily extendable for additional models or operations.

---

## Requirements

- Python 3.9 or higher
- PostgreSQL
- Required Python libraries:
  - `SQLAlchemy`
  - `psycopg2-binary`
  - `argparse`

---

## Installation

1. Clone this repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>

Create and activate a virtual environment:

bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

# goit-pythonweb-hw-06
