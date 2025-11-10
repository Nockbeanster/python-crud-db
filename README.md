DEMO: https://youtu.be/9nCvY5F30Gs?si=AoOsp-LsRjBSQtmw

This project implements a PostgreSQL database and uses python to perform specific CRUD (Create, Read, Update, Delete) operations.

Requirements: 
 * Python 3.11.9
 * PostgreSQL installed and running
 * Student Table created and INSERTED DATA

PostgreSQL Commands:

    CREATE TABLE students (
        student_id SERIAL PRIMARY KEY,
        first_name TEXT NOT NULL,
        last_name TEXT NOT NULL,
        email TEXT NOT NULL UNIQUE,
        enrollment_date DATE
    ); 

    INSERT INTO students (first_name, last_name, email, enrollment_date) VALUES
    ('John', 'Doe', 'john.doe@example.com', '2023-09-01'),
    ('Jane', 'Smith', 'jane.smith@example.com', '2023-09-01'),
    ('Jim', 'Beam', 'jim.beam@example.com', '2023-09-02');


    SELECT * FROM students;

Setup:
 * Clone from Repo
 * Initalize DB with commands above
 * When DB is running
 * Install requirements.txt via
	pip install -r requirements.txt
	(While being in the same directory)
 * Run the dbms_app.ipynb
