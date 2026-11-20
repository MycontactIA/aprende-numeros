# Aprende los números

Juego para practicar la escritura de números con el dedo índice, frente a la cámara.

## Cómo se juega

1. Elige el idioma (Español, English o Français).
2. Pulsa **Empezar** y permite el uso de la cámara.
3. Traza con el dedo índice el número que aparece en pantalla. Cuando cubres la mayor parte de la forma, el número se completa.
4. Al completarlo, suena una recompensa al azar y el juego pronuncia el número en el idioma elegido.

Niveles: 0–10, 11–20, 40–100 (de 20 en 20), 150–500 (de 50 en 50) y 600–1000 (de 100 en 100).

## Privacidad

- La cámara se procesa en tu navegador. El video no se envía ni se guarda en ningún servidor.
- El detector de manos (MediaPipe) y su modelo se descargan desde CDN públicos la primera vez.
- La pronunciación usa las voces del sistema operativo y del navegador.

## Uso local

Los navegadores bloquean la cámara en `file://`. Para probarlo en tu equipo:

```
python3 -m http.server 8000 --bind 127.0.0.1
```

Abre `http://127.0.0.1:8000` y recarga con Cmd+Shift+R si hace falta.

## Modo de depuración

Con `?debug` en la dirección, la página expone `window.__dbg` (simular la punta del dedo, completar un número y leer el registro de eventos). No se activa en el uso normal.

## Limitaciones conocidas

- El juego no exige un orden de trazo; basta con cubrir la forma del número.
- La detección depende de la luz y de la cámara. Se probó en un entorno sin cámara real.
