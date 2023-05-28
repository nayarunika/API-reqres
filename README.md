# API Collection Testing for regres.in

This repository contains an API collection for testing various endpoints of the regres.in web application. The API collection includes tests for creating, retrieving, updating, and deleting user data.

## Table of Contents

- [Introduction](#introduction)
- [Endpoints](#endpoints)
- [Getting Started](#getting-started)
- [Test Execution](#test-execution)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The regres.in API provides a simple web service for testing purposes, allowing you to simulate user management operations. This API collection focuses on testing the following user-related operations:

- Create User: Test the endpoint for creating a new user.
- Get User: Test the endpoint for retrieving user information.
- Edit User Name: Test the endpoint for updating a user's name.
- Delete User: Test the endpoint for deleting a user.

## Endpoints

The API collection includes the following endpoints:

- `POST /api/users`: Create a new user.
- `GET /api/users/{id}`: Retrieve user information by ID.
- `PUT /api/users/{id}`: Update a user's name by ID.
- `DELETE /api/users/{id}`: Delete a user by ID.

Refer to the API documentation for more details on each endpoint's request and response formats.

## Getting Started

To get started with testing the API collection, follow these steps:

1. Install a REST client: Choose a REST client tool like Postman or Insomnia to execute the API requests.

2. Clone the repository: Clone this repository to your local machine using the following command:

   ```bash
   git clone <repository_url>
Replace <repository_url> with the URL of this GitHub repository.

Import the API collection: Import the API collection file (api_collection.json) into your chosen REST client. This collection contains pre-configured requests for each endpoint.

Configure environment variables: Set up any required environment variables for the API collection, such as the base URL of the regres.in API.

Review and update variables: Review the variable placeholders in the API requests and update them with appropriate values if needed (e.g., user IDs).

Test Execution
Once you have imported the API collection and set up the environment, follow these steps to execute the tests:

Run the desired API requests: Execute the requests in the API collection to perform various user operations such as creating, retrieving, updating, and deleting users.

Verify the response: Inspect the response from each request to ensure it matches the expected behavior. Check the response status codes, response body, and any relevant data returned.

Validate the functionality: Verify that the user operations, such as creating a user, retrieving user details, updating the user's name, and deleting a user, are functioning correctly according to the API documentation.

Analyze test results: Record the test results and any issues encountered during testing. Identify any failures or unexpected behavior and troubleshoot accordingly.

Contributing
Contributions to this API collection testing project are welcome! If you have any improvements, bug fixes, or additional tests to suggest, feel free to open an issue or submit a pull request.

When contributing, please follow the existing coding style, include appropriate documentation, and ensure that the tests are passing.
