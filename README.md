# EcoMarket

## Nombre del proyecto
**EcoMarket** — Tienda virtual ecológica, reutilizable y sostenible.

## Descripción
EcoMarket es una tienda web estática, desarrollada con **HTML5 semántico** y **CSS3 puro**. Su objetivo es mostrar un catálogo de productos ecológicos con una identidad visual inspirada en la naturaleza, el consumo consciente y el diseño editorial premium.

## Objetivo del proyecto
Crear una experiencia visual atractiva, moderna, elegante y profesional para una tienda virtual ecológica, cumpliendo estrictamente con las restricciones técnicas impuestas (sin JavaScript, sin frameworks ni librerías).

## Características principales
- **HTML5 semántico** y arquitectura clara por archivos.
- **CSS3 puro** con **Variables CSS**, **Flexbox**, **CSS Grid**, **Media Queries**, pseudoclases y transiciones.
- **Identidad visual ecológica** con paleta basada en verdes, beige, blanco y grises cálidos.
- **Cuatro vistas completas**: Inicio, Productos (catálogo), Sobre nosotros y Contacto.
- **Catálogo con 20 productos** distribuidos en cuatro categorías: Hogar, Moda, Cuidado personal y Alimentos.
- **Favoritos visuales** con `checkbox` oculto + `label`, cambio de color al marcarse y persistente mientras la página esté abierta.
- **Productos agotados** con etiqueta visual clara y botón desactivado.
- **Menú móvil** con `checkbox` + CSS (sin JavaScript).
- **Formulario de contacto** con validación HTML nativa y estados visuales con `:valid`, `:invalid`, `:focus`.
- **Carrusel horizontal** con CSS puro para testimonios.
- **Filtros visuales** (categorías, precio, disponibilidad) estilizados con CSS.
- **Paginación visual** demostrativa.
- **Animaciones sutiles** con respeto a `prefers-reduced-motion`.
- **Accesibilidad**: etiquetas asociadas, `alt` descriptivos, `focus-visible`, jerarquía de encabezados.
- **Responsive**: Mobile First, adaptable a móvil, tablet, portátil y escritorio.
- **Sin dependencias**: puede abrirse localmente con Live Server.

## Tecnologías utilizadas
- HTML5
- CSS3 (Variables, Grid, Flexbox, Media Queries, Animaciones, Pseudoclases)

## Estructura de carpetas
```text
EcoMarket/
│
├── index.html
│
├── css/
│   ├── main.css        # Reset, variables, globales, tipografía
│   ├── layout.css      # Cabecera, navegación, grids, pie de página
│   ├── components.css  # Botones, tarjetas, formularios, filtros, favoritos
│   └── animations.css  # Transiciones y animaciones
│
├── img/
│   ├── products/       # Ilustraciones SVG de productos (p01-p20)
│   ├── icons/          # Iconos SVG ecológicos
│   └── hero/           # Imágenes e ilustraciones para hero/nosotros/contacto
│
├── views/
│   ├── productos.html
│   ├── sobre-nosotros.html
│   └── contacto.html
│
└── README.md
```

## Instrucciones para ejecutar el proyecto localmente
1. Clonar o descargar el proyecto.
2. Abrir la carpeta `EcoMarket` en **Visual Studio Code**.
3. Instalar/usar la extensión **Live Server**.
4. Abrir `index.html` con **Open with Live Server**.
5. Navegar entre las cuatro vistas desde el menú.

También puede abrirse directamente con el navegador, aunque Live Server es recomendado.

## Descripción de las cuatro vistas
| Vista | Archivo | Descripción |
|---|---|---|
| **Inicio** | `index.html` | Hero con llamado a acción, beneficios, productos destacados, banner de sostenibilidad y pie de página. |
| **Productos (Catálogo)** | `views/productos.html` | Catálogo con 20 productos, barra de búsqueda visual, filtros laterales, favoritos con checkbox CSS, productos agotados, paginación visual. |
| **Sobre nosotros** | `views/sobre-nosotros.html` | Historia/origen demostrativo, misión y visión, principios ecológicos, testimonios ficticios en carrusel CSS, llamado a la acción. |
| **Contacto** | `views/contacto.html` | Encabezado, formulario con validación nativa, información complementaria, redes sociales, mapa estático ilustrado. |

