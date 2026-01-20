# GearGuard

GearGuard is a comprehensive Equipment Maintenance and Management System built with Flask. It helps organizations track equipment health, manage maintenance requests, schedule repairs, and generate detailed reports.

## Features

-   **Dashboard**: Real-time overview of critical equipment, open requests, and technician utilization.
-   **Equipment Management**:
    -   Track equipment details, health status, and location.
    -   Categorize equipment.
    -   Manage equipment lifecycle (assignment, maintenance, scrap).
-   **Maintenance Requests**:
    -   Create and manage corrective and preventive maintenance requests.
    -   Track request status (New, In Progress, Blocked, Ready, Repaired, Scrap).
    -   Assign technicians and teams.
    -   Schedule maintenance and set due dates.
-   **Work Centers**: Manage different work centers and their capacities.
-   **Reporting**: Generate reports for maintenance requests, equipment status, technician performance, and more.
-   **User Management**: Role-based access control (RBAC) with secure authentication.
-   **Calendar View**: Visual calendar for scheduled maintenance tasks.

## Tech Stack

-   **Backend**: Python, Flask
-   **Database**: SQLite
-   **Frontend**: HTML, CSS, JavaScript (Jinja2 Templates)

## Prerequisites

-   Python 3.8 or higher
-   pip (Python package installer)

## Setup and Installation

1.  **Clone the repository** (if applicable):
    ```bash
    git clone <repository_url>
    cd GearGuard
    ```

2.  **Create a virtual environment**:
    ```bash
    python -m venv venv
    ```

3.  **Activate the virtual environment**:
    -   **Windows (PowerShell)**:
        ```powershell
        .\venv\Scripts\Activate.ps1
        ```
    -   **Windows (CMD)**:
        ```cmd
        venv\Scripts\activate.bat
        ```
    -   **Linux/Mac**:
        ```bash
        source venv/bin/activate
        ```

4.  **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1.  **Run the application**:
    ```bash
    python app.py
    ```

2.  **Access the application**:
    Open your web browser and go to `http://localhost:5000`.

3.  **Login/Signup**:
    -   Create a new account via the Signup page.
    -   Login with your credentials.

## Project Structure

-   `app.py`: Main Flask application file containing routes and logic.
-   `database.py`: Database connection and helper functions.
-   `templates/`: HTML templates for the application.
-   `static/`: Static files (CSS, JS, images).
-   `*.db`: SQLite database files (`auth.db`, `equipment.db`, `requests.db`).

## API Endpoints (Internal)

-   `GET /`: Landing page.
-   `GET /dashboard`: Main user dashboard.
-   `GET /equipment`: List all equipment.
-   `GET /requests`: List all maintenance requests.
-   `GET /reporting`: Reporting interface.
-   `POST /create-request`: Create a new maintenance request.
-   `POST /create-equipment`: Add new equipment.

## License

[License Name]
