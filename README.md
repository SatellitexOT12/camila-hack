# camila-hack 🎁

Experiencia web de una sola página para el cumpleaños de Camila: lluvia 0/1 estilo
*Matrix*, un mensaje **«Has sido hackeada»** y un sudoku fácil que, al resolverse,
detiene el "hack" y revela **¡Feliz cumpleaños, Camila!**

## Cómo funciona

1. **Lluvia 0/1** — lluvia de dígitos binarios sobre canvas + consola tecleando;
   la línea se desencripta hasta **«HAS SIDO HACKEADA»**. (Se puede acelerar con un clic.)
2. **Módulo de defensa** — sudoku de 9×9 con 45 pistas (solución única, resoluble
   solo con singles). Teclado con flechas y dígitos, retroceso, **PISTA** y
   **RENDIRSE** con doble confirmación (camino alternativo: nunca hay callejón sin salida).
3. **Revelación** — las fichas del tablero vuelan y los dígitos se destraban
   carácter a carácter hasta el saludo completo + botón para reiniciar. La lluvia
   del fondo se enmascara con el nombre **CAMILA** detrás del saludo.

**Trucos ocultos:** durante la intro, teclea en el teclado físico `help`, `hola`,
`cumples` o `camila` y la consola responde. Al ganar verás tus estadísticas
(`hackeada en 3m 42s · sin pistas · sin rendirse`) y tu récord se guarda en el
navegador (`localStorage`) para batirlo en la siguiente partida.

## Detalles técnicos

- Una sola página: `index.html` con CSS y JS en línea. Sin dependencias, sin backend.
- Fuentes auto-alojadas (woff2) en `assets/fonts/`: VT323 + IBM Plex Mono.
- Respeta `prefers-reduced-motion` (sin lluvia ni partículas con animación reducida).
- Diseñado móvil primero: funciona de 360px en adelante, sin desbordamiento horizontal.
- Funciona sin conexión una vez cargado (todo inline + fuentes locales).

## Ejecutar en local

Para que carguen las fuentes, sirve el directorio con cualquier servidor estático:

```bash
npx serve .
# o
python -m http.server 8000
```

y abre `http://localhost:8000`.

## Publicación (GitHub Pages)

Publicado desde la rama `main`, raíz `/` (`.nojekyll` incluido). Cualquier push a
`main` actualiza el sitio en `https://<usuario>.github.io/camila-hack/`.

## Estructura

| Ruta | Contenido |
|---|---|
| `index.html` | El sitio completo (HTML + CSS + JS) |
| `assets/fonts/` | Fuentes woff2 auto-alojadas |
| `DESIGN.md` | Sistema de diseño derivado del artefacto |
| `PRODUCT.md` | Registro de producto |
