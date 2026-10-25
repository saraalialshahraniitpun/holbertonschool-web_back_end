# Python - Object-Relational Mapping & RESTful APIs

This repository contains projects developed as part of the Software Engineering curriculum at **Holberton School / Tuwaiq Academy**. It covers connecting Python with MySQL databases using direct drivers (`MySQLdb`), abstracting storage with Object-Relational Mappers (`SQLAlchemy`), and building/securing web services and RESTful APIs using `http.server`, `Flask`, `requests`, Basic Authentication, and JSON Web Tokens (`JWT`).

---

## 🛠️ Technologies & Requirements
- **Language:** Python (version 3.8.5+)
- **Database:** MySQL 8.0
- **Libraries & Modules:**
  - `MySQLdb` (version 2.0.x)
  - `SQLAlchemy` (version 1.4.x)
  - `Flask`
  - `requests`
  - `Flask-HTTPAuth`, `Flask-JWT-Extended`, `Werkzeug`
- **Environment:** Ubuntu 20.04 LTS / macOS with Homebrew development tools.
- **Coding Style:** `pycodestyle` (version 2.7.*)

---

## 📂 Project Structure & Tasks

### 1. Python - Object-Relational Mapping (`python-object_relational_mapping`)
* **0-select_states.py**: Lists all states from the database.
* **1-filter_states.py**: Lists states starting with 'N'.
* **2-my_filter_states.py**: Displays states matching a user argument using exact comparison.
* **3-my_safe_filter_states.py**: Safe implementation protected against SQL Injection.
* **4-cities_by_state.py**: Lists all cities with their corresponding states using `JOIN`.
* **5-filter_cities.py**: Lists all cities of a specific state safely.
* **model_state.py**: Defines the `State` class mapped to the `states` table using SQLAlchemy.
* **7 to 13-model_state_*.py**: CRUD operations using SQLAlchemy ORM (fetching, filtering, inserting, updating, and deleting).
* **model_city.py & 14-model_city_fetch_by_state.py**: Defines the `City` class and fetches cities grouped by state.

### 2. RESTful API (`restful-api`)
* **task_02_requests.py**: Consumes data from JSONPlaceholder API and exports it to a CSV file.
* **task_03_http_server.py**: Implements a lightweight HTTP server using `http.server`.
* **task_04_flask.py**: Builds a RESTful API with Flask supporting GET and POST requests.
* **task_05_basic_security.py**: Secures API routes using Basic Authentication and JWT with role-based access control.

---

## 🚀 Usage & Execution
All Python scripts are executable and follow PEP 8 guidelines. Make sure to grant execution permissions before running them:

```bash
chmod +x <script_name>.py
./<script_name>.py <mysql_username> <mysql_password> <database_name> [additional_args]
