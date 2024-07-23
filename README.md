# Social Network API

## Description

This is an API for a social network web application where users can share their thoughts, react to friends’ thoughts, and create a friend list. The API is built using Express.js for routing, a MongoDB database, and the Mongoose ODM.

## Installation

1. Clone the repository
2. Install dependencies: `npm install`
3. Start the server: `npm start`

## Usage

The API provides the following routes:

- `/api/users`
  - GET all users
  - POST a new user
- `/api/users/:userId`
  - GET a single user by ID
  - PUT to update a user by ID
  - DELETE to remove a user by ID
- `/api/users/:userId/friends/:friendId`
  - POST to add a new friend to a user's friend list
  - DELETE to remove a friend from a user's friend list
- `/api/thoughts`
  - GET all thoughts
  - POST a new thought
- `/api/thoughts/:thoughtId`
  - GET a single thought by ID
  - PUT to update a thought by ID
  - DELETE to remove a thought by ID
- `/api/thoughts/:thoughtId/reactions`
  - POST to create a reaction in a single thought's reactions array
  - DELETE to remove a reaction by the reaction's reactionId

## Demo

Include a link to a walkthrough video that demonstrates the functionality of the application.

## License

This project is licensed under the MIT License.
