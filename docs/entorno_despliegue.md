# Entorno de Despliegue – SIGA
## Objetivo
Documentar la configuración del entorno de ejecución y despliegue para mantener consistencia entre los integrantes del equipo.
## Variables de entorno
| Variable | Descripción |
|---|---|
| DATABASE_URL | Cadena de conexión a PostgreSQL. |
| JWT_SECRET | Clave para firmar los tokens de autenticación. |
| PORT | Puerto de ejecución del backend. |
## Docker
- Dockerfile para el backend (Node.js).
- docker-compose para levantar backend + PostgreSQL.
- Variables sensibles gestionadas mediante archivo .env (no versionado).
## Notas
Configuración orientada a entornos de despliegue consistentes y seguros, evitando exponer credenciales en el repositorio.
