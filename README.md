# Bryan Growth — blog

Sitio estático. Sin build, sin dependencias: abrir `index.html` o servir la carpeta tal cual.

Sistema visual: **papel, archivo y azul** (manual v2.0, proyecto de design system en Claude Design `01ce26bb…`). Todo lo visual está en `assets/css/bryan-growth.css`.

```
index.html                        Portada del blog: lista de escritos
escritos/<slug>/index.html        Una pieza (post)
escritos/<slug>/imagens/          Sus fotos (img-N.jpg para web, img-N.png originales)
assets/css/bryan-growth.css       Tokens + componentes + maquetación (compartido)
assets/logo/                      Monograma BG, 4 variantes (texto vivo: requiere Archivo Black)
```

## Añadir una pieza

1. Duplicar `escritos/niveis-de-consciencia/` con un nuevo slug (minúsculas, guiones).
2. En su `index.html` cambiar: `<title>`, metas, número de pieza (`7` → el siguiente del registro, sin ceros a la izquierda, no se reinicia), etiqueta de categoría, tiempo de lectura, fecha, título (línea grotesca + línea didona), entradilla y el cuerpo.
3. Poner las fotos en `imagens/` (blanco y negro, de archivo; JPEG ≤1200px para web).
4. En `index.html` (portada): actualizar el bloque **Última peça** (foto 16:9, número, título, pie, etiqueta). La lista **Todas as peças** está comentada mientras hay una sola pieza: al publicar la segunda, quitar los delimitadores `<!-- -->` y añadir una `<li>` por pieza (la más nueva arriba), con el mismo título y pie que usa el post.

## Copy: una sola verdad por pieza

El título (línea grotesca, ≤5 palabras), el pie de una línea, la categoría, la fecha y los minutos de lectura se escriben una vez y se repiten iguales en: `<title>`, portada (destaque y lista), cabecera del post y cabecera corrida. Mayúscula inicial de frase, nunca Title Case. Byline: `Bryan Orellana · estrategista criativo`.

## Reglas rápidas del manual

- Seis colores + Klein `#002FA7` como único acento (≤8% de la pieza, un solo uso por pieza: número, filete, palabra, tachado o duotono).
- Tres familias: didona (Playfair Display), grotesca (Archivo / Archivo Black), lectura (EB Garamond). Dos por bloque, nunca las tres.
- Radio 0. Sin sombras. Sin degradados. Sin iconos ni emoji (`✕` solo en listas de exclusión).
- Fotografía siempre B/N de archivo; sin pantallas, cables ni oficinas modernas.
- Jerarquía con filetes: 1px gris claro · 1px tinta · 2px tinta (sección) · 3px azul (regla) · 4px azul (cita).
- Transiciones de color de 120ms y nada más: sin fades ni revelados al scroll.
