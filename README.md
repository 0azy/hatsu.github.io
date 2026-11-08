# Hatsu

**Hatsu** es un bot de seguridad para Discord, actualmente en desarrollo. Su objetivo es ayudar a las comunidades a detectar estafas, reducir el spam y responder a raids con moderación configurable y permisos mínimos.

## Estado del proyecto

El prototipo del bot incluye:

- Detección de dominios de estafa configurados y de algunos patrones de enlaces sospechosos.
- Eliminación de mensajes detectados.
- Ban opcional dentro del servidor para coincidencias de alta confianza; viene desactivado por defecto.
- Registro local de metadatos de moderación, sin guardar el texto ni las URLs del mensaje.

El panel web, el inicio de sesión con Discord, la configuración por servidor y las reglas completas antiraid todavía están en desarrollo. Este repositorio contiene el sitio de políticas; el código del bot se mantiene aparte.

## Privacidad

El contenido de los mensajes se analiza en memoria para moderarlos. El prototipo guarda los identificadores del servidor, canal, miembro y mensaje, la regla detectada y el resultado de la acción en `hatsu-actions.jsonl`, en el equipo que aloja el bot. No hay borrado automático de esos registros todavía.

Para conocer los detalles, consulta la [Política de Privacidad](https://0azy.github.io/hatsu.github.io/privacy-policy.html). Las [Condiciones del Servicio](https://0azy.github.io/hatsu.github.io/terms-of-service.html) explican el uso del bot.

## Documentos

- [Política de Privacidad](https://0azy.github.io/hatsu.github.io/privacy-policy.html)
- [Condiciones del Servicio](https://0azy.github.io/hatsu.github.io/terms-of-service.html)
- [Sitio legal de Hatsu](https://0azy.github.io/hatsu.github.io/)

## GitHub Pages

Este repositorio publica el sitio legal. GitHub Pages está configurado para servir la rama `main` desde la carpeta raíz. Los archivos principales son `index.html`, `privacy-policy.html` y `terms-of-service.html`.

## Contacto

Para consultas sobre Hatsu o sus políticas, escribe a [zyra.develops@gmail.com](mailto:zyra.develops@gmail.com).
