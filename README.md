# Edu-Path

![Edu-Path Logo](https://example.com/logo.png) <!-- Replace with actual logo URL -->

## Descripción

Edu-Path es una plataforma de aprendizaje en línea que ofrece una variedad de cursos diseñados para ayudar a los estudiantes a alcanzar sus objetivos educativos. Utilizando la metodología BEM (Block Element Modifier), hemos estructurado nuestro código CSS para facilitar la mantenibilidad y escalabilidad del proyecto.

## Características

- **Cursos en Línea**: Acceso a más de 100 cursos en diversas áreas.
- **Instructores Expertos**: Aprende de los mejores en la industria.
- **Certificaciones**: Obtén certificaciones al completar los cursos.
- **Planes Flexibles**: Diferentes opciones de suscripción para adaptarse a tus necesidades.

## Funcionamiento

La aplicación está diseñada para ser intuitiva y fácil de navegar. A continuación, se describen los elementos clave de la interfaz:

### Estructura del Código

- **HTML**: La estructura principal de la aplicación se encuentra en `index.html`. Este archivo contiene la disposición de los elementos y se organiza de la siguiente manera:

```html
<header class="header">
    <div class="header__container">
        <nav class="header__navbar navbar">
            <a href="" class="navbar__logo logo">
                <i class='bx bxs-institution logo__icon'></i>
                <span class="logo__text">EduPath</span>
            </a>
            ...
        </nav>
    </div>
</header>
```

- **CSS**: Utilizamos archivos CSS organizados en carpetas siguiendo la metodología BEM. Por ejemplo, el archivo `css/header/header.css` contiene estilos específicos para el encabezado:

```css
.header {
    background-image: url(../../images/bg2.png);
    background-repeat: no-repeat;
    background-size: cover;
    padding-bottom: 3rem;
}
```

### Elementos Destacados

- **Navegación**: La barra de navegación permite a los usuarios acceder fácilmente a diferentes secciones de la plataforma.
- **Estadísticas**: Sección que muestra estadísticas clave sobre la plataforma, como el número de cursos y estudiantes.

```html
<div class="overview__stats stats">
    <div class="stats__item stats__item--bg1">
        <i class="bx bx-slideshow stats__icon"></i>
        <p class="stats__text">
            <span class="stats__number">+100</span>
            <span class="stats__label">Cursos en Línea</span>
        </p>
    </div>
    ...
</div>
```

## Tecnologías Utilizadas

- **HTML5**: Para la estructura de la página.
- **CSS3**: Para el diseño y estilo, utilizando la metodología BEM.
- **JavaScript**: Para la interactividad (si aplica).
- **Boxicons**: Para los íconos utilizados en la interfaz.

## Instalación y Uso

1. Clona el repositorio:
   ```bash
   git clone https://github.com/tu_usuario/edu-path.git
   ```
2. Abre el archivo `index.html` en tu navegador para ver la aplicación en acción.

## Contribuciones

Las contribuciones son bienvenidas. Si deseas contribuir, por favor abre un issue o envía un pull request.

## Contacto

Para más información, puedes contactarnos a través de [correo@ejemplo.com](mailto:correo@ejemplo.com).
