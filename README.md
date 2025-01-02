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

2. Create and activate a virtual environment:

```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

3. Install dependencies:

```bash
pip install -r requirements.txt

4. Set up the database:

Make sure PostgreSQL is running.
Create a database:
```sql
CREATE DATABASE mydatabase;

Update the database URL in alembic.ini and your SQLAlchemy configuration.

5. Run Alembic migrations:

```bash
alembic upgrade head

# goit-pythonweb-hw-06
