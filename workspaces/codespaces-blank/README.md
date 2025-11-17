# Expedición E‑R‑C: Dominio del Autocontrol

Pequeño micrositio interactivo (HTML estático) creado por Eduardo Javier Vogel.

Descripción
- Experiencia gamificada con 6 etapas para practicar autocontrol laboral.
- Está implementado como un único `index.html` con dependencias externas (Tailwind CDN, Chart.js, FontAwesome).

Cómo probar localmente
1. Abrir una terminal en la carpeta del proyecto (`/workspaces/codespaces-blank`).
2. Levantar un servidor HTTP simple (Python 3):

```bash
python3 -m http.server 8000
# luego abre http://localhost:8000 en tu navegador
```

Publicar en GitHub (resumen de comandos)
1. Inicializar, añadir y commitear:

```bash
git add .
git commit -m "Public: Expedición E-R-C - micrositio para Genially"
```

2. Crear repo público y hacer push (usando GitHub CLI `gh`):

```bash
# reemplaza <usuario> y <nombre-repo>
gh repo create <usuario>/<nombre-repo> --public --source=. --remote=origin --push
```

3. (Opcional) Activar GitHub Pages desde la rama `main` en Settings → Pages o usando `gh`.

URL para embeber en Genially
- Una vez publicada con Pages la URL será: `https://<usuario>.github.io/<nombre-repo>/`
- En Genially puedes embeber con un `iframe`:

```html
<iframe src="https://<usuario>.github.io/<nombre-repo>/" width="100%" height="600" frameborder="0" allowfullscreen></iframe>
```

Notas técnicas
- El proyecto carga recursos desde CDNs; no requiere build.
- Si necesitas persistencia (localStorage) u otros cambios, indícalo y puedo implementarlos.

Contacto
- Si quieres que yo (ahora) ejecute los comandos de `git`/`gh` en este Codespace, dímelo y lo intento (necesitarás haber autenticado `gh`).
Resumen

Este repositorio contiene una versión estática del "Tablero interactivo: Expedición E-R-C" lista para hospedar en GitHub Pages u otro hosting estático.

Archivos incluidos

- `index.html` — el micrositio completo (usa CDNs para Tailwind, Chart.js, Font Awesome y Google Fonts).

Dependencias externas (se cargan desde CDN)

- Tailwind CSS (cdn.tailwindcss.com)
- Chart.js (cdn.jsdelivr.net)
- Font Awesome (cdnjs)
- Google Fonts (fonts.googleapis.com)
- Fondo de Unsplash y videos embebidos (YouTube)

Opciones de publicación

1) GitHub Pages (recomendado)

- Inicializa el repositorio y haz push:

```bash
git init
git add .
git commit -m "Initial commit: Tablero interactivo"
git branch -M main
# Crear repo remoto y enviar (requiere gh CLI configurado o crea repo manualmente en github.com)
gh repo create <tu-usuario>/<nombre-repo> --public --source=. --remote=origin --push
```

- Luego en GitHub: `Settings > Pages` (o `Pages` en el nuevo menú) selecciona la rama `main` y la carpeta `/ (root)` y guarda. GitHub Pages publicará en `https://<tu-usuario>.github.io/<nombre-repo>/`.

2) Netlify (Drop)

- Comprime la carpeta en un ZIP y arrástrala a https://app.netlify.com/drop para publicar instantáneamente.

3) Alternativa de prueba local

```bash
# Servir localmente en puerto 8000
python3 -m http.server 8000
# Luego abre http://localhost:8000
```

Instrucciones para embeber en Genially

Consulta `GENIALLY.md` para pasos detallados y ejemplo de iframe.
