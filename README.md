## Library available/login System

# Project Overview

Library available/login System is a web-based application developed using Flask and PostgreSQL. It allows users to browse books, register, and log in to the system. The project could simulate a library's online book reservation system, although the reservation functionality is not yet implemented.

# Features

- User Registration and Login
- Book Browsing (with details such as title, author, and availability)
- Basic form validation (e.g., ensuring all fields are filled and email format  is valid)
- Simple database seeding with initial book data

# Known Issues and Limitations

- All books currently have "Available: Yes." The application needs further implementation to manage the reservation and availability status.
- The email validation only checks for the presence of an "@" symbol and a domain, not the full validity of an email.
- The visual design is minimal and can be improved for a better user experience.

# Project Setup

Prerequisites:

- Python 3.6+
- PostgreSQL
- Virtual Environment (optional but recommended)
- pgAdmin for managing the PostgreSQL database

# Installation

- Clone the Repository:
git clone <repository-URL>
cd library-available/login-system

- Set Up Virtual Environment:
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

- nstall Required Packages:
pip install -r requirements.txt

- Database Configuration;
Create a PostgreSQL database named library using pgAdmin or command line.
Update the .env file with your database credentials:

DB_USERNAME=your_username
DB_PASSWORD=your_password
DB_NAME=library
DB_HOST=localhost
DB_PORT=5432

- Database Setup:

flask db upgrade


- Seed the Database:
  python seed.py


- Testing:
  python -m unittest discover tests

# Running the Application
To run the application, use the following command:

python run.py


The application will be accessible at http://127.0.0.1:5000.


# Code Comments and Explanations:

routes.py:

- Home Route: Displays the home page.
- Register Route: Handles user registration.
- Login Route: Handles user login.
- Book List Route: Displays available books.


models.py:
- User Model: Defines user attributes such as username, email, and password.
- Book Model: Defines book attributes such as title, author, and availability.

init.py:
- App Initialization: Sets up the Flask app, database, and other configurations.


# Deployment

- For deployment, you may need to set up a production WSGI server and configure your database and environment variables accordingly.


# Future Improvements
- Implement reservation functionality, allowing users to reserve and unreserve books.
- Improve email validation for stricter checks on valid email formats.
- Enhance the UI for a better user experience.
- Expand the database schema to include more detailed information about books and reservations.


# License

This project is licensed under the MIT License.












# library-available-login-system
# library-available-login-system
# library-available-login-system_project
# library-available-login-system_project
