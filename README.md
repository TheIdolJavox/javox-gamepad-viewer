# JAVOX — CSS para GamePad Viewer (PS4 / DS4)

Tema con fondo negro, acentos cian (`#00FFC8`), texto **JAVOX** estilo LED y hueco para tu logo.

El logo ya está en `assets/logo.png`; el CSS lo referencia con una ruta relativa (correcta al servir el `.css` desde GitHub Raw).

## Usar en GamePad Viewer (clásico)

En [gamepadviewer.com](https://gamepadviewer.com/), genera una URL que incluya el parámetro `css` apuntando al archivo **raw** de este repositorio:

`https://gamepadviewer.com/?p=1&css=URL_ENCODED_DEL_CSS_RAW`

La URL del CSS debe ser HTTPS y ser el enlace “Raw” de GitHub (no la página HTML del archivo).

## Beta (beta.gamepadviewer.com)

Si el builder te deja pegar CSS o enlazar una hoja externa, usa la misma URL raw del `javox-ds4.css`.

## OBS

Fuente **Navegador**: pega la URL final generada por GamePad Viewer y ajusta ancho/alto hasta que el mando se vea bien.
