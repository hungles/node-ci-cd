# Node CI/CD Project

Este es un pequeño proyecto en Node.js que incluye integración continua y despliegue continuo (CI/CD) usando GitHub Actions.

## Requisitos

- Node.js >= 18
- npm

## Instalación

```bash
npm install
```

## Levantar el proyecto

```bash
npm start
```

## Ejecutar tests

```bash
npm test
```

## Construir imagen Docker

1. Asegúrate de tener Docker instalado.
2. Construye la imagen:

    ```bash
    docker build -t node-ci-cd-app .
    ```

3. Ejecuta el contenedor:

    ```bash
    docker run -p 3000:3000 node-ci-cd-app
    ```

## CI/CD con GitHub Actions

Este proyecto está integrado con GitHub Actions. Cada push o pull request ejecuta automáticamente los tests y puede desplegar la aplicación si los tests pasan.

El flujo de trabajo se encuentra en `.github/workflows/ci-cd.yml`.

---

¡Contribuciones y sugerencias son bienvenidas!