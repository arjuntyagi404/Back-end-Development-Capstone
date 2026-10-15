# Back-End Development Capstone

## Project Overview

This project is a Django web application that integrates the course's backend services and provides pages for the band's information, songs, photos, and concerts.

## Prerequisites

- Python compatible with the project's requirements
- pip
- Git
- The project dependencies listed in `requirements.txt`

## Environment Setup

### 1. Obtain the Project

Clone or download the `Back-end-Development-Capstone` repository and open a terminal in the project root directory, where `manage.py` is located.

### 2. Create and Activate a Virtual Environment

Create a virtual environment if one does not already exist:

```bash
python3 -m venv backend-django-venv
```

Activate it in Bash:

```bash
source backend-django-venv/bin/activate
```

### 3. Install Dependencies

If the repository contains `requirements.txt`, install the dependencies:

```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables

Configure any required database connection settings, service URLs, credentials, and other environment variables according to the course lab instructions. Do not commit secrets or passwords to the repository.

### 5. Apply Database Migrations

From the directory containing `manage.py`, run:

```bash
python manage.py migrate
```

If the application requires new migrations for modified models, follow the course instructions for generating and applying them.

### 6. Create a Django Administrator

Create an administrator account with:

```bash
python manage.py createsuperuser
```

Follow the prompts to configure the username, email address if requested, and password. Use the credentials you created to sign in to Django Admin.

### 7. Start the Development Server

Run:

```bash
python manage.py runserver
```

Open the local address printed by Django in your browser. Use the course lab instructions for the correct deployed application URL when testing a deployed version.

## Running Tests

If the repository includes Django tests, run:

```bash
python manage.py test
```

## Application Pages

The application may include the following pages, depending on the project configuration:

- Home
- Songs
- Photos
- Concerts
- Login and signup
- Django administration

## Deployment

Deployment configuration and commands depend on the target environment. Follow the course instructions for building the container image, configuring the deployment, applying Kubernetes or OpenShift resources, and verifying the deployed application.

## Security Notes

Do not store passwords, API keys, or database credentials in source control. Configure secrets through the appropriate environment or deployment settings.
