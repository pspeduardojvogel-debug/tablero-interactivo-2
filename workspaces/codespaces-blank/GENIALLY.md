Cómo insertar este micrositio en Genially

Opción recomendada: hospedar y embeber vía iframe (permite mantener interactividad y JavaScript completo).

1) Hospeda el sitio (GitHub Pages recomendado)

- Publica `index.html` usando GitHub Pages o Netlify (ver README.md).
- Obtén la URL pública, por ejemplo: `https://<tu-usuario>.github.io/<nombre-repo>/`.

2) En Genially (editor)

- Abre tu proyecto en Genially y entra en modo edición.
- En el menú izquierdo selecciona "Insertar" > "Insertar código/iframe" (o "Website" según versión).
- Pega este iframe (ajusta `width`/`height` si lo necesitas):

```html
<iframe src="https://<tu-usuario>.github.io/<nombre-repo>/" width="100%" height="700" frameborder="0" allowfullscreen></iframe>
```

- O sólo pega la URL en la opción "Insertar > Website/Enlace" si Genially solicita una URL.

Requisitos y notas

- Debe servir sobre HTTPS (GitHub Pages y Netlify usan HTTPS por defecto).
- El sitio no debe enviar un encabezado `X-Frame-Options: DENY` ni `Content-Security-Policy` que impida iframes. GitHub Pages permite embeber en iframes.
- Recursos externos (CDNs, YouTube, Google Fonts) funcionan normalmente si la página se sirve vía HTTPS.

Alternativa si prefieres no hospedar

- Puedes subir los assets (imágenes, HTML) directamente a Genially si la cuenta/plan lo permite, pero Genially no permite ejecutar HTML+JS arbitrario dentro de su entorno — por eso la opción iframe es la más fiable.

¿Quieres que yo publique esto en GitHub Pages por ti?

Puedo hacerlo si me confirmas:
- El nombre del repositorio a crear (ej: `expedicion-erc`)
- Si quieres que lo haga público o privado (recomendado público para Pages)

Si me autorizas usar `gh` en este entorno, puedo crear el repo y hacer push, y te daré la URL lista para embeber.