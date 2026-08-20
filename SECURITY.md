# Seguridad de REPORT 2026 Landing

## Alcance

Este repositorio contiene una landing estática. No debe contener contraseñas, tokens, claves API, credenciales de Hostinger, credenciales de Cloudflare, archivos `.env`, certificados privados ni datos personales que no sean públicos y necesarios para el contacto comercial.

## Cómo informar un problema

Si detectás una credencial expuesta, una modificación no autorizada, un enlace sospechoso o una vulnerabilidad, no la publiques en un issue abierto. Contactá al responsable del repositorio por un canal privado y detallá el archivo, la URL, el momento de detección y los pasos para reproducirlo.

## Reglas de mantenimiento

1. Mantener la rama `main` como rama de publicación.
2. Realizar cambios mediante una rama separada y una revisión antes de fusionar.
3. No pegar tokens o contraseñas en HTML, CSS, README, issues, commits ni capturas.
4. Revisar los cambios antes de sincronizarlos con GitHub.
5. Rotar inmediatamente cualquier credencial que se haya expuesto, incluso si luego se elimina del archivo.
6. Mantener el dominio final con HTTPS activo y revisar DNS, redirecciones y certificados después de cada cambio de hosting.

## Modelo de amenaza básico

La landing es pública y su código fuente puede ser visible. Eso es normal para un sitio estático. La protección principal consiste en no incluir secretos, limitar quién puede escribir en el repositorio, revisar los cambios y utilizar un flujo de despliegue con permisos mínimos. La información de contacto publicada debe considerarse pública.
