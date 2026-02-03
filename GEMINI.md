# Finanpy Project GEMINI.md

## Project Overview

Finanpy is a personal finance management system built with Python and Django. It provides a full-stack solution using Django Template Language and TailwindCSS for the frontend. The application allows users to manage bank accounts, categorize transactions, and view a dashboard with a summary of their financial situation.

The project is structured into the following Django apps:
- `core`: Global configurations and main URLs.
- `users`: Manages user authentication.
- `profiles`: Manages user profiles.
- `accounts`: Manages user bank accounts.
- `categories`: Manages transaction categories.
- `transactions`: Manages financial transactions.

The database used is SQLite, as configured in `core/settings.py`.

## Building and Running

To set up and run this project, follow these steps:

1.  **Set up the virtual environment and install dependencies:**
    ```bash
    python3 -m venv .venv
    source .venv/bin/activate
    pip install -r requirements.txt
    ```

2.  **Apply database migrations:**
    ```bash
    python3 manage.py migrate
    ```

3.  **Run the development server:**
    ```bash
    python3 manage.py runserver
    ```
    The application will be available at `http://127.0.0.1:8000/`.

## Development Conventions

- **Code Style**: The project follows the PEP 8 style guide for Python code. All code, including comments and documentation, should be written in English.
- **Commits**: The project uses semantic commits. For example: `feat(accounts): add feature to create bank accounts`.
- **Database**: All models should include `created_at` and `updated_at` fields.
- **Testing**: (TODO) Testing practices are not yet defined. The `tests.py` file in each app is the recommended place to add tests.