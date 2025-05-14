Travel Tracker 🌍✈️
A full-stack Node.js application that lets users track, manage, and visualize their travel destinations. Built with Express.js, PostgreSQL, and Node.js, this app provides a simple yet powerful interface for storing and retrieving travel data.

Features
Add new travel destinations with details (name, country, date, notes, etc.)

View all saved destinations in a clean list

Edit or delete destinations

Store data persistently using PostgreSQL

RESTful API design

Server-side rendering or API-based response (depending on implementation)

Technologies Used
Node.js

Express.js

PostgreSQL

pg (node-postgres)

(Optional) EJS / Pug / JSON response / Frontend framework

Installation
Clone the repository:

bash
Copy
Edit
git clone (https://github.com/NasrKashtu/Travel-Tracker/tree/main)
cd travel-tracker
Install dependencies:

bash
Copy
Edit
npm install
Set up PostgreSQL:

Create a new database:

sql
Copy
Edit
CREATE DATABASE travel_tracker;
Create a destinations table:

sql
Copy
Edit
CREATE TABLE destinations (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100),
  country VARCHAR(100),
  visit_date DATE,
  notes TEXT
);
Configure the database connection in .env:

ini
Copy
Edit
DB_HOST=localhost
DB_USER=your_postgres_username
DB_PASSWORD=your_postgres_password
DB_NAME=travel_tracker
DB_PORT=5432
Run the app:

bash
Copy
Edit
node index.js
API Routes (Example)
Method	Route	Description
GET	/destinations	Get all destinations
POST	/add	Add a new destination
PUT	/edit/:id	Edit a destination
DELETE	/delete/:id	Delete a destination

Screenshots (Optional)
Add screenshots of the list view, form to add destinations, etc.

Future Improvements
Add user authentication (e.g., for personal travel tracking)

Map integration (e.g., display destinations on a world map)

Photo upload for each destination

Frontend UI using React or Vue

Export travel list as PDF or CSV

License
MIT License

