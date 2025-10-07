# PropertyHub Infra

Repositorio de **infraestructura** para levantar el proyecto completo **PropertyHub**, compuesto por:

- **api/** → backend .NET + MongoDB
- **web/** → frontend Vite/React
- **mongo** → base de datos (solo uso interno, no expuesta)

---

## Notas para clonar (usa submódulos)

> Este proyecto utiliza **submódulos de Git**.  
> Si no los inicializas, las carpetas `api/` y `web/` aparecerán vacías.

### Opción 1 — Clonar con submódulos directamente

```bash
git clone --recurse-submodules https://github.com/CarlosArguello/realty-hub-infra.git
cd realty-hub-infra
```

### Opción 2 — Si ya clonaste sin submódulos

```bash
git submodule update --init --recursive
```

## Levantar el entorno con Docker Compose

### Sin “daemon”

```bash
docker compose up --build
```

### Con “daemon”

```bash
docker compose up -d --build
```
