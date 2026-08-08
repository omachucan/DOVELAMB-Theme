# DOVELAMB Theme Architecture

## Overview

DOVELAMB Theme is a custom Oh My Posh configuration designed to provide a consistent terminal experience across the DOVELAMB development ecosystem.

The project follows a simple architecture intentionally. Oh My Posh consumes a single configuration file, so the initial version avoids unnecessary build or composition processes.

## Architecture Principles

The project follows these principles:

- Keep the terminal clean and readable.
- Display only useful contextual information.
- Maintain compatibility across Windows and Linux environments.
- Keep the configuration easy to understand and maintain.
- Add integrations only when they become part of the real development environment.
- Avoid unnecessary complexity.

## Project Structure

```text
DOVELAMB-Theme
│
├── README.md
├── .gitignore
│
├── assets
│   └── previews
│
├── docs
│   ├── README.es.md
│   ├── ARCHITECTURE.md
│   ├── CHANGELOG.md
│   └── ROADMAP.md
│
├── scripts
│
└── src
    └── doverlamb.omp.json
```

## Main Configuration

The main theme configuration is located at:

```text
src/doverlamb.omp.json
```

This file is the source of truth for the DOVELAMB Oh My Posh theme.

## Planned Context Segments

The theme will progressively support contextual information for:

- Workstation identity
- Current user
- Working directory
- Git
- Java
- Maven / Gradle
- Node.js
- Docker
- Kubernetes
- Cloud environments

Segments will be introduced progressively and only when they provide meaningful information.

## Portability

The theme is intended to be reusable across the DOVELAMB infrastructure, including Windows workstations and Linux-based systems.

Platform-specific behavior should be minimized whenever possible.