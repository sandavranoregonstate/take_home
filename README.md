# Using the code.
Create the virtual environment and install flask.

```
python3 -m venv venv
source venv/bin/activate
pip install flask
```

Start up the server.

`flask --app main run`

# API documentation.

## Overview

This API provides a service for translating text into sign language. It accepts text input and returns a confirmation of successful translation.

## Base URL

`http://127.0.0.1:5000`


## Endpoints

### Translate Text to Sign Language

Simulates sign language translation.

- **URL:** `/`
- **Method:** `POST`
- **Content-Type:** `application/json`

#### Request Body

| Field | Type   | Description                   | Required |
|-------|--------|-------------------------------|----------|
| text  | string | The text to be translated     | Yes      |

#### Example Request

```
curl -X POST -H "Content-Type: application/json" -d '{"text":"Hello, world!"}' http://127.0.0.1:5000
```