# REPORT 2026 — Landing B2B

Landing informativa de REPORT 2026 y del Congreso Técnico ATIPAT.

## Estructura

- `index.html`: contenido y estructura de la landing.
- `styles.css`: estilos responsive, UX y presentación visual.

## Flujo de actualización

Las modificaciones se realizan primero en la versión de trabajo de Manus. Luego se sincronizan con este repositorio mediante un commit descriptivo y una revisión previa. No publicar cambios en producción sin aprobación explícita.

## Flujo de publicación

La landing se publica desde la rama `main` mediante GitHub Pages. Los cambios deben prepararse primero en una rama separada, revisarse visualmente y luego fusionarse a `main`. El workflow de Pages tiene permisos mínimos: lectura del contenido, escritura limitada del artefacto de Pages y emisión de identidad para el despliegue.

## Despliegue futuro en Hostinger

La landing es estática y puede desplegarse copiando `index.html` y `styles.css` al directorio público del dominio, normalmente `public_html`, mediante el Administrador de archivos, SFTP o Git si el plan lo permite. Antes de desplegar, verificar dominio, SSL, DNS, rutas, enlaces de WhatsApp y versión móvil. Las credenciales de Hostinger nunca deben guardarse en este repositorio.

## Seguridad

Consultá `SECURITY.md` antes de incorporar integraciones o credenciales. Un repositorio público puede exponer su código fuente, pero no debe exponer secretos. Si se conecta Hostinger o Cloudflare, las credenciales deberán gestionarse fuera del HTML/CSS y con permisos limitados.
