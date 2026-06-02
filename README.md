# containers

Docker Compose configurations for local development.

This repository contains reusable Docker Compose setups for common backend infrastructure such as databases and message brokers.  
It is intended to be used alongside application repositories and does **not** contain application code.

---

## Purpose

- Centralize local development containers
- Avoid duplicating Docker Compose files across projects
- Make local setup fast and consistent

---

## Repository Structure

```text
containers/
├── kafka-confluentinc/
├── pgadmin/
├── postgresql13/
├── postgresql16/
├── redis/
└── README.md
```

---

## Getting Started

### Prerequisites

Several containers (such as PostgreSQL and pgAdmin) share an external Docker network named `shared-network`. This network **must be created manually** before starting the containers:

```bash
docker network create shared-network
```

### Usage

Navigate to the directory of the service you wish to run, then start it using:

```bash
docker compose up -d
```
