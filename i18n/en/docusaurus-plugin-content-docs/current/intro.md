---
sidebar_position: 1
---


<!-- 
💬 Instrucciones (ES):
- Mantén este README como una introducción técnica breve (landing).
- NO incluyas Tabla de Contenidos.
- Separa "Installation" (herramientas + CLI) y "Getting Started" (uso básico).
- Ajusta las secciones según tu flujo real y plantillas disponibles.
-->

# Schemify

A CLI to scaffold production-grade projects and artifacts following software architecture best practices (DDD, Hexagonal, CQRS, gRPC, Kafka, Prisma, Docker).

<!-- (Opcional) Inserta logo o badges aquí:
<p align="left">
  <img src="LINK_TO_LOGO" width="120" alt="Schemify Logo" />
</p>
-->

## Features / Highlights
- Opinionated scaffolding aligned with Domain-Driven Design and Hexagonal Architecture.
- First-class scaffolds for CQRS, gRPC controllers, Kafka consumers, and Prisma repositories.
- Consistent monorepo layout with clear ports/adapters boundaries.
- Production-ready templates with testing hooks and Docker Compose for local orchestration.
- Friendly CLI workflow to generate new microservices and artifacts.

## Installation
<!-- 
💬 Instrucciones (ES):
- Combina aquí herramientas requeridas y la instalación mínima de la CLI.
- Usa enlaces oficiales y mantén pasos claros.
-->

**Prerequisites**
- **Node.js** ≥ 18.x (install from the official website: https://nodejs.org/)
<!-- - **npm** (bundled with Node.js) or **pnpm/yarn** -->
- **Docker** for local services (databases, Kafka): https://www.docker.com/
<!-- - (Optional) **Docker Compose** v2 for multi-service orchestration -->

**Install the CLI**
```bash
npm install -g @schemifyjs/cli
# or with pnpm
# pnpm add -g @schemifyjs/cli
# or with yarn
# yarn global add @schemifyjs/cli
```

NPM package: [https://www.npmjs.com/package/@schemifyjs/cli](https://www.npmjs.com/package/@schemifyjs/cli)

## Getting Started

<!-- 
💬 Instrucciones (ES):
- Muestra un flujo mínimo, tipo "hello world".
- Si el template genera infraestructura, indica cómo levantarla con Docker.
-->

Create a new service using the CLI:

```bash
schemify new <your-project-name>
```

Install dependencies and run:

```bash
cd <your-project-name>
npm install
npm run start:dev
```
<!-- 
If your generated project includes infrastructure (e.g., PostgreSQL, Kafka), start it with Docker:

```bash
# If the project includes a docker-compose.yml
docker compose up -d
```

Generate additional artifacts:

```bash
# Example commands (actual names depend on available schematics):
schemify generate grpc-controller users
schemify generate kafka-consumer example-created
``` 
-->
<!-- :::tip Requisito rápido
Instala **Node.js 18+** y **Docker** antes de usar la CLI.
::: -->

## License

MIT

## Contributing

Contributions are welcome.
Open an issue to discuss significant changes, follow conventional commits, and include tests when possible.

## Credits / Community (optional)

Maintained by Schemify contributors.
NPM: [https://www.npmjs.com/package/@schemifyjs/cli](https://www.npmjs.com/package/@schemifyjs/cli)

