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

To execute these requests sequentially using Newman, follow these steps:

    Install Node.js: Make sure you have Node.js installed on your machine.

    Install Newman: Open the command prompt and run the following command to install Newman globally:

npm install -g newman

Export Collection: Export the Postman collection containing the above requests as a JSON file.

execute using this command

newman run (path-to-collection-file).json -e(path-to-collection-environtment-file).json -r cli,json

Replace (path-to-collection-file) with the path to the exported collection JSON file, 
Replace (path-to-collection-environtment-file) with the path to exorted collection environtment JSON file,

If you want to make it short just convert it to js file. 

Create a new file with the .bat extension: Open a text editor (e.g., Notepad) and create a new file.

Copy the shell command into the file: Copy the shell command used to run the Newman test and paste it into the newly created file.

Adjust the syntax for Windows Command Prompt:

    Replace the shebang (#!/bin/bash) at the beginning of the shell command with @echo off.
    Replace the forward slashes (/) with backslashes (\) in the file paths.
    Remove the .sh file extension from the file name.

For example, the shell command:

bash

#!/bin/bash
newman run (path-to-collection-file).json -e (path-to-data-file).json

Becomes:

vbnet

@echo off
newman run (path-to-collection-file).json -e (path-to-data-file).json

Save the file with a .bat extension: Save the file with a .bat extension, such as api_test.bat.

Execute the batch file in Windows Command Prompt: Open the Windows Command Prompt, navigate to the directory where the batch file is saved, and run the batch file by entering its name. For example:

    api_test.bat

    This will execute the Newman test using the batch file in the Windows Command Prompt.

By following these steps, you can convert the shell command to a batch file that can be executed in the Windows Command Prompt.

Observe the Newman execution: The Newman tool will execute the API requests one by one and display the results on the command prompt.

