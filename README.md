# University Housing User Authentication Service

The University Housing User Authentication Service is a Django-based microservice designed to manage user authentication, registration, and authorization for the University Housing project. This service ensures a secure and seamless user experience for accessing the various features of the application.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
  - [Prerequisites](#prerequisites)
  - [Setting up a Virtual Environment](#setting-up-a-virtual-environment)
  - [Database Setup](#database-setup)
- [Usage](#usage)
  - [Running Locally](#running-locally)
  - [Running with Docker](#running-with-docker)
- [Contributing](#contributing)

## Features

- User registration with email verification.
- User authentication and login.
- Password reset functionality.
- Role-based authorization (e.g., Student, Landlord, Admin).
- User profile management.

## Installation

### Prerequisites

- Python 3.x
- Pip (Python package installer)
- Docker (optional)

### Setting up a Virtual Environment

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/university-housing-auth.git
    cd university-housing-auth
    ```

2. Create and activate a virtual environment:

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

### Database Setup

4. Apply migrations:

    ```bash
    python manage.py migrate
    ```

## Usage

### Running Locally

5. Run the development server:

    ```bash
    python manage.py runserver
    ```

6. Access the User Authentication Service at [http://localhost:8000/](http://localhost:8000/).

### Running with Docker

5. Build the Docker image:

    ```bash
    docker build -t university-housing-auth .
    ```

6. Run the Docker container:

    ```bash
    docker run -p 8000:8000 university-housing-auth
    ```

7. Access the User Authentication Service at [http://localhost:8000/](http://localhost:8000/).

## Contributing

If you'd like to contribute to the development of the University Housing User Authentication Service, please follow our [Contribution Guidelines](CONTRIBUTING.md).
