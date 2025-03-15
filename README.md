
The Airline Booking System is a Flask-based API that enables users to:

Search flights
Book tickets
Manage reservations
Track flight statuses
Leave reviews for flights
This system is designed to simulate a real-world airline booking experience while utilizing RESTful API principles.

 How the Project Functions:
1️⃣ User Authentication
Users must register with a valid email and password.
Upon login, an access token is generated to authenticate API requests.
2️⃣ Flight Management
The system provides an API to retrieve flight details.
Admins can add, update, and delete flights.
Users can search flights based on departure, destination, and date.
3️⃣ Booking System
Users can book flights by selecting an available option.
Booking details include:
Flight Number
Passenger Information
Seat Class
Contact Details
Users can view, update, or cancel their bookings.
4️⃣ Flight Status Updates
Admins can update flight status (On Time, Delayed, Canceled).
Users can check flight statuses via API.
5️⃣ Reviews & Ratings
Users can submit, update, and delete reviews for their flights.
Reviews include a rating (1-5 stars) and comments.

API Endpoints:
Method	Endpoint	Description
POST	/register	Register a new user
POST	/login	Login & get authentication token
GET	/flights	Retrieve all available flights
GET	/flights/{id}	Retrieve specific flight details
POST	/bookings	Book a flight
GET	/bookings/{id}	Retrieve booking details
PUT	/flights/{flight_id}/status	Update flight status
DELETE	/bookings/{id}	Cancel a booking

 Technologies Used
Python (Flask) – Backend API
MongoDB – Database for storing user & flight data
Postman – API Testing & Debugging
JWT (JSON Web Tokens) – Secure User Authentication


How to Run the Project:
1️⃣ Clone the repository

bash
Copy code
git clone https://github.com/Csaf111/Airline_Booking_System.git
2️⃣ Navigate to the project folder

bash
Copy code
cd Airline_Booking_System
3️⃣ Install required dependencies

bash
Copy code
pip install -r requirements.txt
4️⃣ Run the Flask application

bash
Copy code
python app.py
5️⃣ Test the API using Postman or Curl
