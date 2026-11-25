# RE:SET · SYNC-01 — Experiencia AR

**Una chaqueta. Tres versiones.**

RE:SET es una submarca de MOVink que imagina la ropa de 2036. Su primera prenda, la chaqueta inteligente **SYNC-01**, se carga sola con el sol y el movimiento, se adapta al clima y a los rayos UV, permite pagar con un toque y se personaliza cambiando sus módulos. La idea de la marca es simple: no compras ropa, compras una versión.

Esta experiencia de realidad aumentada te deja verlo con tu propio celular. Apunta la cámara a una de las tres tarjetas de RE:SET y la chaqueta se "actualiza" frente a ti, como si fuera un software, para mostrarte en video la versión que tienes en la mano.

> RE:SET SYNC-01 es un concepto de producto ficticio, creado como proyecto académico para la materia gerencia en diseño de la carrera profesional Diseño Digital y Multimedia.

## Qué vas a encontrar

| Tarjeta | Versión | Para qué es | Qué puede hacer |
| --- | --- | --- | --- |
| **DIARIO** | v2036.1 | La calle, la universidad, el trabajo y TransMilenio | Se carga con el sol y caminando, carga tu celular en el bolsillo del pecho, detecta el sol fuerte y te hace visible de noche con reflectivos y luces LED |
| **INSTITUCIONAL** | v2036.2 | El uniforme de una empresa o universidad | Lleva el escudo de la institución, te deja pagar o entrar con un toque del puño y tiene un pasaporte digital que cuenta de dónde viene la prenda y permite revenderla |
| **NATURALEZA** | v2036.3 | El páramo y los cerros | Tiene panel solar extra, capucha que se abre sola con el sol y mangas magnéticas que se quitan para convertirla en chaleco |

## Cómo usarla

1. Abre el enlace de la experiencia en Chrome o Safari desde tu celular.
2. Toca **Abrir cámara** y acepta el permiso de cámara.
3. Apunta a una de las tres tarjetas y enmárcala completa.
4. Mira cómo la chaqueta se actualiza y se reproduce su video.
5. En el panel de abajo puedes ver sus funciones, activar el sonido o abrir el video en pantalla completa.

¿No tienes las tarjetas a mano o tu celular no abre la cámara? Toca **Ver sin cámara** para ver los videos de las tres versiones.

## Uso de inteligencia artificial

El proyecto se hizo con apoyo de tres herramientas de inteligencia artificial. La dirección creativa, el concepto de producto y las decisiones de diseño son del equipo.

| Herramienta | Qué hizo |
| --- | --- |
| **Nano Banana** (Google) | Generó las imágenes: las vistas de las tres chaquetas, los renders de producto y los fotogramas de inicio y final de cada plano del video. |
| **MiniMax H3** | Generó los videos de cada plano a partir de esos fotogramas. Con ellos se armó el video de cada versión que aparece sobre las tarjetas. |
| **Claude y Claude Code** (Anthropic) | Diseñaron y programaron la interfaz web, organizaron la información de cada chaqueta a partir del guion y el brandbook, prepararon las tarjetas para que la cámara las reconozca y probaron la experiencia. |

## Tecnología

- [MindAR](https://github.com/hiukim/mind-ar-js) para reconocer las tarjetas con la cámara.
- [A-Frame](https://aframe.io) para mostrar el contenido en realidad aumentada.
- Una página web en HTML, CSS y JavaScript: no necesitas instalar ninguna app.

## Identidad visual

Fondo Void `#0B0B0F`, texto Chrome `#D9DCE3` y un solo neón por versión: Reboot Lime `#C6FF3D` para DIARIO, Chrome sin neón para INSTITUCIONAL y naranja `#FF7828` para NATURALEZA. Los titulares usan Unbounded y los datos, JetBrains Mono.

---

**RE: SET** · por MOVink — Tu ropa, reiniciada.
