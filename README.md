# Django Blog Project
Welcome to the Django Blog Project, a full-featured blogging platform built with Django and deployed on Fly.io.

This project showcases a practical, production-ready setup featuring CRUD functionality, user accounts, templating, static assets, and Docker-based deployment using Gunicorn and PostgreSQL.

---

## 🚀 Live Demo
🌐  Check out the live site here: https://my-blog-test.fly.dev/

---

## Features
- 📝  **Blog app**: Create, read, update, and delete blog posts with a clean and user-friendly interface.

- 👤 **Accounts app**: User registration, authentication, and profile management.

- 🧩 **Templates**: Django templating engine to render dynamic HTML pages.

- 🎨 **Static files**: CSS, JavaScript, and images served efficiently using Django static files setup.

- 🐘 **PostgreSQL**: Reliable, production-grade database support.

- 🐳 **Dockerized**: Easy to build, run, and deploy using Docker.

- 🐍 **Production-ready server**: Runs with Gunicorn for efficient request handling.

- ☁️ **Deployed on Fly.io**: Fast and scalable hosting platform.

---

## ⌨️ Getting Started
### ✅ Prerequisites
- [Docker](https://www.docker.com/) installed on your machine  
- [Fly CLI](https://fly.io/docs/hands-on/install-flyctl/) for deployment (optional)

---

### 🐋 Running Locally with Docker
# Clone the repository

```bash
git clone https://github.com/your-username/blog.git
cd blog
```

# Build the Docker image

```bash
docker build -t django-blog .
```

# Run the container, passing your secret key and database info as environment variables

```bash
docker run -it -p 8000:8000 \
   -e SECRET_KEY="your-secret-key" \
   -e DATABASE_URL="postgres://user:password@host:port/dbname" \
   django-blog
```

# Open your browser at http://localhost:8000

## 🗂️ Project Structure
```php
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

---

## 🚢  Deployment
This project is deployed on Fly.io, taking advantage of Docker containerization for seamless scaling and global availability.

## 💻 Tech Stack
![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python)
![Django](https://img.shields.io/badge/Django-4.x-success?logo=django)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-15-blue?logo=postgresql)
![Docker](https://img.shields.io/badge/Docker-ready-blue?logo=docker)
![Gunicorn](https://img.shields.io/badge/Gunicorn-enabled-green)
![Fly.io](https://img.shields.io/badge/Deployed-Fly.io-purple?logo=fly.io)

---

## 📑License
This project is open source and available under the MIT License.
