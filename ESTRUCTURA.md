# Estructura del Proyecto

Este documento explica en detalle la estructura de archivos del portafolio web para un Ingeniero en Sistemas Computacionales.

## Archivos Principales

| Archivo | Descripción |
|---------|-------------|
| `app.py` | Contiene la configuración principal de la aplicación Flask |
| `main.py` | Punto de entrada para ejecutar la aplicación |
| `README.md` | Documentación general del proyecto |
| `INSTALACION.md` | Guía detallada de instalación |
| `ESTRUCTURA.md` | Este archivo que explica la estructura del proyecto |

## Directorios

### `/templates`

Contiene las plantillas HTML que Flask utiliza para renderizar las páginas web.

| Archivo | Descripción |
|---------|-------------|
| `index.html` | Página principal del portafolio con todas las secciones |

#### Secciones de `index.html`

1. **Navegación** - Barra de navegación con enlaces a las diferentes secciones
2. **Hero (Inicio)** - Sección de introducción con la información principal
3. **Perfil** - Información detallada sobre el perfil profesional e idiomas
4. **Habilidades** - Listado de habilidades técnicas divididas en:
   - Software (Bases de datos, ERP, Redes, Ofimática, Sistemas Operativos)
   - Hardware (Redes, Mantenimiento, Instalación, Equipos)
5. **Experiencia** - Experiencia laboral organizada cronológicamente
6. **Educación** - Formación académica y certificaciones
7. **Contacto** - Información de contacto y formulario para enviar mensajes

### `/static`

Archivos estáticos que no cambian y son servidos directamente por el servidor.

#### `/static/css`

Hojas de estilo CSS que definen la apariencia del portafolio.

| Archivo | Descripción |
|---------|-------------|
| `styles.css` | Estilos personalizados para todos los elementos del portafolio |

#### `/static/js`

Archivos JavaScript que controlan la interactividad del sitio.

| Archivo | Descripción |
|---------|-------------|
| `script.js` | Funcionalidades como desplazamiento suave, formulario de contacto, etc. |

#### `/static/img`

Imágenes y gráficos utilizados en el portafolio.

| Archivo | Descripción |
|---------|-------------|
| `profile-placeholder.svg` | Imagen SVG vectorial para el perfil del ingeniero |

## Flujo de la Aplicación

1. `main.py` inicia la aplicación Flask configurada en `app.py`
2. Cuando un usuario accede a la ruta principal `/`, Flask ejecuta la función `index()` en `app.py`
3. La función `index()` renderiza `templates/index.html`
4. Los archivos estáticos (CSS, JS, imágenes) son servidos directamente por Flask

## Tecnologías Utilizadas

- **Backend**:
  - Python 3.x
  - Flask (Framework web)
  - Gunicorn (Servidor WSGI opcional para producción)

- **Frontend**:
  - HTML5
  - CSS3
  - JavaScript
  - Bootstrap 5 (Framework CSS responsive)
  - Font Awesome (Iconos)