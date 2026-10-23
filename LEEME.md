# Invitación de cumpleaños · Nathan León

Una sola página (`index.html`) con sobre animado, cuenta regresiva, calendario, mapa, marcos de fotos y confirmación de asistencia.

## 1. Archivos

```
tu-carpeta/
├── index.html
├── LEEME.md
└── assets/
    ├── foto1.jpg   foto2.jpg   foto3.jpg      ← fotos de Nathan
    ├── osito-portada.png                      ← tus dibujos (opcionales)
    ├── osito-bebe.png
    ├── osito-asoma.png
    ├── osito-globo.png
    ├── osito-duerme.png
    ├── osito-saluda.png
    └── osito-final.png
```

Reglas de nombres: todo en **minúsculas**, sin espacios, con la extensión exacta (`.jpg` para fotos, `.png` para dibujos).

## 2. Estructura de la invitación (de arriba a abajo)

| # | Sección | Qué contiene | Imagen que usa |
|---|---|---|---|
| 1 | Portada | Nombre, fecha en pastilla roja, tarro de miel que se toca para abrir | `osito-portada.png` |
| 2 | Frase de bienvenida | Texto `cita` | — |
| 3 | "1 añito" | Hexágono de miel | — |
| 4 | Pose bebé | Osito con chupón o pañal | `osito-bebe.png` |
| 5 | Marco de foto 1 | Marco con adornos de fiesta | `foto1.jpg` + `osito-asoma.png` |
| 6 | ¡Prepárate! | Osito con globo y cuenta regresiva | `osito-globo.png` |
| 7 | Guarda la fecha | Calendario del mes, osito dormido, botón "Añadir al calendario" | `osito-duerme.png` |
| 8 | Marco de foto 2 | Marco con estrella, regalo y abeja | `foto2.jpg` |
| 9 | ¿Dónde? | Osito saludando, mapa, botones Google Maps y Waze | `osito-saluda.png` |
| 10 | Marco de foto 3 | Marco con gorro, regalo y flor | `foto3.jpg` + `osito-asoma.png` |
| 11 | Asistencia | Formulario que abre WhatsApp | — |
| 12 | Despedida | Osito con gorro y mensaje final | `osito-final.png` |

`osito-asoma.png` se usa en los marcos 1 y 3.

## 3. Cómo meter tus propios diseños

1. Crea tu imagen en **PNG con fondo transparente**, de unos 600 a 800 px de ancho y con el personaje centrado.
2. Guárdala en `assets/` con el nombre exacto de la tabla.
3. Sube o recarga la página. Ya trae las animaciones puestas, tú solo cambias la imagen.
4. Si un archivo no existe, la invitación muestra automáticamente un osito original de respaldo.

Poses recomendadas para cada archivo:

- `osito-portada.png`: abrazando el tarro de miel.
- `osito-bebe.png`: sentado, con chupón o pañal.
- `osito-asoma.png`: solo cabeza y patitas, recortado abajo.
- `osito-globo.png`: sosteniendo un globo.
- `osito-duerme.png`: dormido, abrazando el tarro.
- `osito-saluda.png`: saludando.
- `osito-final.png`: brazos arriba, con gorrito de fiesta.

Animaciones que ya trae cada uno:

- **Portada:** respira, y salta al tocar el tarro.
- **Bebé y final:** rebotan.
- **Asoma:** sube y baja.
- **Globo:** se mece.
- **Duerme:** respira, con "z z" flotando.
- **Saluda:** se balancea.

Usa solo imágenes que tengas derecho a usar. Esa responsabilidad es tuya.

## 4. Qué debes cambiar (al inicio de `index.html`, en `const C`)

| Campo | Qué poner |
|---|---|
| `lugar.nombre` | Nombre del salón o lugar |
| `limite` | Fecha límite para confirmar |
| `whatsapp` | Número con código de país, ej. `5215512345678` |
| `fotos[].pie` | Texto bajo cada foto |
| `cita` y `cierre` | Mensajes de bienvenida y despedida |

Ya están puestos: nombre, fecha (6 nov 2026, 4:00 PM), duración de 5 horas y ubicación del mapa.

## 5. Colores

Están en `:root`, al inicio del bloque de estilos:

- `--rojo`: acentos rojos.
- `--miel` y `--miel2`: amarillos.
- `--cafe` y `--cafe2`: textos.
- `--crema` y `--papel`: fondos.

## 6. Invitaciones personalizadas

Agrega el nombre al enlace y aparecerá en la portada y en el formulario:

```
https://tu-sitio.com/?invitado=Familia%20Pérez
```

## 7. Publicar

Sube **`index.html` y la carpeta `assets` completa** a GitHub Pages, Netlify u otro hosting. Si solo envías el archivo por chat, las imágenes no viajan con él.

## 8. Si una imagen no aparece

1. Revisa que esté en `assets/`, junto a `index.html`.
2. Revisa el nombre exacto, en minúsculas y sin espacios.
3. Revisa la extensión: `.png` para dibujos y `.jpg` para fotos.
4. Si lo publicaste, confirma que subiste la carpeta `assets`.
5. Recarga forzada o ventana privada, por la caché.
