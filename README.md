# RE:SET · SYNC-01 · Experiencia AR

Página web de realidad aumentada (MindAR + A-Frame). La cámara reconoce las tres tarjetas de la carpeta `STICKERS` y sobre cada una reproduce el video de su chaqueta, con una barra "UPDATING" y un panel con la información de esa versión.

## Archivos

| Archivo | Qué es |
| --- | --- |
| `index.html` | La experiencia. El contenido de cada chaqueta está en el bloque `CHAQUETAS`, al inicio del script. |
| `targets.mind` | Las tres tarjetas compiladas para MindAR: 0 = DIARIO, 1 = INSTITUCIONAL, 2 = NATURALEZA. |
| `stickers/` | Miniaturas de las tarjetas para la pantalla de inicio y el modo sin cámara. |
| `videos/` | Aquí van los tres videos (ver abajo). |

## Cómo poner los videos

Guarda cada video en `videos/` con este nombre exacto:

- `videos/v1_diario.mp4`
- `videos/v2_institucional.mp4`
- `videos/v3_naturaleza.mp4`

Mientras falte un video, sobre la tarjeta aparece el aviso "[ VIDEO PENDIENTE ]" y la página sigue funcionando.

Formato recomendado para que cargue rápido en el celular: MP4 H.264, 4:3, 960 × 720, unos 8 MB como máximo. Con FFmpeg:

```
ffmpeg -i ENTRADA.mp4 -vf scale=960:720 -c:v libx264 -preset veryfast -crf 26 -c:a aac -b:a 96k -movflags +faststart videos/v1_diario.mp4
```

Si el video no es 4:3, cambia `VIDEO_AR.ancho` y la proporción en el script, o recórtalo a 4:3.

## Cómo probarla

La cámara solo funciona desde un enlace **https://**. Sube la carpeta completa a Netlify (arrastrar y soltar en app.netlify.com/drop) y abre el enlace en Chrome o Safari del celular. Para revisar los videos sin cámara, usa el botón "Ver sin cámara".

## Si cambias las tarjetas

Si editas cualquier sticker, hay que volver a compilar `targets.mind` con las tres imágenes en el mismo orden (DIARIO, INSTITUCIONAL, NATURALEZA), por ejemplo en el compilador web de MindAR.
