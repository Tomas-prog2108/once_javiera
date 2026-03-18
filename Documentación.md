# Decisiones semánticas

Para hacer mi tarjeta de presentación utilice etiquetas semánticas de HTML5 con el objetivo de darle una estructura compresible al código.

## Estructura general

- `<header>`
  Se utilizó para agrupar el título principal, el nombre y la cita. Es la introducción del contenido.

- `<main>`
  Contiene el contenido principal de la página, donde se encuentra toda la información relevante.

- `<footer>`
  Incluye la información de contacto y derechos de autor. Es  el cierre de la tarjeta de presentación.


## Organización del contenido

- `<section>`
  Lo utilice para dividir el contenido en bloques:

  * Sobre mí
  * Habilidades
  * Pasatiempos
  * Contacto

- `<article>`
  Lo empleé dentro de el bloque "Pasatiempos" para cada actividad, ya que cada una puede considerarse una unidad independiente del contenido.


## Encabezados

- `<h1>`: Título principal de la página.
- `<h2>`: Subtítulos de secciones principales.
- `<h3>`: Subtítulos dentro de artículos.
- `<h4>`: Subtítulo en el footer.


## Etiquetas de texto

- `<p>`: Para párrafos de texto.
- `<strong>`: Para resaltar información importante.
- `<em>`: Para énfasis o tono reflexivo.
- `<br>`: Para saltos de línea en la cita.


## Etiquetas semánticas

- `<time>`
  Se utilizó para fechas (nacimiento y año actual), lo que permite interpretación por máquinas.

- `<ul>` y `<li>`
  Para listar habilidades de forma ordenada y clara.

- `<address>`
  Para información de contacto, indicando semánticamente que es información de ubicación o comunicación.

- `<a href="mailto:...">`
  Permite enviar correos directamente desde el enlace.

- `<small>`
  Para texto legal o menos relevante visualmente.

- `<hr>`
  Para separar visualmente secciones importantes (header/main/footer).


## Árbol DOM.

Esta es la estructura jerárquica del la página:

```
html
├── head
│   ├── meta (charset)
│   ├── meta (viewport)
│   └── title
│
└── body
    ├── header
    │   ├── h1
    │   ├── h2
    │   └── p
    │       └── em
    │
    ├── hr
    │
    ├── main
    │   ├── section (Sobre mí)
    │   │   ├── h2
    │   │   ├── p
    │   │   │   └── time
    │   │   ├── p
    │   │   ├── p
    │   │   └── p
    │   │
    │   ├── section (Habilidades)
    │   │   ├── h2
    │   │   └── ul
    │   │       ├── li
    │   │       ├── li
    │   │       ├── li
    │   │       └── li
    │   │
    │   └── section (Pasatiempos)
    │       ├── h2
    │       ├── article
    │       │   ├── h3
    │       │   └── p (x2)
    │       ├── article
    │       │   ├── h3
    │       │   └── p
    │       └── article
    │           ├── h3
    │           └── p
    │
    ├── hr
    │
    └── footer
        ├── section
        │   ├── h4
        │   └── address
        │       ├── p (email - a)
        │       └── p (ubicación)
        │
        └── p
            └── small
                └── time