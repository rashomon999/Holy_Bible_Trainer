# Santa Biblia — Landing (redirección a Google Play)

Página estática para poner en la bio de Instagram. Enlaza a:
https://play.google.com/store/apps/details?id=com.myshkin.holybible

## Desplegar en Vercel
- **Opción A (Git):** sube este repo a GitHub y en vercel.com haz *Add New → Project → Import*.
  No hace falta configurar nada: es un sitio estático estático, todo en la raíz.
- **Opción B (CLI):** `npx vercel --prod` desde esta carpeta.

## Cambiar el link de Google Play
Está en dos sitios dentro de `index.html`:
1. La constante `PLAY_URL` en el `<script>` del final.
2. Los `href` de los dos botones `.cta`.

## Redirección automática
En el `<script>` final: `AUTO_REDIRECT = true` hace que la página salte sola
a Google Play después de `AUTO_REDIRECT_DELAY` milisegundos.
