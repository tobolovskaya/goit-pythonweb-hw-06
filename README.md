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
```

2. Create and activate a virtual environment:

  ```bash
  python -m venv venv
  source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

3. Install dependencies:

  ```bash
  pip install -r requirements.txt
```

4. Set up the database:

Make sure PostgreSQL is running.
Create a database:
```sql
CREATE DATABASE mydatabase;
```

Update the database URL in alembic.ini and your SQLAlchemy configuration.

5. Run Alembic migrations:

```bash
alembic upgrade head
```

## Usage
# CLI Commands
General Format
```bash
python main.py -a <action> -m <model> [additional options]
```

# Examples
1. Create a teacher:

```bash
python main.py -a create -m Teacher -n "Boris Jonson"
```

2. List all teachers:

```bash
python main.py -a list -m Teacher
```

3. Update a teacher:

```bash
python main.py -a update -m Teacher --id 1 -n "Andry Bezos"
```

4. Remove a teacher:

```bash
python main.py -a remove -m Teacher --id 1
```

# Additional Notes
The database connection URL is configured in the alembic.ini file and should match your PostgreSQL setup.
For any errors or issues, check the logs or database configuration.

# Contributing
Feel free to fork this repository and make contributions via pull requests.

# License
This project is licensed under the MIT License. See the LICENSE file for details.

```vbnet

This `README.md` provides clear instructions on how to set up, use, and extend the CLI tool. Let me know if you need modifications!
```

# goit-pythonweb-hw-06
