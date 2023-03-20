# Dockerized Vue

Dockerized a starter Vue project for development, testing and production and hmr support for development & testing


## Features

- Dockerize a starter vue project
- Separate dockerfile for both development and production
- Add HMR support for development and testing
- In production serve the build file with nginx
- For development and test use docker compose 



## All available links

- For development with hmr support
  - http://localhost:5173
- For testing with hmr support 
  - http://localhost:5174
- For production 
  - http://localhost:5175


## Available docker command in npm package.json
```json
"docker:prod:build": "docker build -t frontend_prod -f Dockerfile.prod .",
"docker:prod:run": "docker run -p 5175:80 -it frontend_prod:latest",
"docker:dev:run": "docker compose up",
"docker:dev:build&run": "docker compose up --build"
```
