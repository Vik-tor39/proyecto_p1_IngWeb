# 🌿 Web Design Project — GRID/FLEX, SASS, BEM, Responsive Design

Este proyecto consiste en la **replicación de un diseño web realizado en Figma**, con el objetivo de poner en práctica conceptos fundamentales de **diseño web**, como la estructura semántica en **HTML**, el uso de **CSS (Grid y Flexbox)**, la **implementación de SASS/SCSS** bajo la metodología **BEM**, y la creación de un diseño **responsive** mediante *media queries*.

El resultado final corresponde a una **landing page** para una marca ficticia de herramientas ecológicas, donde se describen los productos, sus características, la misión de la empresa y un formulario de contacto.

---

## 🎯 Objetivo del proyecto

- Replicar fielmente el diseño original en Figma.  
- Aplicar estructura modular con **SASS y BEM**.  
- Usar **Flexbox** y **Grid** para la maquetación.  
- Implementar **Media Queries** con enfoque **Mobile First**.  
- Lograr un diseño completamente **responsive y escalable**.

---

## 🧠 Conceptos aplicados

- **HTML semántico:** estructura base del sitio.  
- **CSS:** propiedades y atributos, grid y flexbox.  
- **SASS/SCSS:** uso de variables, mixins, partials y `@forward`.  
- **BEM (Block Element Modifier):** para una arquitectura CSS modular y mantenible.  
- **Responsive Design:** diseño adaptado a distintos tamaños de pantalla (principal breakpoint: 768px).  
- **Estrategia Mobile First:** el diseño base se desarrolla para móvil y luego se expande hacia desktop.  

---

## ⚙️ Tecnologías y herramientas

| Tecnología / Herramienta | Uso principal |
|---------------------------|---------------|
| 🧩 **HTML** | Estructura del sitio |
| 🎨 **CSS (Grid / Flex)** | Diseño y maquetación |
| 🧵 **SASS / SCSS** | Modularización y reutilización de estilos |
| 🧱 **BEM** | Nomenclatura y organización del código CSS |
| 🧭 **Media Queries** | Adaptación responsive |
| ⚡ **Live Sass Compiler (VSCode)** | Compilación SCSS → CSS |

---

## 📁 Estructura del proyecto

```bash
project/
├── index.html
├── scss/
│   ├── about/
│   │   ├── _index.scss
│   │   └── _about.scss
│   ├── base/
│   │   ├── _globales.scss
│   │   ├── _index.scss
│   │   ├── _mixins.scss
│   │   ├── _utilities.scss
│   │   └── _vars.scss
│   ├── features/
│   │   ├── _features.scss
│   │   └── _index.scss
│   ├── footer/
│   │   ├── _footer.scss
│   │   └── _index.scss
│   ├── gallery/
│   │   ├── _gallery.scss
│   │   └── _index.scss
│   ├── header/
│   │   ├── _header.scss
│   │   ├── _nav.scss
│   │   └── _index.scss
│   ├── mission/
│   │   ├── _mission.scss
│   │   └── _index.scss
│   └── timeline/
│       ├── _advertencias.scss
│       ├── _timeline.scss
│       └── _index.scss
├── css/
│   ├── app.scss          # Archivo principal que importa todos los parciales SCSS
│   ├── app.css           # Resultado compilado del SCSS
│   └── app.css.map       # Archivo de mapeo SCSS → CSS
└── img/                  # Recursos gráficos
```
Cada carpeta dentro de scss/ representa una sección del HTML.
Los archivos _index.scss usan @forward para importar los parciales a app.scss.

---

## 🎨 Descripción visual del sitio 

El diseño sigue un estilo moderno, limpio y ecológico, combinando tonos verdes, azules y blancos.
Incluye secciones como:
- **Header**: barra de navegación con logo y botón de compra.
- **About**: descripción general del producto con imágenes y texto.
- **Features**: características destacadas con listas y fondo de color.
- **Mission**: presentación del producto principal.
- **Timeline**: cronología de la empresa y beneficios ecológicos.
- **Gallery**: galería de productos.
- **Footer**: información, enlaces y formulario de contacto.

**📱 Diseño responsive**
- Breakpoint principal: 768px.
- En dispositivos móviles, las secciones se apilan verticalmente.
- En pantallas grandes, se usa Grid y Flex para dividir las secciones en columnas.
- Se ajustan fuentes, márgenes y tamaños de imagen según el ancho del viewport.

---

## 🧩 Media query utilizado
```scss
@mixin tablet_mq {
  @media (min-width: 768px) {
    @content;
  }
}
```
Este mixin se utiliza en múltiples secciones (header, features, timeline, etc.) para adaptar el layout y los estilos.

---

## 🧠 Aprendizajes obtenidos

Durante este proyecto se reforzaron conceptos de:
- Diseño **HTML/CSS** estructurado y semántico.
- Modularización de estilos con **SASS y** BEM.
- Uso de **Grid y** Flexbox de forma combinada.
- Creación de **mixins reutilizables** para media queries.
- Construcción de un **diseño responsive** Mobile First.

---

## 🚀 Cómo ejecutar el proyecto

- 1️⃣ Clonar el repositorio
    ```bash
    git clone https://github.com/Vik-tor39/proyecto_p1_IngWeb.git
    ```
- 2️⃣ Abre el archivo index.html en tu navegador.
- 3️⃣ (Opcional) Usa la extensión Live Sass Compiler en VSCode para compilar los archivos .scss en tiempo real.

---

## 🎥 Defensa de la solución (video)
[![Ver demostración breve del proyecto](https://img.youtube.com/vi/NFwnRXNGjAc/hqdefault.jpg)](https://www.youtube.com/watch?v=NFwnRXNGjAc)

---

## 👤 Autor

**Víctor Suquilanda**  
📧 Proyecto Progreso 1 | Ingeniería Web (HTML, CSS, SASS, BEM, MEDIA QUERYS)  
📅 Año: 2025  

---