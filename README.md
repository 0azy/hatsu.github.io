# Hatsu

**Hatsu** es un bot de seguridad para Discord en desarrollo, con moderación configurable y un panel autohospedado. Su propósito es ayudar a detectar estafas y spam y contener raids.

## Funciones implementadas

- Detección de dominios de estafa configurados por cada servidor.
- Eliminación de mensajes que coinciden con dominios confirmados o ciertos patrones de enlaces sospechosos.
- Ban automático configurable únicamente para dominios confirmados. Viene desactivado por defecto y solo afecta al servidor.
- Antiraid opcional mediante umbrales de entradas y timeouts temporales. Viene desactivado por defecto.
- Comandos `/hatsu` para configurar dominios, bans, antiraid y canal de avisos.
- Panel inicial con inicio de sesión de Discord. Requiere alojar y configurar una instancia propia.

La detección no cubre todas las variantes y no analiza imágenes ni mensajes directos. Mantén revisión humana para acciones automáticas.

## Datos y privacidad

El contenido de mensajes se procesa en memoria y no se escribe en los registros. La instancia guarda configuración local por servidor y metadatos de moderación en archivos diarios separados por servidor. Los registros con más de 30 días se eliminan al iniciar y cada 24 horas mientras Hatsu está ejecutándose. Las sesiones del panel permanecen en memoria hasta cuatro horas; el token OAuth no se guarda en disco.

Quien controla el equipo que aloja Hatsu puede acceder al contenido durante el procesamiento y a los archivos locales. Para que el operador del servicio no pueda leer esos registros, cada comunidad debe alojar su propia instancia.

- [Política de Privacidad](https://0azy.github.io/hatsu.github.io/privacy-policy.html)
- [Condiciones del Servicio](https://0azy.github.io/hatsu.github.io/terms-of-service.html)
- [Sitio legal](https://0azy.github.io/hatsu.github.io/)

## Este repositorio

Este repositorio publica las páginas legales de Hatsu mediante GitHub Pages. El código del bot se mantiene en el workspace de desarrollo.

- Portada: `index.html`
- Privacidad: `privacy-policy.html`
- Condiciones: `terms-of-service.html`

## Contacto

Para consultas sobre Hatsu o sus políticas, escribe a [zyra.develops@gmail.com](mailto:zyra.develops@gmail.com).
