# Estructura del juego

Cosmo Kid queda separado en piezas para evitar tocar un archivo gigante en cada cambio.

- `game.html`: estructura de la pantalla del juego. Solo HTML y enlaces a CSS/JS.
- `assets/css/game.css`: estilos visuales del juego, HUD, portada interna, controles tactiles y fullscreen.
- `assets/js/game.js`: logica del juego: jugador, enemigos, camara, niveles, bosses, controles y render.
- `index.html`: portada/entrada directa al juego.
- `sw.js`: cache offline/PWA. Tocar cuando se cambian versiones o archivos cacheados.
- `manifest.webmanifest`: configuracion de instalacion como app.

Siguiente paso recomendado: dividir `assets/js/game.js` por sistemas cuando haya una mejora concreta, por ejemplo `camera`, `player`, `enemies`, `levels` y `ui`.
