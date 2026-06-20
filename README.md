# Juan Crovatto — Static Site

Sitio estático en HTML/CSS/JS listo para subir a GitHub Pages.

## Estructura
- `index.html` — página principal (Tailwind vía CDN + fuentes Google)
- `images/` — imágenes (hero, bio, flyer, crowd)

## Publicar en GitHub Pages
1. Creá un repo nuevo en GitHub (por ejemplo `juan-crovatto`).
2. Subí todos los archivos de esta carpeta a la raíz del repo:
   ```bash
   git init
   git add .
   git commit -m "init"
   git branch -M main
   git remote add origin https://github.com/USUARIO/REPO.git
   git push -u origin main
   ```
3. En GitHub: **Settings → Pages → Source: Deploy from a branch → main / root → Save**.
4. En unos segundos vas a tener el sitio en `https://USUARIO.github.io/REPO/`.

## Notas
- Tailwind se carga desde el CDN (`cdn.tailwindcss.com`); no requiere build.
- Para producción seria, considerá compilar Tailwind con la CLI y reemplazar el `<script>` por un CSS estático.
