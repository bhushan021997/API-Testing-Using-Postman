# API-Testing-Using-Postman

## API Testing with Postman
This repository contains Postman collections and environments for testing the API endpoints of the [Restful Booker API's]. 

The purpose of this document is to guide you through setting up and running API tests using Postman.

## Table of Contents
Prerequisites

Installation

Setup

Running Tests

Environment Variables

Collection Structure

Contributing

License

## Prerequisites
Before you begin, ensure you have the following installed on your machine:

## Postman
Node.js (if you plan to run tests using Newman)

## Open Postman.
Click on Import in the top left corner.

Select Upload Files and choose the YourCollection.postman_collection.json file.

Repeat the process for the environment file YourEnvironment.postman_environment.json.

## Configure Environment Variables:

Go to the Environments tab in Postman.

Select the environment you imported (e.g., QA).

Update the initial and current values for the environment variables as per your setup (e.g., baseUrl, apiKey, etc.).

Running Tests Using Postman
## Select Environment:

In the top right corner of Postman, select the environment you want to use (e.g., QA).

## Run Collection:

Go to the Collections tab.

Hover over the imported collection and click on the Run button.

In the Collection Runner, select the appropriate environment and click Start Test.

## Using Newman
To run the collection from the command line, use the following command:
sh
Copy code
newman run YourCollection.postman_collection.json -e YourEnvironment.postman_environment.json
Environment Variables
The environment file contains variables that can be used throughout the requests in the collection. Common variables include:

baseUrl: The base URL for the API.

apiKey: The API key for authentication (if applicable).

userId: Example user ID for testing.

Ensure these variables are correctly set before running the tests.

## Collection Structure
The Postman collection is organized into folders based on the API endpoints. Each folder contains requests for the respective endpoint operations (e.g., GET, POST, PUT, DELETE).

Example Structure
Auth

Get Booking 

Get Single Booking

Create Booking

Update Booking

Delete Booking



