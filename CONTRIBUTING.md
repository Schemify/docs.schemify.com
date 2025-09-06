<!-- `docs/CONTRIBUTING.md` es un archivo de texto en formato Markdown que se suele incluir dentro de un repositorio (por convención, en la carpeta `docs/` o en la raíz).

Su propósito es **explicar a colaboradores externos cómo contribuir al proyecto**. Normalmente incluye:

* Guía para clonar y levantar el entorno local.
* Reglas de estilo (nombres de ramas, convenciones de commits, etc.).
* Flujo de trabajo con issues y pull requests.
* En tu caso, también los pasos para traducir con **GitLocalize** y revisar los PRs.

👉 Piensa en él como un “manual para contribuir” que los futuros traductores o desarrolladores puedan seguir sin preguntarte nada.

¿Quieres que te redacte un borrador de `docs/CONTRIBUTING.md` enfocado en la traducción con GitLocalize para tu proyecto Docusaurus? -->

# Website

This website is built using [Docusaurus](https://docusaurus.io/), a modern static website generator.

## Installation

```bash
yarn
```

## Local Development

```bash
yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

## Build

```bash
yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

## Deployment

Using SSH:

```bash
USE_SSH=true yarn deploy
```

Not using SSH:

```bash
GIT_USER=<Your GitHub username> yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.
