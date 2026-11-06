# Jugar en paz · instrucciones para WordPress

Hola. Ramón quiere poner en la web principal (`www.ramonromeroboquete.com`, en WordPress) la página **«Jugar en paz»**. Es **temporal**: cuando esté en marcha el subdominio `jugar.ramonromeroboquete.com` (Vercel, conectado al repositorio de GitHub `beforget-plataforma/culturaventas`), Ramón te avisará para quitarla.

## Archivo

`jugar-en-paz-wordpress.html` es un bloque de HTML autónomo:

- Todos los estilos están **aislados** dentro de `.rrb-jugar`, así que no tocan el tema y el tema apenas los toca a ellos.
- No lleva JavaScript.
- Solo carga las fuentes Oswald y DM Sans de Google Fonts.
- Va sin barra de navegación propia: usa la cabecera de WordPress.

## Cómo instalarlo

1. Crea una página nueva llamada «Jugar en paz», o usa la página que Ramón indique, por ejemplo la portada.
2. Plantilla: **ancho completo / sin barra lateral / sin título** (el nombre depende del tema, por ejemplo «Full width», «Canvas» o «Blank»). La página tiene su propio fondo oscuro y su propio titular.
3. Añade un bloque **«HTML personalizado»** y pega **el archivo completo**.
4. Si usas Elementor u otro maquetador: un widget «HTML» dentro de una sección de ancho completo, con el relleno de la sección a 0.
5. Si hay un plugin de caché o de optimización (WP Rocket, Autoptimize, LiteSpeed…), vacía la caché. Comprueba también que no elimine la etiqueta `<style>` del bloque.

## Qué comprobar

- Que el fondo oscuro llegue de borde a borde. Si queda un margen blanco, el contenedor del tema tiene `max-width` o `padding`: usa una plantilla de ancho completo.
- Que en el móvil (unos 390 px de ancho) no haya desplazamiento horizontal.
- Que los enlaces funcionen:
  - «Leer el manifiesto completo» → `https://jugar.ramonromeroboquete.com/manifiesto/`. Este enlace **no funcionará hasta que exista el subdominio**. Hasta entonces, si Ramón lo prefiere, cámbialo por la URL de la página de WordPress donde esté el manifiesto.
  - Newsletter → `https://www.beforget.com/letter/`
  - YouTube → `https://www.youtube.com/@ramonromeroboquete`
  - Reunión de los miércoles (Zoom) y WhatsApp.

## Para quitarlo más adelante

Borra el bloque, o la página, y redirige su URL a `https://jugar.ramonromeroboquete.com/` (301).

## Cambios de texto

La versión original vive en GitHub, en `index.html` del repositorio. Si Ramón cambia algún texto, se actualiza allí y se regenera este bloque. Evita editarlo a mano en WordPress, para que las dos versiones no se separen.
