# Docker Practice Projects

A collection of small hands-on projects built while learning **Docker** and **Docker Compose** - from containerizing a single script to orchestrating a multi service application stack.

## 📁 Projects

### 1. PHP + Apache (`app1/`)
A basic PHP web app served with Apache, running inside a Docker container.

- **Tech:** PHP 7.4, Apache
- **Run it:**
  ```bash
  cd app1
  docker build -t img-php-apache-example .
  docker run -it -d -p 8080:80 img-php-apache-example
  ```
**Test:** curl localhost:8080
**Output:**
  Welcome to Meem_shah
  Running php with Apache on Docker

---

### 2. PHP CLI Script (`app2/`)
A PHP command line script running inside a lightweight CLI based container (no web server needed).

- **Tech:** PHP 7.4 CLI
- **Run it:**
  ```bash
  cd app2
  docker build -t img-php-cli-example .
  docker run -it --rm img-php-cli-example
  ```
**Output:**
  Welcome to Meem_shah
  Running php CLI script with docker

---

### 3. Python Script (`app3/`)
A simple Python script containerized and executed on container startup.

- **Tech:** Python 3
- **Run it:**
  ```bash
  cd app3
  docker build -t mypython .
  docker run -it mypython
  ```
**Output:**
Welcome to Meem_shah
This is Python running in Docker

---

### 4. WordPress + MySQL Stack (`app4/`)
A full multi container setup using **Docker Compose**, running WordPress connected to a MySQL database - demonstrating service orchestration, networking, and persistent volumes.

- **Tech:** WordPress, MySQL 5.7, Docker Compose
- **Run it:**
  ```bash
  cd app4
  docker compose up
  ```
- **Access:** `localhost:8000`
  
## 🚀 Getting Started

**Clone the repository:**
```bash
git clone https://github.com/abdulraheem774/docker-practice-projects.git
cd docker-practice-projects
```

Then move into any project folder (`app1`, `app2`, `app3`, or `app4`) and follow the build/run commands listed under that project above.

---

## 🎯 What This Covers

- Writing Dockerfiles for different runtimes (Apache, CLI, Python)
- Building and running containers manually
- Exposing and mapping ports
- Multi-container orchestration with Docker Compose
- Managing environment variables and persistent volumes

## 🛠 Requirements

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/) (included with Docker Desktop / recent Docker Engine)

---

*Built as part of hands-on Docker learning during an AIOps/DevOps/Cybersecurity diploma.*
