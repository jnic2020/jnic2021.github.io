# Web para la JNIC 2020

La URL para probar la web es https://2020.jnic.es/

Después de subir cambios a este repositorio, hay que esperar unos 15 segundos y refrescar la web varias veces para que se reflejen.

# Slider

Para añadir o quitar imágenes al slider de la página principal hay que editar el fichero `_layouts/home.html` y editar abajo:

```javascript
var urlArray = [
'{{ site.url }}/images/slider1.jpg',
'{{ site.url }}/images/slider2.jpg'
];
```
Las imágenes no deberían pesar más de 500KB para no ralentizar la carga de la web. (Ojo al copyright...)

# Fechas importantes y noticias

Para añadir/quitar fechas importantes y/o noticias hay que editar el fichero `_data/fechas_importantes.json` y `_data/noticias.json`. El campo `fecha_ref`se usa para ordenar por fecha.

# Contenido de las distintas secciones

El contenido de cada sección se cambia editando los ficheros markdown (extensión `.md`). Más info sobre markdown: https://gist.github.com/roachhd/779fa77e9b90fe945b0c

Para quitar o añadir secciones al menú principal hay que editar el fichero `_config.yml`:

```markdown

links:
  - title: Comités
    url: /comites
    external: false
  - title: Participa
    url: /participa
    external: false
  - title: Envío de trabajos
    url: /trabajos
    external: false
  - title: Programa
    url: /programa
    external: false
  - title: Sede
    url: /sede
    external: false
  - title: Inscripción
    url: /inscripcion
    external: false
  - title: Patrocinadores
    url: /patrocinadores
    external: false
  - title: Contacto
    url: /contacto
    external: false
```

