# Portafolio · José Rayos

Marketing digital y performance · Ciudad de Panamá
Sitio: https://joserayos.github.io (inglés: https://joserayos.github.io/?lang=en)

## Cómo está armado

- `index.html`: toda la página (estilos, contenido y código en un solo archivo).
- `img/`: piezas por proyecto (`zews/`, `utopia/`, `anayansi/`, `jose-teng/`), portadas de artículos (`articulos/`), retrato, imagen para compartir (`og-jose-rayos.jpg`) e íconos.
- `cv/`: CV en español e inglés (PDF).
- `sitemap.xml` y `robots.txt`: para Google Search Console.

## Cómo actualizar

- **Nuevo artículo:** agrega un bloque al inicio de `ARTICLES` (título, fecha, tema, resumen, link y portada) y sube la portada a `img/articulos/`.
- **Nueva pieza:** agrégala a `pieces` del proyecto en `projects`, como `{type:'image'|'video'|'carousel', label, title, src | slides, ratio}`. Los videos llevan `sound:true` para mostrar el botón de sonido.
- **Videos:** `.mp4` de 720p, con audio, menos de 10 MB, con un póster `<nombre>-poster.webp` al lado.
- **Inglés:** los textos fijos están en `EN_UI` (por clave `data-i18n`) y los de proyectos y piezas en `EN` (texto en español → texto en inglés). Si cambias un texto en español, actualiza también su clave en `EN`.
- **CV:** reemplaza los PDF en `cv/` con el mismo nombre.

## Analítica

GoatCounter (sin cookies). Ya está instalado con el código `joserayos`; se activa al crear la cuenta en goatcounter.com con ese código. Registra visitas, casos abiertos, descargas de CV, clics en WhatsApp/correo y cambio de idioma.
