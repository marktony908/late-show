# late-show

Late Show API
Overview
The Late Show API is a Flask-based RESTful API designed to manage episodes, guests, and their appearances on a fictional late-night show. This API allows users to perform various operations, including retrieving data about episodes and guests, as well as creating new appearances.

Features
Retrieve a list of all episodes
Get details of specific episodes by ID
Retrieve a list of all guests
Create new appearances linked to episodes and guests
Technologies Used
Python 3.x
Flask
Flask-SQLAlchemy
Flask-Migrate
SQLite
Getting Started
Prerequisites
Python 3.x
pip (Python package installer)
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/marktony/late-show.git
cd late-show
(Optional) Set up a virtual environment using pipenv:

bash
Copy code
pipenv install
pipenv shell
Install required packages:

bash
Copy code
pip install Flask Flask-SQLAlchemy Flask-Migrate
Initialize the database:

bash
Copy code
flask db init
flask db migrate
flask db upgrade
Seed the database (if applicable):

bash
Copy code
python seed.py
Running the Application
Start the Flask application:

bash
Copy code
python app.py
The server will run at http://127.0.0.1:5000/.

API Endpoints
GET /episodes: Retrieve a list of all episodes.
GET /episodes/<id>: Retrieve details of a specific episode by its ID.
GET /guests: Retrieve a list of all guests.
POST /appearances: Create a new appearance.
Request Body for POST /appearances:

json
Copy code
{
  "rating": 5,
  "episode_id": 1,
  "guest_id": 2
}
Testing the API
You can test the API using tools like Postman or curl.

Troubleshooting
Ensure the Flask server is running before making requests.
Verify the endpoints for correctness.
Check the console output for any errors or logs during operation.
Author
Created by marktony.

License
This project is licensed under the MIT License. See the LICENSE file for more details.

