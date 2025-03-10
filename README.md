# FastAPI Project



This is a FastAPI project that demonstrates how to build and run a simple web application using Docker.

## Project Structure

```
fast-api-project
├── .github
│   └── workflows
│       └── ci.yml
├── src
│   └── main.py
├── Dockerfile
├── requirements.txt
└── README.md
```

## Requirements

- Python 3.7+
- Docker

## Setup Instructions

1. Clone the repository:

   ```
   git clone https://github.com/yourusername/fast-api-project.git
   cd fast-api-project
   ```

2. Install the required Python packages:

   ```
   pip install -r requirements.txt
   ```

## Running the Application

To run the FastAPI application locally, you can use the following command:

```
uvicorn src.main:app --reload
```

This will start the server at `http://127.0.0.1:8000`.

## Running with Docker

To build and run the application using Docker, execute the following commands:

1. Build the Docker image:

   ```
   docker build -t fastapi-app .
   ```

2. Run the Docker container:

   ```
   docker run -d -p 8000:8000 fastapi-app
   ```

The application will be accessible at `http://localhost:8000`.

## CI/CD

This project includes a GitHub Actions workflow for continuous integration, defined in `.github/workflows/ci.yml`. It automates the process of building and testing the application whenever changes are pushed to the repository.

## License

This project is licensed under the MIT License.
