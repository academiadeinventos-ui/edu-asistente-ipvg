# Edu · Asistente del IP Virginio Gómez

Asistente virtual (chatbot) interactivo para el Instituto Profesional Dr. Virginio Gómez G., con interfaz de humanoide animado, voz y (opcional) cámara.

## Archivos
- `index.html`: Aplicación web completa (HTML/CSS/JS en un solo archivo).

## Cómo funciona
- Interfaz responsive con tema claro/oscuro automático.
- Respuestas con voz (síntesis de voz del navegador, `es-CL`).
- Animación de boca sincronizada con el habla.
- Reconocimiento de voz (si el navegador lo soporta).
- Soporte para cámara (Edu "ve" la imagen cuando se activa).
- Cuando no está disponible el modelo de IA, usa respuestas predefinidas sobre carreras y sedes del IPVG.

## Publicar en GitHub Pages
1. Sube este repositorio a tu cuenta de GitHub.
2. En la configuración del repositorio, activa **GitHub Pages** desde la rama `main`.
3. Tu asistente estará disponible en `https://<tu-usuario>.github.io/<nombre-repo>/`.

> Nota: La funcionalidad de IA en tiempo real que usa `claude.use` solo funciona en el entorno de Arena.ai; al alojarlo públicamente, el asistente usará el sistema de respuestas de respaldo incluido en el código.
