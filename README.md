NoSQL Social Network API
This repository contains the code for a NoSQL-based Social Network API. It serves as the backend for a social networking application, providing various functionalities for users, posts, and reactions. This project is part of the homework assignment for Module 18 in the UCF Bootcamp curriculum.

Table of Contents
Description
Technologies Used
Installation
Usage
API Endpoints
Contributing
License
Description
The NoSQL Social Network API is designed to handle the backend operations of a social networking application. It utilizes a NoSQL database (MongoDB) for data storage and retrieval. The API provides various endpoints to perform CRUD (Create, Read, Update, Delete) operations on users, posts, and reactions.

Key features of the NoSQL Social Network API include:

User management: Create new users, retrieve user profiles, update user information, and delete user accounts.
Post management: Create new posts, retrieve posts, update post content, and delete posts.
Reaction management: Add reactions (like, love, laugh, etc.) to posts and manage them.
Friendship management: Establish connections between users by sending and accepting friend requests.
This API is developed using Node.js and Express.js framework, which enables efficient routing and handling of HTTP requests. Mongoose library is used to interact with the MongoDB database.

Technologies Used
The following technologies and libraries are used in this project:

Node.js
Express.js
MongoDB
Mongoose
Installation
To install and run the NoSQL Social Network API locally, follow these steps:

Clone this repository to your local machine.
Navigate to the root directory of the project.
Install the dependencies by running the following command:
Copy code
npm install
Make sure you have MongoDB installed and running on your local machine.
Create a .env file in the root directory and provide the necessary environment variables, such as database connection details and JWT secret key.
Start the application by running the following command:
sql
Copy code
npm start
The API will be accessible at http://localhost:3001.
Usage
The NoSQL Social Network API provides a set of endpoints that can be accessed using various HTTP methods (GET, POST, PUT, DELETE) to perform different operations. Detailed information about the available endpoints and their usage can be found in the API Endpoints section below.

To interact with the API, you can use tools like cURL, Postman, or any other HTTP client.

API Endpoints
The NoSQL Social Network API exposes the following endpoints:

GET /api/users: Retrieve all users

GET /api/users/:userId: Retrieve a specific user by ID

POST /api/users: Create a new user

PUT /api/users/:userId: Update user information

DELETE /api/users/:userId: Delete a user

GET /api/posts: Retrieve all posts

GET /api/posts/:postId: Retrieve a specific post by ID

POST /api/posts: Create a new post

PUT /api/posts/:postId: Update post content

DELETE /api/posts/:postId: Delete a post

POST /api/posts/:postId/reactions: Add a reaction to a post

DELETE /api/posts/:postId/reactions/:reactionId: Remove a reaction from a post

POST /api/users/:userId/friends/:friendId: Send a friend request

PUT /api/users/:userId/friends/:friendId: Accept a friend request

For detailed information on each endpoint, including request/response formats and required parameters, please refer to the API documentation.

Contributing
Contributions to the NoSQL Social Network API are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

When contributing, please adhere to the existing code style and follow the standard Git workflow (fork, branch, commit, pull request).

License
This project is licensed under the MIT License. Feel free to use, modify, and distribute the code as permitted by the license.