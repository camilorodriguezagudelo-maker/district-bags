# DISTRICT — Sprayground originales

Catálogo estático en español con cinco modelos, 21 fotografías, galerías, favoritos y una selección con subtotal.

## Ejecutar localmente

Requiere Python 3. Desde la raíz del proyecto:

```sh
python -m http.server 8000 --directory dist
```

Abre http://localhost:8000.

## Archivos

- `dist/index.html`: estructura y contenido.
- `dist/style.css`: diseño Mint Noir y adaptación móvil.
- `dist/app.js`: catálogo e interacciones.
- `dist/assets/`: 21 fotografías y `catalog.json`.

No requiere instalar dependencias ni compilar. Las fuentes de Google se descargan en línea, con fuentes alternativas locales.

## Precios en COP

Shark Rojo, Shark Graffiti, Shark Amarillo y Shark Oscuro: $700.000 cada uno. Hello 15 Years: $800.000.

Al cambiar precios, actualiza tanto el catálogo de `app.js` como `assets/catalog.json` y el precio inicial o contenido estático de `index.html` cuando corresponda.

## Alcance

Los favoritos y la selección se guardan en el navegador. Los enlaces de WhatsApp abren un mensaje para revisar antes de enviarlo. Copiar la selección no realiza pedidos. No hay backend de pagos ni checkout. Envío y disponibilidad por confirmar.

## Publicación

Configura `dist` como directorio público en un servicio de hosting estático. No hay comando de build. Subir el código a GitHub no publica por sí solo una web.

## Recursos

Las fotografías corresponden a los productos aportados por el propietario. No se concede una licencia de reutilización de esas imágenes ni de las marcas mediante este repositorio.

## Vercel

Importa este repositorio y usa la raíz del repositorio como Root Directory. `vercel.json` configura el sitio estático y la carpeta de salida `dist`. No necesita variables de entorno ni comando de compilación.