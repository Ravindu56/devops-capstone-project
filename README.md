## Project Description

This repository contains my implementation of the **DevOps Capstone Project**, part of the IBM DevOps and Software Engineering Professional Certificate on Coursera. The project builds a **Customer Accounts RESTful microservice** for an e-commerce platform, following Agile, Test-Driven Development (TDD), and DevOps best practices from planning through production deployment.

### What This Service Does

The microservice manages customer account records, including name, email, address, phone number, and date joined. It exposes a full set of REST API endpoints to **create, read, update, delete, and list** customer accounts, backed by a PostgreSQL database and following the Model-View-Controller (MVC) pattern.

### Development Approach

- **Agile Planning** — Managed via a GitHub Kanban board with a structured Product Backlog, Sprint Backlog, and user story templates.
- **Test-Driven Development (TDD)** — All REST endpoints were built by writing failing tests first, then implementing just enough code to pass them, maintaining at least 95% test coverage.
- **Continuous Integration (CI)** — A GitHub Actions workflow automatically lints (Flake8), tests, and checks coverage on every push and pull request to `main`.
- **Secure Coding** — Flask-Talisman enforces HTTPS and security headers; Flask-CORS manages Cross-Origin Resource Sharing policies.
- **Containerization & Deployment** — The service is packaged in Docker, pushed to IBM Cloud Container Registry, and deployed to an OpenShift/Kubernetes cluster with PostgreSQL as a managed service.
- **Continuous Delivery (CD)** — A Tekton pipeline automates cloning, linting, testing, image building, and deployment to Kubernetes without manual intervention.

### Tech Stack

Python, Flask, PostgreSQL, Docker, Kubernetes, OpenShift, GitHub Actions, Tekton, Nose/PyTest, Flake8, Flask-Talisman, Flask-CORS.
