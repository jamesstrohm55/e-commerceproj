# e-commerceproj
E-Commerce API 

This project implements a fully functional e-commerce API using Flask, Flask-SQLAlchemy, Flask-Marshmallow, and MySQL. The API manages Users, Orders, and Products with proper relationships, including One-to-Many and Many-to-Many associations. The project is designed to demonstrate database modeling, API development, data serialization, and RESTful CRUD endpoints.

Features

User Management: CRUD operations for users.

Product Management: CRUD operations for products.

Order Management: Create and manage orders with associated products.

Relationships:

One User → Many Orders (One-to-Many)

Many Orders ↔ Many Products (Many-to-Many)

Input validation and data serialization using Marshmallow.

MySQL as the database backend.

Technologies Used

Python

Flask

Flask-SQLAlchemy

Flask-Marshmallow

MySQL

Marshmallow-SQLAlchemy

Installation

Prerequisites

Python 3.7 or higher

MySQL server

MySQL Workbench (optional for database management)

Steps

Clone the repository:

git clone <repository_url>
cd <repository_directory>

Create and activate a virtual environment:

python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

Install dependencies:

pip install Flask Flask-SQLAlchemy Flask-Marshmallow marshmallow-sqlalchemy mysql-connector-python

Set up the MySQL database:

Open MySQL Workbench.

Create a new database:

CREATE DATABASE ecommerce_api;

Update the database configuration in app.py:

app.config['SQLALCHEMY_DATABASE_URI'] = 'mysql+mysqlconnector://root:<YOUR PASSWORD>@localhost/ecommerce_api'

Initialize the database:

python app.py

This will create the required tables in the database.

Run the application:

python app.py

Access the API at http://127.0.0.1:5000.

API Endpoints

User Endpoints



