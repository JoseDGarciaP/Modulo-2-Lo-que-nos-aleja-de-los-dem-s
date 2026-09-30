# 🐸 Froggy Jumps · Módulo 2

Minijuego de preguntas del Módulo 2: *"Lo que nos aleja de los demás. ¿Por qué a veces nos cuesta conectar?"*. La rana salta de nenúfar en nenúfar con cada respuesta.

## Cómo se juega

- El jugador escribe su nombre al inicio.
- 10 preguntas en orden aleatorio (el texto de preguntas y respuestas es el original).
- Empieza con 100 puntos; cada error resta 100/10 (10 puntos). Un solo intento por pregunta.
- Al final aparece una tarjeta con nombre, fecha, aciertos, fallos, puntaje, **ID de partida** y **código de verificación**. El estudiante le toma pantallazo y lo envía por Teams.

## Integridad de los resultados

- No hay botones para borrar el historial, descargarlo ni cambiar puntos.
- Las respuestas correctas no están escritas en el código: se validan con un hash.
- El estado del juego es privado y no se puede modificar desde la consola del navegador.
- La partida se registra desde que empieza. Si el jugador recarga o cierra la página a mitad de juego, queda como **Incompleta** con los aciertos y fallos que llevaba.
- Cada registro del historial va firmado. Si alguien lo edita por fuera, aparece como **⚠ Alterado**.
- **`verificar.html`**: página para el docente. Se copian el nombre, el ID, los aciertos, los fallos y el código del pantallazo; si alguien editó la imagen, el código no coincide.

> Límite: es un juego 100 % estático en el navegador (GitHub Pages). Estas medidas impiden los cambios fáciles y detectan pantallazos editados, pero alguien con conocimientos avanzados de programación podría estudiar el código. Para una evaluación de alto impacto se necesitaría un servidor.

## Publicar gratis en GitHub Pages

1. Sube `index.html`, `verificar.html` y este `README.md` a la raíz del repositorio (rama `main`).
2. Ve a **Settings → Pages**. En *Source* elige **Deploy from a branch**, rama **main**, carpeta **/ (root)** → **Save**.
3. Espera 1–2 minutos. Los enlaces serán:
   - Juego: `https://TU-USUARIO.github.io/Modulo-2-Lo-que-nos-aleja-de-los-dem-s/`
   - Verificador: `https://TU-USUARIO.github.io/Modulo-2-Lo-que-nos-aleja-de-los-dem-s/verificar.html`
