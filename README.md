# Taller 02 – Práctico Selectores CSS

**Fundamentos de Desarrollo Web**

Proyecto académico enfocado en la aplicación correcta de selectores CSS, jerarquía, especificidad y organización modular de estilos mediante archivos externos.

---

## Descripción del Proyecto

Este proyecto consiste en la construcción de una página temática titulada **“Archivos de la Ciudadela”**, inspirada en el universo de *Canción de Hielo y Fuego*.

El objetivo principal es aplicar de forma práctica:

* Selectores básicos (elemento, clase e ID)
* Selectores combinadores (descendentes, hijos directos, adyacentes y generales)
* Pseudo-clases (`:hover`, `:focus`, etc.)
* Organización modular de hojas de estilo
* Uso de variables CSS
* Buenas prácticas de estructura y nomenclatura (BEM)

---

## Objetivos Académicos

* Comprender la jerarquía del DOM y cómo afecta la aplicación de estilos.
* Aplicar correctamente la especificidad en CSS.
* Separar estructura (HTML) y presentación (CSS).
* Organizar estilos en múltiples archivos reutilizables.
* Implementar un diseño estructurado y semántico.

---

## Estructura del Proyecto

```
.
├── README.md
├── assets
│   ├── fonts
│   │   ├── Cinzel-VariableFont_wght.ttf
│   │   └── Inter-VariableFont_wght.ttf
│   ├── images
│   │   └── hero-bg.jpg
│   └── styles
│       ├── fonts.css
│       ├── reset.css
│       ├── style.css
│       └── variables.css
└── index.html
```

---

## Organización de Estilos

Los estilos están modularizados de la siguiente manera:

### 🔹 `reset.css`

Normaliza estilos por defecto del navegador.

### 🔹 `variables.css`

Define variables CSS globales:

* Paleta de colores
* Tipografías
* Valores reutilizables

Ejemplo:

```css
--color-primary
--color-bg
--font-primary
```

### `fonts.css`

Carga y declara las fuentes personalizadas del proyecto.

### `style.css`

Archivo principal que importa los anteriores y contiene:

* Estilos globales
* Componentes (navbar, hero, cards, footer, etc.)
* Layout (Flexbox y Grid)
* Pseudo-clases y efectos interactivos

```css
@import url(reset.css);
@import url(fonts.css);
@import url(variables.css);
```

---

## Estructura HTML

La página está organizada semánticamente utilizando:

* `<header>`
* `<nav>`
* `<main>`
* `<section>`
* `<article>`
* `<aside>`
* `<footer>`

Secciones principales:

* Hero principal
* Introducción
* Sagas
* Línea de tiempo
* Casas reales
* Formulario de contacto
* Galería
* Curiosidades
* Footer

---

## Metodología CSS

### Selectores Básicos

* Selectores por elemento (`body`, `h1`, `p`)
* Selectores por clase (`.btn`, `.hero`, `.navbar`)
* Selectores por ID (anclas de navegación)

### Selectores Combinadores

* Descendentes
* Hijos directos
* Estructura basada en anidación

### Pseudo-clases

```css
.btn:hover
.contact-form__input:focus
.curiosity__link:hover
```

### Metodología BEM

Se utilizó una convención similar a **BEM (Block Element Modifier)**:

```
.block
.block__element
.block--modifier
```

Ejemplos:

* `.navbar__item`
* `.btn--primary`
* `.contact-form__input--textarea`

---

## Tecnologías Utilizadas

* HTML5 semántico
* CSS3
* Flexbox
* CSS Grid
* Variables CSS
* Tipografías personalizadas

---

## Cómo Ejecutar el Proyecto

1. Clonar el repositorio:

```bash
git clone https://github.com/alomia/02-taller-practico-css.git
```

2. Abrir el archivo:

```bash
index.html
```

No requiere servidor ni dependencias externas.

---

## Conceptos Aplicados

* Especificidad CSS
* Cascada
* Modelo de caja
* Layout moderno con Flexbox y Grid
* Organización modular de estilos
* Diseño responsive base

