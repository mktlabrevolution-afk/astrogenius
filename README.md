# astrogenius

Repositorio para el sitio dinámico "astrogenius".

Instrucciones rápidas (en español):

1) Instalar dependencias

```bash
npm install
```

2) Hacer build (ajusta según tu framework):

- Create React App: `npm run build` (publica la carpeta `build`)
- Vue CLI: `npm run build` (publica `dist`)
- Gatsby: `gatsby build` (publica `public`)
- Next.js (export estático): `next build && next export` (publica `out`)
- Sitio estático: no hace falta build; publica la carpeta raíz o `public`

3) Subir cambios a GitHub (si trabajas localmente):

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/mktlabrevolution-afk/astrogenius.git
git push -u origin main
```

4) Despliegue en Netlify:

- En Netlify: "Add new site" → "Import from Git" → conectar con GitHub → seleccionar este repo.
- Configurar: Branch = main, Build command = (ej.: `npm run build`), Publish directory = (ej.: `build`, `dist`, `public` o `out`).
- Guardar y desplegar.

5) Variables de entorno y claves

Agrega las claves/API en Netlify → Site settings → Build & deploy → Environment.

Notas:
- Si tu proyecto usa server-side rendering (por ejemplo Next.js sin export), revisa compatibilidad con Netlify o usa Vercel. También puedes adaptar a funciones serverless y Netlify Functions.
- Para funciones serverless, coloca lambdas en `netlify/functions`.

---
Archivos añadidos por el asistente para facilitar el primer despliegue en Netlify.
