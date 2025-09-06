---
sidebar_position: 1
---

# Schemify

Una CLI para generar proyectos y artefactos de nivel productivo siguiendo buenas prácticas de arquitectura de software (DDD, Hexagonal, CQRS, gRPC, Kafka, Prisma, Docker).

## Características / Destacados
- Scaffolding con opinión fuerte alineado a Domain-Driven Design y Arquitectura Hexagonal.  
- Plantillas listas para CQRS, controladores gRPC, consumidores Kafka y repositorios Prisma.  
- Estructura monorepo consistente con límites claros de puertos/adaptadores.  
- Plantillas preparadas para producción con pruebas integradas y Docker Compose para orquestación local.  
- Flujo CLI amigable para generar nuevos microservicios y artefactos.  

## Instalación

**Requisitos previos**
- **Node.js** ≥ 18.x (instalar desde la web oficial: https://nodejs.org/)  
- **Docker** para servicios locales (bases de datos, Kafka): https://www.docker.com/  

**Instalar la CLI**
```bash
npm install -g @schemifyjs/cli
# o con pnpm
# pnpm add -g @schemifyjs/cli
# o con yarn
# yarn global add @schemifyjs/cli
````

Paquete NPM: [https://www.npmjs.com/package/@schemifyjs/cli](https://www.npmjs.com/package/@schemifyjs/cli)

## Primeros Pasos

Crea un nuevo servicio usando la CLI:

```bash
schemify new <nombre-de-tu-proyecto>
```

Instala dependencias y ejecuta:

```bash
cd <nombre-de-tu-proyecto>
npm install
npm run start:dev
```

<!-- 
Si el proyecto generado incluye infraestructura (ej. PostgreSQL, Kafka), levántala con Docker:

```bash
docker compose up -d
```

Genera artefactos adicionales:

```bash
schemify generate grpc-controller users
schemify generate kafka-consumer example-created
```
-->

## Licencia

MIT

## Contribuir

Las contribuciones son bienvenidas.
Abre un issue para discutir cambios significativos, usa *conventional commits* y agrega pruebas cuando sea posible.

## Créditos / Comunidad (opcional)

Mantenido por colaboradores de Schemify.
NPM: [https://www.npmjs.com/package/@schemifyjs/cli](https://www.npmjs.com/package/@schemifyjs/cli)
