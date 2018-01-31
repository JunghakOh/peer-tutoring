# UMass Peer Tutoring

### What is UMass Peer Tutoring?
---

UMass Peer Tutoring was developed as a proof-of-concept application that allows UMass students to search for peer tutors
based on the departments (or concentrations) in a simple, fast, and reliable way.


# Setup and Installation

First, install python virtual environment with `virtualenv -p python3 venv` and
activate with the virtual environment with `source venv/bin/activate` and download
dependencies with `pip install -r requirements.txt`

Make code migrations:

		cd peer-tutoring
		python manage.py makemigrations
		python manage.py migrate

Create database on localhost

		psql -d postgres
		CREATE DATABASE peer_tutoring WITH OWNER postgres;
		\q

You can take a look at the postgres dump `peer_tutoring.sql`

To run the application

		cd peer-tutoring
		python manage.py runserver
