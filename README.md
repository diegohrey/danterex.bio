# danterex.bio — web inicial

## Qué hay en esta carpeta
- `index.html`: el sitio completo en un solo archivo, en español, inglés, alemán y portugués. El idioma se elige solo según el navegador y se puede cambiar arriba a la derecha.
- `glosario.csv`: la tabla maestra del glosario (término en 4 idiomas + origen en 4 idiomas). Se abre en Excel. Es la misma base que luego alimenta los mazos de repaso.

## Antes de publicar (se edita al inicio del bloque `<script>`, en `CONFIG`)
1. **Correo:** crear `hola@danterex.bio` con reenvío al correo de Diego (casi todos los registradores lo ofrecen gratis). Si se usa otro, cambiar `email`.
2. **Redes:** cuando existan las cuentas, pegar los enlaces en `social` (YouTube, TikTok, Instagram). Mientras estén vacíos, se muestran como "pronto".
3. **Boletín "Ríos de ADN":** crear cuenta en un proveedor (Buttondown, Brevo o MailerLite tienen plan gratis) y pegar la URL de su formulario en `newsletterEndpoint`. Mientras esté vacío, el botón abre un correo a `hola@danterex.bio`.
4. **Textos:** que Dante los lea en voz alta; si algo no suena a él, se cambia en el bloque `I18N` (un bloque por idioma).

## Publicar gratis
Opción recomendada: **GitHub Pages**
1. Crear un repositorio (por ejemplo `danterex.bio`) y subir `index.html`.
2. Settings → Pages → publicar desde la rama `main`.
3. En "Custom domain" escribir `danterex.bio` y activar "Enforce HTTPS".
4. En el registrador del dominio, crear los registros DNS que indica la guía de GitHub Pages para dominios propios (registros A del dominio raíz y CNAME para `www`).

Alternativas igual de simples: Netlify o Cloudflare Pages (arrastrar la carpeta y conectar el dominio).

## Agregar un término al glosario
1. Agregar la fila en `glosario.csv` (fuente de verdad, con fuente consultada).
2. Copiar un bloque dentro de `TERMS` en `index.html` y cambiar los textos.
En las vacaciones de dic–ene se puede automatizar: un script que lea el CSV y genere una página por término (mejor para aparecer en Google).

## Reglas de privacidad (del plan)
Sin apellidos completos, colegio, uniforme, ciudad ni rutina de Dante. El contacto siempre llega a la familia.
