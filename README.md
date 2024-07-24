# Social Network API

## Description

This is an API for a social network web application where users can share their thoughts, react to friends’ thoughts, and create a friend list. The API is built using Express.js for routing, a MongoDB database, and the Mongoose ODM.

## Table of Contents

- [Description](#description)
- [Installation](#installation)
- [Usage](#usage)
- [User Story](#user-story)
- [Acceptance Criteria](#acceptance-criteria)
- [Links](#link-to-github-repository)

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

## User Story

AS A social media startup
I WANT an API for my social network that uses a NoSQL database
SO THAT my website can handle large amounts of unstructured data

## Acceptance Criteria

GIVEN a social network API
WHEN I enter the command to invoke the application
THEN my server is started and the Mongoose models are synced to the MongoDB database
WHEN I open API GET routes in Insomnia for users and thoughts
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia
THEN I am able to successfully create, update, and delete users and thoughts in my database
WHEN I test API POST and DELETE routes in Insomnia
THEN I am able to successfully create and delete reactions to thoughts and add and remove friends to a user’s friend list

## Links

Link to Github Repository:

https://github.com/adamh1223/social-network-api

Link to video demonstration:

https://vimeo.com/989317224?share=copy
