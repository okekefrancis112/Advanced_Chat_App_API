# Advanced Chat App API

An advanced chat application API built with Django REST Framework, containerized with Docker, and integrated with GitHub Actions for CI/CD.

## Overview

A production-ready chat API with user authentication, real-time messaging capabilities, and automated testing pipeline.

## Features

- **User Authentication** — Registration and token-based login
- **Chat Messaging** — Create and manage chat conversations
- **Docker** — Fully containerized with Docker and Docker Compose
- **CI/CD** — GitHub Actions for automated testing and linting
- **Flake8** — Code quality enforcement

## Tech Stack

- **Python** 3.x
- **Django** + **Django REST Framework**
- **Docker** + **Docker Compose**
- **PostgreSQL** — Database
- **GitHub Actions** — CI/CD pipeline

## Getting Started

```bash
git clone https://github.com/okekefrancis112/Advanced_Chat_App_API.git
cd Advanced_Chat_App_API
docker-compose build
docker-compose up
```

### Run Tests

```bash
docker-compose run --rm app sh -c "python manage.py test"
```

### Lint

```bash
docker-compose run --rm app sh -c "flake8"
```

## Project Structure

```
├── app/
│   ├── core/              # Core models and admin
│   ├── chat/              # Chat app (messages, conversations)
│   ├── user/              # User authentication
│   └── app/               # Django settings
├── Dockerfile
├── docker-compose.yml
└── .github/workflows/     # CI/CD checks
```

## License

MIT
