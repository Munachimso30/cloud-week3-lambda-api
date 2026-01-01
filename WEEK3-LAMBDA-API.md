# Week 3 – Serverless API with Lambda

## Goal
Build a serverless HTTP API using AWS Lambda (Python) and API Gateway HTTP API.

## Architecture
- HTTP API Gateway (dev stage) → Lambda function `week3-hello-api` returning JSON.

## Steps
1. Created Lambda with Python 3.11 and handler `lambda_function.lambda_handler`.
2. Implemented query parameter `name` and returned `{"message": "Hello, <name> from Lambda!"}`.
3. Created HTTP API `week3-lambda-http-api` with route `GET /week3-hello-api`.
4. Deployed to `dev` stage with auto‑deploy enabled.

## Testing
- `GET https://eyiettkmqj.execute-api.eu-north-1.amazonaws.com/dev/week3-hello-api`
- `GET https://eyiettkmqj.execute-api.eu-north-1.amazonaws.com/dev/week3-hello-api?name=Munachimso`

![Lambda code](screenshots/week3-lambda-code.png)
