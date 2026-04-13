# Third-repository-
API testing project using Postman to validate RESTful services, including request handling, response validation, and automated test scripts.
# API Testing Project - Postman

## Overview
This project demonstrates API testing using Postman by validating RESTful APIs, verifying responses, and ensuring proper system behavior.

## Objectives
- Test API endpoints using different HTTP methods
- Validate response data and status codes
- Ensure proper error handling
- Automate API test scenarios

## Features
- Tested GET, POST, PUT, DELETE requests
- Validated status codes (200, 201, 400, 404)
- Verified response body structure and data integrity
- Automated test scripts using JavaScript in Postman
- Tested edge cases and error responses

## Tools & Technologies
- Postman
- REST APIs
- JavaScript (Postman test scripts)

## Sample Test Scenarios
1. Retrieve data using GET request
2. Create new data using POST request
3. Update existing data using PUT request
4. Delete data using DELETE request
5. Validate error response for invalid requests

## Example API Used
https://jsonplaceholder.typicode.com

## Sample Test Script
```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Response contains data", function () {
    const jsonData = pm.response.json();
    pm.expect(jsonData).to.not.be.empty;
});
