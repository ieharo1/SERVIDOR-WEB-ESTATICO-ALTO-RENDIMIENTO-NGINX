# Servidor Web Estático de Alto Rendimiento con Nginx

Infraestructura de despliegue para frontend estático con enfoque en velocidad, cache agresiva y compresión en entorno Linux containerizado.

## Descripción

Este servidor está pensado para publicar sitios HTML/CSS/JS con comportamiento de SPA y optimización de assets para producción.

## ¿Qué hace este proyecto?

- Sirve contenido estático desde Nginx en imagen ligera Alpine.
- Aplica compresión gzip para mejorar tiempos de respuesta.
- Configura cache de larga duración para assets estáticos.
- Implementa fallback de SPA con `try_files`.

## Características Principales

| Característica | Descripción |
|---|---|
| Entrega estática | Publicación de frontend sin runtime extra |
| Gzip habilitado | Reduce tamaño de transferencia |
| Cache inteligente | `Cache-Control immutable` en assets |
| SPA fallback | Soporte para rutas internas frontend |

## Stack Tecnológico

- Nginx 1.27 (alpine)
- Docker
- Docker Compose

## Instalación y Uso

### Levantar entorno

```bash
docker compose up -d --build
```

### Probar

- URL: `http://localhost:8081`

## Variables de Entorno

- `NGINX_PORT`: puerto local para exponer el servicio.

## Estructura del Proyecto

```text
.
├── Dockerfile
├── docker-compose.yml
├── .env
├── app/
│   └── index.html
└── nginx/
    └── default.conf
```

## Casos de Uso

- Landing pages de alto tráfico.
- Sitios corporativos estáticos.
- Frontends SPA desacoplados de APIs externas.

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
