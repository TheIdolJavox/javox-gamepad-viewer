# JAVOX — CSS para GamePad Viewer (PS4 / DS4)

Repositorio: [github.com/TheIdolJavox/javox-gamepad-viewer](https://github.com/TheIdolJavox/javox-gamepad-viewer)

Tema con fondo negro, acentos cian (`#00FFC8`), texto **JAVOX** estilo LED y hueco para tu logo.

## URLs del CSS (elige una)

**1. GitHub Raw** (a veces tu operador o red guardan en caché una versión vieja):

```
https://raw.githubusercontent.com/TheIdolJavox/javox-gamepad-viewer/main/javox-ds4.css
```

**2. jsDelivr** (mismo archivo, otra CDN; suele funcionar si Raw te muestra código antiguo con `filter:` en `.controller.ds4`):

```
https://cdn.jsdelivr.net/gh/TheIdolJavox/javox-gamepad-viewer@main/javox-ds4.css
```

**Cómo saber que es la versión correcta:** al abrir el enlace debe aparecer el comentario *«NO usar filter en .controller.ds4»* y la regla **`.controller.ds4 { position: relative; box-shadow: … }`**. Si ves **`filter: saturate`** ahí, es caché: prueba jsDelivr, datos móviles u otra red.

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

En **Edit CSS URL** pega la URL de **jsDelivr** o la **Raw** (la que en tu navegador muestre la versión sin `filter` en el mando).

## OBS

Fuente **Navegador**: pega la URL final generada por GamePad Viewer y ajusta ancho/alto hasta que el mando se vea bien.

## Si el mando sale “arriba” o recortado en la vista previa

El skin base de GamePad Viewer centra el DS4 con `position: absolute` y `transform`. **No uses `position: relative` en `.controller.ds4`** (rompe ese centrado). Este tema ya evita eso.

## Si el mando “desaparece” en la beta

- Asegúrate de tener la última versión de este CSS (evitamos `filter` en todo el mando: en algunos navegadores el control deja de dibujarse).
- Abre en el navegador la URL Raw del CSS: debe mostrarse texto CSS, no error 404.
- Si sigue fallando solo en la beta, prueba la vista clásica con el mismo CSS:  
  [gamepadviewer.com con tu skin](https://gamepadviewer.com/?p=1&css=https%3A%2F%2Fraw.githubusercontent.com%2FTheIdolJavox%2Fjavox-gamepad-viewer%2Fmain%2Fjavox-ds4.css)
