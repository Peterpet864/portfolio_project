Flask Authentication App.
Author: Jerome Udoh and Peter Okon
Email: jubass640@gmail.com and Peterokon86@yahoo.com
Description
This Flask application is a simple web application that allows users to view articles, register, log in, create, edit, and delete articles, and manage user sessions. It uses a MySQL database to store articles and user information. The application is designed to showcase basic web development concepts using Flask, MySQL, and other related technologies.

Technologies Used
#Flask: Flask is a micro web framework for Python used to build web applications. MySQL: MySQL is an open-source relational database management system used for data storage. Flask-MySQLdb: Flask-MySQLdb is a Flask extension that simplifies MySQL database connections in Flask applications. WTForms: WTForms is a library for creating and validating web forms in Flask applications. passlib: Passlib is a library used for password hashing and verification. Python 3.x: The application is built using Python 3.x. Installation To run this Flask application on your local machine, follow these steps:

Clone the Repository: Clone this repository to your local machine using Git:
git clone <repository_url> Install Dependencies: Navigate to the project directory and install the required Python packages using pip:

pip install -r requirements.txt Configure the Database: Edit the app.py file to specify your MySQL database configuration. Modify the following lines with your MySQL credentials:

app.config['MYSQL_HOST'] = 'localhost' app.config['MYSQL_USER'] = 'your_username' app.config['MYSQL_PASSWORD'] = 'your_password' app.config['MYSQL_DB'] = 'myflaskapp' Initialize the Database: Create the necessary database tables by running the following command from the project directory:

python initialize_database.py Run the Application: Start the Flask application:

python app.py The application will be available at http://localhost:5000/ in your web browser.

Usage
Visit the home page at http://localhost:5000/ to view articles. Register an account to create and manage articles. Log in to your account to access the dashboard for article management. Create, edit, and delete articles as a logged-in user. Challenges Faced During the development of this application, the following challenges were encountered:

Database Configuration:
Configuring the MySQL database correctly, including setting up the schema and ensuring that the 'root' user had the necessary privileges.

Session Management:
Implementing user sessions and securing routes that require authentication using Flask's session management.

Password Hashing:
Properly implementing password hashing and verification using the Passlib library to enhance security.

Form Validation: Validating user input in registration and article creation forms using WTForms to prevent data inconsistencies and security vulnerabilities.

Debugging:
Debugging and troubleshooting any issues that arose during development, including SQL queries, route handlers, and template rendering.

Contributing
Contributions to this project are welcome. You can fork the repository, make your changes, and submit a pull request. Please follow best practices and maintain code quality.

License
This project is licensed under the MIT License. See the LICENSE file for details.
