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
├── postgresql13/
├── postgresql16/
├── redis/
└── README.md
```
