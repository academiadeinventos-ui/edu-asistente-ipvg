# Edu · Asistente virtual del IP Virginio Gómez 🤖🎓

**Edu** es un asistente virtual con IA (Gemini 2.0 Flash de Google) para el Instituto Profesional Dr. Virginio Gómez de Chile. Tiene rostro animado, voz en español de Chile, reconocimiento de voz y soporte para cámara (puede describir lo que ve).

🔗 **Demo en vivo:** https://academiadeinventos-ui.github.io/edu-asistente-ipvg/

## Características
- 🤖 **IA real** con Google Gemini 2.0 Flash (respuestas inteligentes, no solo reglas fijas).
- 🗣️ **Voz** en español chileno (síntesis de voz del navegador) + animación de boca sincronizada.
- 🎤 **Reconocimiento de voz** (habla y Edu te responde hablando).
- 📷 **Cámara** (Edu puede verte y describir lo que ve, gracias a la visión de Gemini).
- 🌗 Tema claro/oscuro automático.
- 📱 Diseño responsive (se ve bien en celular).
- 👀 Ojos que siguen el cursor, parpadeo y animaciones.
- 💬 Respuestas con markdown ligero (negritas, listas).
- 📋 Botón de copiar en cada mensaje.
- 🧹 Botón para limpiar la conversación.
- ⌨️ Enter para enviar, Shift+Enter para salto de línea.

## Cómo usarlo
1. Abre el sitio web.
2. La primera vez, pega tu API key de Google Gemini (es **gratuita**).
   - Ve a https://aistudio.google.com/apikey
   - Inicia sesión con tu cuenta de Google
   - Haz clic en "Create API Key" → copia la clave que empieza por `AIza...`
   - Pégala en el cuadro de diálogo de Edu.
3. Tu clave se guarda solo en tu navegador (localStorage), nunca en ningún servidor.
4. Si no quieres usar IA real, puedes usar el modo de respuestas básicas.

## ¿Por qué pedir una API key propia?
El plan gratuito de Gemini permite ~15 solicitudes por minuto y un millón+ de tokens al mes, más que suficiente para un asistente educativo. Cada visitante usa su propia clave, así que el asistente escala sin costos para quien lo publica.

## Publicación con GitHub Pages
Este repositorio usa un workflow de GitHub Actions que publica automáticamente el sitio al hacer push a `main`. Ya está configurado y funcionando.

## Tecnologías
- HTML, CSS y JavaScript puro (sin dependencias externas ni build step).
- Gemini API v1beta (`gemini-2.0-flash`, streaming SSE).
- Web Speech API (reconocimiento y síntesis de voz).
- MediaDevices API (cámara).
- GitHub Actions + Pages para hosting.

## Estructura de archivos
- `index.html` → Aplicación completa (todo en un solo archivo).
- `.github/workflows/pages.yml` → Deploy automático a GitHub Pages.
- `README.md` → Este archivo.

## Notas importantes
- Edu está orientado a responder sobre el IPVG. El prompt del sistema le indica no inventar datos exactos (aranceles, puntajes, fechas) y recomendar revisar ipvg.cl cuando no está seguro.
- La IA puede equivocarse. Los datos oficiales siempre deben confirmarse en ipvg.cl o admisión.
