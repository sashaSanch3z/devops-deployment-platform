# DevOps Deployment Platform

A hands-on DevOps portfolio project focused on
building, testing, and deploying a Python application.

## Goals

- Build a simple Python API
- Add automated tests
- Containerize the application with Docker
- Create a CI/CD pipeline
- Document deployment and troubleshooting

## Current Status

- [x] Create a Flask API with a health endpoint
- [x] Set up a Python virtual environment
- [x] Add `.gitignore`
- [x] Add automated tests
- [ ] Containerize the application with Docker
- [ ] Set up CI/CD with GitHub Actions

## API

### Health Check

- **Method:** `GET`
- **Endpoint:** `/health`
- **Response:** `{"status": "ok"}`

## Run Locally

Activate the virtual environment:

```bash
source .venv/bin/activate
```

Install Flask:

```bash
python -m pip install flask
```

Start the application:

```bash
python app/main.py
```

Open `http://127.0.0.1:5000/health` in your browser.

## Automated Tests

Run the tests with:

```bash
python -m pytest -v
```

The tests verify the health endpoint response:
- HTTP status code `200`
- JSON response `{"status": "ok"}`

## Dependencies

Install the project dependencies:

```bash
python -m pip install -r requirements.txt
```