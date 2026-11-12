# Mundo Tecnológico - Tienda de Computación y Hardware

Sitio web profesional de comercio electrónico especializado en componentes de hardware, periféricos y equipos de computación gamer y de oficina.

## Tecnologías Utilizadas

- **HTML5:** Semántica, accesibilidad y metadatos Open Graph / SEO local.
- **CSS3 & SASS (SCSS):** Estilos modulares, diseño responsive con Grid y Flexbox.
- **Bootstrap 5.3:** Sistema de grillas y menú de navegación colapsable.
- **Librería AOS (Animate On Scroll):** Animaciones suaves al hacer scroll en todos los módulos.
- **Git y GitHub:** Control de versiones con ramas y flujo de trabajo colaborativo.

---

## Arquitectura de Estilos (SCSS)

El proyecto utiliza una arquitectura modular basada en **partials** dentro del directorio `scss/`:

```text
scss/
├── utilities/
│   ├── _variables.scss      # Colores de marca, tipografías, sombras y breakpoints
│   └── _mixins.scss         # Mixins con parámetros para flexbox y responsive
├── base/
│   ├── _base.scss           # Reset global, estilos del body y media query prefers-reduced-motion
│   └── _tipografia.scss     # Encabezados h1, h2, h3 y estilos de contenido
├── layout/
│   ├── _header.scss         # Encabezado principal y keyframes de entrada suave
│   ├── _nav.scss            # Barra de navegación Bootstrap personalizada
│   └── _footer.scss         # Pie de página y enlaces a redes sociales
├── components/
│   ├── _buttons.scss        # Botones de compra y formulario estilados con @extend
│   ├── _cards.scss          # Tarjetas de productos, etiquetas de oferta y galería
│   └── _sections.scss       # Secciones de beneficios, tablas, videos y formularios
└── main.scss                # Archivo principal orquestador que importa exclusivamente los partials
```

---

## Compilación de SCSS a CSS

Los estilos compilados se generan directamente en el archivo `styles/main.css`, manteniendo el código fuente separado del código final de producción.

### Opción 1: Con la extensión Live Sass Compiler (VS Code)
1. Abrir el proyecto en Visual Studio Code.
2. Hacer clic en el botón **`Watch Sass`** ubicado en la barra de estado inferior.
3. El compilador observará los cambios en `scss/main.scss` y regenerará `styles/main.css` automáticamente.

### Opción 2: Desde la terminal con Sass CLI
Para compilar manualmente el archivo una sola vez:
```bash
sass scss/main.scss styles/main.css
```

Para mantener la compilación en tiempo real en segundo plano:
```bash
sass --watch scss/main.scss:styles/main.css
```

---

## Estructura del Sitio

1. **Inicio (`index.html`):** Catálogo principal, beneficios de compra y promociones destacadas.
2. **Ofertas (`pages/ofertas.html`):** Descuentos por tiempo limitado y tabla comparativa de productos.
3. **Galería (`pages/galeria.html`):** Galería visual de setups gamer, notebooks y monitores.
4. **Nosotros (`pages/nosotros.html`):** Misión, visión, equipo de trabajo, video institucional y mapa de ubicación.
5. **Contacto (`pages/contacto.html`):** Formulario de consultas, horarios de atención y sucursal.

---

## Despliegue en Producción

- **Sitio Web en Vivo (Deploy):** https://diplomaturajaviercordoba.vercel.app/  
- **Repositorio GitHub:** [https://github.com/javicordoba10/Pagina-WEB-Computacion](https://github.com/javicordoba10/Pagina-WEB-Computacion)

---

## Autor

- **Javier Córdoba** - Diplomatura Full Stack Developer