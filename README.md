# JAVOX — CSS para GamePad Viewer (PS4 / DS4)

Repositorio: [github.com/TheIdolJavox/javox-gamepad-viewer](https://github.com/TheIdolJavox/javox-gamepad-viewer)

Tema con fondo negro, acentos cian (`#00FFC8`), texto **JAVOX** estilo LED y hueco para tu logo.

## URLs del CSS (elige una)

**1. GitHub Raw** (a veces tu operador o red guardan en caché una versión vieja):

```
https://raw.githubusercontent.com/TheIdolJavox/javox-gamepad-viewer/main/javox-ds4.css
```

**2. jsDelivr** (`@main` a veces va **retrasado** respecto a GitHub; si no ves la última versión, purga la caché):

```
https://cdn.jsdelivr.net/gh/TheIdolJavox/javox-gamepad-viewer@main/javox-ds4.css
```

Abre una vez en el navegador (o usa GET) la URL de purga de jsDelivr y luego recarga el CSS:

```
https://purge.jsdelivr.net/gh/TheIdolJavox/javox-gamepad-viewer@main/javox-ds4.css
```

**3. Raw con anti-caché** (útil en tu red):

```
https://raw.githubusercontent.com/TheIdolJavox/javox-gamepad-viewer/main/javox-ds4.css?nocache=1
```

**Cómo saber que es la versión nueva:** el comentario debe incluir **`build: safe-base-v2`** (o superior). Si el mando se ve “por defecto” o mal centrado, suele ser **caché de jsDelivr** con un CSS viejo: usa la **URL con commit** de abajo o purga.

**URL fija al último commit** (sustituye `COMMIT` por el hash corto del último commit en GitHub → botón verde “<> Code” → copiar SHA):  
`https://cdn.jsdelivr.net/gh/TheIdolJavox/javox-gamepad-viewer@COMMIT/javox-ds4.css`

## Usar en GamePad Viewer (clásico)

En [gamepadviewer.com](https://gamepadviewer.com/), en el generador, pega la URL **Raw** anterior en el campo de CSS personalizado, o usa una URL directa como:

Con Raw:

```
https://gamepadviewer.com/?p=1&css=https%3A%2F%2Fraw.githubusercontent.com%2FTheIdolJavox%2Fjavox-gamepad-viewer%2Fmain%2Fjavox-ds4.css
```

Con jsDelivr:

```
https://gamepadviewer.com/?p=1&css=https%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2FTheIdolJavox%2Fjavox-gamepad-viewer%40main%2Fjavox-ds4.css
```

(`p=1` es el jugador 1; cámbialo si muestras otro mando.)

## Beta (beta.gamepadviewer.com)

En **Edit CSS URL** pega la **Raw** (con `?nocache=1` si hace falta) o **jsDelivr** después de **purgar** si `@main` te muestra código viejo. Comprueba en el navegador que ves **`build: visible-accents`** antes de pegarla en GPV.

## OBS

Fuente **Navegador**: pega la URL final generada por GamePad Viewer y ajusta ancho/alto hasta que el mando se vea bien.

## Si el mando sale “arriba” o recortado en la vista previa

El skin base de GamePad Viewer centra el DS4 con `position: absolute` y `transform`. **No uses `position: relative` en `.controller.ds4`** (rompe ese centrado). Este tema ya evita eso.

## Si el mando “desaparece” en la beta

- Asegúrate de tener la última versión de este CSS (evitamos `filter` en todo el mando: en algunos navegadores el control deja de dibujarse).
- Abre en el navegador la URL Raw del CSS: debe mostrarse texto CSS, no error 404.
- Si sigue fallando solo en la beta, prueba la vista clásica con el mismo CSS:  
  [gamepadviewer.com con tu skin](https://gamepadviewer.com/?p=1&css=https%3A%2F%2Fraw.githubusercontent.com%2FTheIdolJavox%2Fjavox-gamepad-viewer%2Fmain%2Fjavox-ds4.css)
