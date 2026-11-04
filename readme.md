# InterBiz · Inteligencia de Exportación

Prototipo Fase 2 del proyecto InterBiz 2035. Consultor de exportación + simulador de decisiones para comercio exterior colombiano.

## Stack

- Frontend: HTML + JS vanilla (SPA con hash routing)
- Datos: JSON en el repo
- Hosting: Cloudflare Pages (gratis, comercial OK)
- CMS: Decap CMS (opcional, para edición visual)
- Costo operativo: $0/mes

## Quick start

### 1. Crear repo

En GitHub: New repo → "interbiz" → Public → sin README.

### 2. Deploy en Cloudflare Pages

1. Entra a https://dash.cloudflare.com → Workers & Pages → Create → Pages → Connect to Git.
2. Autoriza Cloudflare a ver tu GitHub.
3. Selecciona el repo `interbiz`.
4. Configuración:
   - Project name: `interbiz`
   - Production branch: `main`
   - Framework preset: `None`
   - Build command: (vacío)
   - Build output directory: `public`
5. Save and Deploy.

En ~30 segundos tu app está en `https://interbiz.pages.dev`.

### 3. Editar datos

Opción A — GitHub web (recomendado para MVP):
1. Ve a `public/data/products.json` en tu repo.
2. Click en el lápiz ✏️.
3. Edita el JSON.
4. Commit changes.
5. Cloudflare re-deploya en 30 segundos.

Opción B — Decap CMS (requiere OAuth de GitHub):
1. Sigue la guía: https://decapcms.org/docs/github-backend/
2. Una vez configurado, ve a `https://interbiz.pages.dev/admin/`.
3. Login con GitHub y edita visualmente.

## Estructura
