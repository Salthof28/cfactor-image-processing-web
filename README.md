# CFactor Image Processing Web

A full-stack image processing application built with **Next.js**, **NestJS**, **BullMQ**, **Redis**, and **Docker Compose**.

The application allows users to upload an image, process it asynchronously in the background, monitor the processing status, and download the optimized WebP image.

---

## Tech Stack

* Next.js
* NestJS
* TypeScript
* Tailwind CSS
* TanStack Query
* BullMQ
* Redis
* Sharp
* Docker Compose

---

## Project Structure

```text
.
├── be-cfactor-image-processing-web/     # Backend (NestJS)
├── fe-cfactor-image-processing-web/     # Frontend (Next.js)
└── docker-compose.yml                   # Docker Compose configuration
```

---

## Documentation

Detailed documentation for each project is available below:

* [Frontend Documentation](./fe-cfactor-image-processing-web/README.md)
* [Backend Documentation](./be-cfactor-image-processing-web/README.md)

---

## Prerequisites

Before running the project, ensure you have installed:

* Docker
* Docker Compose

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Salthof28/cfactor-image-processing-web.git
cd cfactor-image-processing-web
```

### 2. Start all services

```bash
docker compose up --build
```

This command will build and start:

* Frontend
* Backend
* Redis

---

## Access the Application

After all containers have started successfully:

| Service  | URL                   |
| -------- | --------------------- |
| Frontend | http://localhost:3000 |
| Backend  | http://localhost:4000 |

---

## Stop the Services

```bash
docker compose down
```

To remove all containers, networks, and volumes:

```bash
docker compose down -v
```

---

## Notes

* Ensure ports **3000** and **4000** are available before starting the containers.
* Redis is automatically started by Docker Compose.
* The frontend communicates with the backend through the configured API endpoint.
* Uploaded images are processed asynchronously using BullMQ.

---

## Author
🔧 Salman Althof

---
