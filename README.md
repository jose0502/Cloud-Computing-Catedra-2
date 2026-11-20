# ACI606 - Docker Rescue Challenge

## Arquitectura
Frontend (Nginx) -> Backend (FastAPI) -> Database (PostgreSQL)

## Cómo iniciar la aplicación
1. Crear el archivo `.env` en la raíz (usar `.env.example` como guía).
2. Ejecutar: `docker compose up --build -d`
3. Verificar que todos los servicios estén "Up": `docker compose ps`
4. Acceder al frontend: `http://localhost:8080`

## Cómo detener la aplicación
`docker compose down`

## Cómo recrear conservando datos
`docker compose down` (sin -v) y luego `docker compose up -d`
