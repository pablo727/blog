# Django Blog Project
Welcome to the Django Blog Project, a full-featured blogging platform built with Django and deployed on Fly.io.

This project showcases a practical, production-ready setup featuring CRUD functionality, user accounts, templating, static assets, and Docker-based deployment using Gunicorn and PostgreSQL.

# 🚀 Live Demo
Check out the live site here: https://my-blog-test.fly.dev/

# Features
- Blog app: Create, read, update, and delete blog posts with a clean and user-friendly interface.

- Accounts app: User registration, authentication, and profile management.

- Templates: Django templating engine to render dynamic HTML pages.

- Static files: CSS, JavaScript, and images served efficiently using Django static files setup.

- PostgreSQL: Reliable, production-grade database support.

- Dockerized: Easy to build, run, and deploy using Docker.

- Production-ready server: Runs with Gunicorn for efficient request handling.

- Deployed on Fly.io: Fast and scalable hosting platform.

# ⌨️Getting Started
Prerequisites
Docker installed on your machine

Fly CLI for deployment if you want to push updates: Fly.io CLI

# 🐋Running Locally with Docker
1. Clone the repository

```bash
git clone https://github.com/your-username/blog.git
cd blog
```
2. Build the Docker image

```bash
docker build -t django-blog .
```
3. Run the container, passing your secret key and database info as environment variables

```bash
docker run -it -p 8000:8000 \
   -e SECRET_KEY="your-secret-key" \
   -e DATABASE_URL="postgres://user:password@host:port/dbname" \
   django-blog
```
4. Open your browser at http://localhost:8000

# Project Structure
```php
Copy
Edit
blog/
│
├── blog/              # Django project root (settings, URLs, wsgi)
├── blog_app/          # Blog app (CRUD logic, models, views, templates)
├── accounts/          # User authentication and profile management
├── templates/         # HTML templates
├── static/            # CSS, JavaScript, and image files
├── Dockerfile         # Docker build configuration
├── .dockerignore      # Docker ignore patterns
├── fly.toml           # Fly.io deployment config
└── requirements.txt   # Python dependencies
```
# Deployment
This project is deployed on Fly.io, taking advantage of Docker containerization for seamless scaling and global availability.

# 💻Tech Stack
- Python 3.12 (slim)

- Django

- Gunicorn

- PostgreSQL

- Docker

- Fly.io

# Future Improvements
- Add REST API endpoints for headless CMS capabilities

- Integrate CI/CD pipelines for automated testing and deployment

- Enhance UI with responsive design and modern CSS frameworks

# 📑License
This project is open source and available under the MIT License.
