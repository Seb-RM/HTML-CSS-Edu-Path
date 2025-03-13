# 🎓 EduPath - Plataforma de Aprendizaje en Línea 🚀
Este proyecto simula la pagina de inicio de una plataforma de aprendizaje en línea diseñada para ofrecer cursos, certificaciones y recursos educativos. Desarrollado aplicando la metodología BEM (Block, Element, Modifier) para garantizar un código limpio, modular y fácil de mantener. A continuación, te explicamos todo lo que necesitas saber sobre este proyecto.
## 📌 Características Principales
- **Diseño Responsivo**: La página se adapta a diferentes dispositivos, desde móviles hasta pantallas de escritorio.

- **Metodología BEM**: Uso de la metodología BEM para la organización del CSS, lo que facilita la escalabilidad y mantenimiento del código.

- **Componentes Reutilizables**: Bloques y elementos reutilizables como botones, tarjetas, y secciones que permiten una construcción rápida y consistente.

- **Integración de Íconos y Fuentes**: Uso de Boxicons para íconos y Google Fonts para tipografías modernas.

- **Secciones Dinámicas**: Incluye secciones como cursos, planes de suscripción, testimonios y más.
## 🛠 Tecnologías Utilizadas
- **HTML5**: Estructura semántica y accesible.

- **CSS3**: Estilos avanzados con variables CSS y organización modular.

- **BEM**: Metodología para nombrar y organizar clases CSS.

- **Boxicons**: Biblioteca de íconos para una interfaz más atractiva.

- **Google Fonts**: Fuentes modernas y legibles.
## 🧩 ¿Qué es BEM?
**BEM** (Block, Element, Modifier) es una metodología para nombrar y organizar clases CSS. Su objetivo es crear componentes reutilizables y mantener un código limpio y escalable. En este proyecto, se ha aplicado BEM de la siguiente manera:

- **Bloque**: Un componente independiente y reutilizable (ej: `.header`, `.footer`).

- **Elemento**: Una parte de un bloque que no tiene sentido por sí sola (ej: `.header__logo`, `.footer__social`).

- **Modificador**: Una variación de un bloque o elemento (ej: `.button--primary`, `.course__price--line`).

Ejemplo de BEM en el código:

```html
<header class="header">
    <div class="header__container">
        <nav class="header__navbar navbar">
            <a href="" class="navbar__logo logo">
                <i class='bx bxs-institution logo__icon'></i>
                <span class="logo__text">EduPath</span>
            </a>
        </nav>
    </div>
</header>
```
## 🚀 Funcionamiento de la Aplicación
### 1. Header (Encabezado)
- **Navbar**: Menú de navegación con un logo y enlaces a las diferentes secciones de la página.

- **Intro**: Sección de introducción con un título llamativo, descripción y botones de acción.

```html
<section class="header__intro intro">
    <h1 class="intro__title">Aprendizaje ilimitado a tu alcance</h1>
    <p class="intro__desc">...</p>
    <div class="intro__actions actions">
        <a href="" class="actions__start-button">Empezar ahora</a>
        <button class="actions__play-btn play-btn">
            <i class="bx bx-play-circle play-btn__icon"></i>
            <span class="play-btn__text">Ver video</span>
        </button>
    </div>
</section>
```
### 2. Overview (Resumen)
- **Estadísticas**: Muestra números clave como la cantidad de cursos, instructores y estudiantes.

- **Educación**: Información sobre los beneficios de la plataforma.

```html
<div class="overview__stats stats">
    <div class="stats__item stats__item--bg1">
        <i class="bx bx-slideshow stats__icon"></i>
        <p class="stats__text">
            <span class="stats__number">+100</span>
            <span class="stats__label">Cursos en Línea</span>
        </p>
    </div>
</div>
```
### 3. Cursos
- **Listado de Cursos**: Muestra los cursos más populares con imágenes, descripciones y precios.

```html
<a class="courses__course course">
    <img src="./images/course-01.jpg" alt="Imagen de curso" class="course__image">
    <div class="course__text">
        <h3 class="course__title">Título del curso se muestra aquí</h3>
        <p class="course__desc">...</p>
    </div>
    <div class="course__footer">
        <p class="course__price">$40 USD</p>
    </div>
</a>
```
### 4. Planes de Suscripción
- **Planes Free, Basic y Expert**: Ofrece diferentes niveles de suscripción con beneficios específicos.

```html
<div class="plans__plan plan">
    <div class="plan__header">
        <h4 class="plan__title">Free</h4>
        <p class="plan__price">Gratis</p>
        <p class="plan__billing">Acceso gratuito a los cursos gratuitos</p>
    </div>
    <ul class="plan__features">
        <li class="plan__feature">
            <i class="bx bx-check"></i>
            Acceso a cursos gratuitos
        </li>
    </ul>
    <a href="" class="plan__button">Suscríbete a Free</a>
</div>
```
### 5. Testimonios
- **Opiniones de Estudiantes**: Muestra testimonios de estudiantes con sus fotos, nombres y calificaciones.

```html
<div class="testimoniales__testimony testimony">
    <div class="testimony__header">
        <img src="./images/photo-profile.jpg" alt="Foto de perfil" class="testimony__profile">
        <h4 class="testimony__name">Juan Carlos</h4>
        <i class="bx bxs-quote-left testimony__icon"></i>
    </div>
    <p class="testimony__stars">...</p>
    <p class="testimony__desc1">...</p>
</div>
```
### 6. Footer (Pie de Página)
- **Información de Contacto**: Enlaces a redes sociales, información de la compañía y enlaces útiles.

```html
<footer class="footer">
    <div class="footer__container">
        <div class="footer__brand">
            <a href="" class="footer__logo logo">
                <i class="bx bxs-institution logo__icon"></i>
                <span class="logo__text">EduPath</span>
            </a>
        </div>
    </div>
</footer>
```
## 🎨 Estilos CSS
El CSS está organizado en módulos siguiendo la metodología BEM. Cada bloque tiene su propio archivo CSS, lo que facilita la mantenibilidad y escalabilidad del proyecto.

Ejemplo de estructura CSS:

```css
/* Estilos para el header */
.header {
    background-color: var(--color-900);
    color: var(--color-100);
}

.header__container {
    max-width: 120rem;
    margin: 0 auto;
}

.navbar__logo {
    display: flex;
    align-items: center;
}
```
## 📂 Estructura del Proyecto
```
/HTML-CSS-Edu-Path
│
├── index.html
│
├── css
│   ├── base.css
│   ├── main.css
│   ├── normalize.css
│   ├── courses
│   │   └── courses.css
│   ├── footer
│   │   └── footer.css
│   ├── header
│   │   ├── header.css
│   │   ├── header__intro.css
│   │   └── header__navbar.css
│   ├── overview
│   │   ├── overview__education.css
│   │   └── overview__stats.css
│   ├── plans
│   │   └── plans.css
│   └── testimonials
│       └── testimonials.css
│
└── images
   └── ... (archivos de imágenes)
```
## 🚀 Cómo Ejecutar el Proyecto
1. Clona el repositorio.

2. Abre el archivo `index.html` en tu navegador.

3. Explora las diferentes secciones de la página.