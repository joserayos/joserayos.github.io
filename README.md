# Portafolio · José Rayos

Marketing digital y performance · Ciudad de Panamá
Sitio: https://joserayos.github.io (inglés: https://joserayos.github.io/?lang=en)

## Cómo está armado

- `index.html`: toda la página (estilos, contenido y código en un solo archivo).
- `img/`: piezas por proyecto (`zews/`, `utopia/`, `anayansi/`, `jose-teng/`), portadas de artículos (`articulos/`), retrato, imagen para compartir (`og-jose-rayos-v2.jpg`) e íconos.
- `cv/`: CV en español e inglés (PDF).
- `sitemap.xml` y `robots.txt`: para Google Search Console.

## Cómo actualizar

- **Nuevo artículo:** agrega un bloque al inicio de `ARTICLES` (título, fecha, tema, resumen, link y portada) y sube la portada a `img/articulos/`.
- **Nueva pieza:** agrégala a `pieces` del proyecto en `projects`, como `{type:'image'|'video'|'carousel', label, title, src | slides, ratio}`. Los videos llevan `sound:true` para mostrar el botón de sonido.
- **Videos:** `.mp4` de 720p, con audio, menos de 10 MB, con un póster `<nombre>-poster.webp` al lado.
- **Inglés:** los textos fijos están en `EN_UI` (por clave `data-i18n`) y los de proyectos y piezas en `EN` (texto en español → texto en inglés). Si cambias un texto en español, actualiza también su clave en `EN`.
- **CV:** reemplaza los PDF en `cv/` con el mismo nombre.

## Telón de entrada y retrato flotante

- **Telón:** paneles naranjas que se abren y dejan ver el inicio (marcado en `.curtain`, lógica al final del `<script>`). Se muestra una vez por sesión; con `?intro` en la dirección se fuerza para verlo de nuevo. No aparece con "reducir movimiento" ni cuando la dirección trae un ancla (`#perfil`). Se salta con un clic, un toque o `Esc`.
- **Retrato flotante (`.fab`):** círculo con el retrato fijo abajo a la derecha. Aparece al bajar medio pantallazo, se achica mientras se baja, muestra la sección actual y abre un menú con correo, WhatsApp y CV. Los textos están en `EN_UI` (`skipIntro`, `fabLabel`) y en `FAB_T` (burbuja).

## Analítica

GoatCounter (sin cookies). Ya está instalado con el código `joserayos`; se activa al crear la cuenta en goatcounter.com con ese código. Registra visitas, casos abiertos, descargas de CV, clics en WhatsApp/correo y cambio de idioma.