## Limitaciones de las funcionalidades sin JavaScript
- **Búsqueda**: Campo y botón son visuales. No filtra resultados.
- **Filtros del catálogo**: Controles HTML estilizados con CSS, sin lógica de filtrado.
- **Carrito**: Solo indicador visual `(0)`. Sin gestión de productos.
- **Favoritos**: Se marcan visualmente con `:checked`, pero no se guardan en almacenamiento.
- **Paginación**: Enlaces visuales. No cambia de página.
- **Formulario**: Validación nativa con HTML/CSS, pero **no envía mensajes reales**. Sin backend ni servicio externo.
- **Carrusel de testimonios**: Desplazable con scroll CSS, sin autoplay ni navegación con JavaScript.
- **Botones "Ver producto"**: Enlaces demostrativos hacia el catálogo o `#`.
- **Políticas/Legal**: Enlaces demostrativos (`#`).

Estas funcionalidades están identificadas como **visuales o demostrativas** conforme a las restricciones.

## Pasos para publicar el proyecto en GitHub
> **Nota:** No se han ejecutado commits/remotos aquí. Sigue estos pasos cuando lo autorices.

```bash
# Inicializar repositorio
git init

# Crear rama principal
git branch -M main

# Agregar archivos
git add .

# Primer commit
git commit -m "feat: initial commit EcoMarket"

# Crear repositorio en GitHub con nombre: EcoMarket_CamiloGonzalez
# Vincular remoto (reemplaza <tu-usuario>)
git remote add origin https://github.com/<tu-usuario>/EcoMarket_CamiloGonzalez.git

# Subir cambios
git push -u origin main
```

**Sugerencia de ramas de trabajo:**
- `feature/home`
- `feature/catalogo`
- `feature/sobre-nosotros`
- `feature/contact-form`
- `style/responsive`
- `docs/readme`

**Conventional Commits sugeridos:**
- `feat: create EcoMarket homepage`
- `feat: add responsive product catalog`
- `feat: create about us page`
- `feat: add contact form`
- `style: implement responsive layouts`
- `style: add CSS animations`
- `docs: write project documentation`
- `fix: correct navigation and image paths`

## Instrucciones para desplegarlo en Netlify o Vercel
### Netlify (Drop & Deploy o Git)
1. Ir a [netlify.com](https://www.netlify.com/) e iniciar sesión.
2. **Opción A - Drag & Drop:** Comprimir la carpeta `EcoMarket` (sin `.git`) y arrastrarla a "Deploy manually".
3. **Opción B - Git:** Conectar repositorio de GitHub y desplegar desde la rama `main`.
4. Configuración: **Publish directory** = `.` (raíz). Sin build command.
5. Desplegar. El sitio funcionará como estático.

### Vercel
1. Ir a [vercel.com](https://vercel.com/) e iniciar sesión.
2. Importar repositorio desde GitHub.
3. Framework Preset: **Other**.
4. Root Directory: `./`
5. Build Command: vacío.
6. Output Directory: `./`
7. Deploy.

**Requisito:** Debe desplegarse como página estática. No requiere Node.js, dependencias ni variables de entorno.

## Espacios para añadir capturas de pantalla
Agrega aquí tus capturas cuando las tengas:

### Escritorio
- [ ] `docs/captura-inicio-desktop.png`
- [ ] `docs/captura-productos-desktop.png`
- [ ] `docs/captura-sobre-nosotros-desktop.png`
- [ ] `docs/captura-contacto-desktop.png`

### Móvil
- [ ] `docs/captura-inicio-mobile.png`
- [ ] `docs/captura-productos-mobile.png`
- [ ] `docs/captura-menu-mobile.png`
- [ ] `docs/captura-contacto-mobile.png`

## Créditos y fuentes de las imágenes
- **Ilustraciones SVG propias**: Generadas para este proyecto académico (`img/products/*.svg`, `img/icons/*.svg`, `img/hero/hero.svg`, `historia.svg`, `mapa.svg`).
- **Fotografías**: Obtenidas de [Unsplash](https://unsplash.com/) con fines demostrativos y educativos.
- **Tipografías**: [Fraunces](https://fonts.google.com/specimen/Fraunces) y [Manrope](https://fonts.google.com/specimen/Manrope) vía [Google Fonts](https://fonts.google.com/).

## Nota importante
**Productos, precios, testimonios, datos de contacto, políticas, redes sociales y resultados comerciales son únicamente demostrativos.** Este proyecto tiene fines académicos y no representa una tienda real en operación. Las funcionalidades marcadas como "demostrativas" no tienen lógica de backend o JavaScript.
