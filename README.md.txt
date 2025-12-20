AWS Cloud Resume Challenge - Visitor Counter
A full-stack serverless application built on AWS.

- Architecture
Frontend: HTML/CSS hosted on Amazon S3.
API: Amazon API Gateway (HTTP API) with CORS enabled.
Compute: AWS Lambda (Python 3.12).
Database: Amazon DynamoDB for visitor tracking.

- How it Works
When a user visits the S3 website, a JavaScript `fetch` call triggers the API Gateway. The API invokes a Lambda function that increments a value in DynamoDB and returns the new count to the frontend.