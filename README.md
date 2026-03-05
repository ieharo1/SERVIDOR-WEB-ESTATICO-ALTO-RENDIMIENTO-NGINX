# Art - Static Site Production Profile

Este repo ahora muestra un despliegue de frontend estatico con Nginx optimizado para cache y compresion.

## Arquitectura

- `Dockerfile`: imagen ligera sobre `nginx:alpine`.
- `docker-compose.yml`: levanta un servicio de Nginx listo para publicar.
- `.env`: define el puerto publico.
- `nginx/default.conf`: SPA fallback, cache de assets y gzip.

## Levantar el proyecto

```bash
docker compose up -d --build
```

Abrir: `http://localhost:8081`

## Variables a cambiar

- `NGINX_PORT`: puerto local para exponer el contenedor.

## Archivos clave

- `Dockerfile`
- `docker-compose.yml`
- `.env`
- `nginx/default.conf`
- `app/index.html`

---

## ‍ Desarrollado por Isaac Esteban Haro Torres

**Ingeniero en Sistemas · Full Stack · Automatización · Data**

-  Email: zackharo1@gmail.com
-  WhatsApp: 098805517
-  GitHub: https://github.com/ieharo1
-  Portafolio: https://ieharo1.github.io/portafolio-isaac.haro/

---

##  Licencia

© 2026 Isaac Esteban Haro Torres - Todos los derechos reservados.
