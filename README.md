USER MANAGEMENT REST API WITH FLASK

This includes a work sample of a RESTful API with Flask to work with user information in-memory. It also offers basic CRUD functions and the clients can create, retrieve, update, and delete user records via well-defined APIs. The validity of data and proper HTTP responses are performed by the API, hence robustness and usability. The application illustrates key principles of REST API development, such as the route processing and working with JSON data and a memory based data management.

Interacting with the API Using curl

Add a New User
To create a new user, send a POST request with user data:

curl -X POST -H "Content-Type: application/json" -d '{"name":"John Doe","email":"john@example.com"}' http://127.0.0.1:5000/users

Get All Users

curl http://127.0.0.1:5000/users

Get a Specific User
Replace <user_id> with the actual user ID:

curl http://127.0.0.1:5000/users/<user_id>

Update a User

curl -X PUT -H "Content-Type: application/json" -d '{"name":"Jane Doe","email":"jane@example.com"}' http://127.0.0.1:5000/users/<user_id>

Delete a user by ID:

curl -X DELETE http://127.0.0.1:5000/users/<user_id>
