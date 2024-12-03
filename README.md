# Proyecto de Aplicación de Búsqueda de Películas y Series

Este proyecto consiste en desarrollar una aplicación web que permite buscar películas y series utilizando la API de OMDb. La aplicación cargará recursos mediante AJAX y ofrecerá una experiencia de usuario fluida sin recargar la página. 
Uso de API Google Charts para mostrar gráficas de los datos.

## Características Principales

- **Landing Page**: La aplicación comienza con una página de inicio que explica el objetivo del sitio web.
- **Búsqueda Dinámica**: Los usuarios pueden buscar películas o series. Al introducir al menos 3 caracteres, la búsqueda se lanza automáticamente.
- **Resultados de Búsqueda**: Los resultados se muestran sin recargar la página y se pueden paginar o mostrar mediante scroll infinito.
- **Detalles de Películas/Series**: Al seleccionar un elemento, se muestra información detallada como el póster, director, actores, sinopsis y año.
- **Navegación Intuitiva**: Los usuarios pueden regresar al listado anterior manteniendo su estado.
- **Imágenes por Defecto**: Si falta una imagen, se muestra una imagen por defecto para evitar errores visuales.

## Funcionalidades Adicionales

- **Scroll Infinito**: En lugar de un botón "Ver más", los datos adicionales se cargan automáticamente al desplazarse hacia abajo.
- **Búsqueda de Series**: Además de películas, se pueden buscar series.
- **Valoraciones Completas**: En la vista detallada se muestran todas las valoraciones disponibles proporcionadas por la API.
- **Generación de Informes**: Los usuarios pueden crear informes basados en:
  - Películas más valoradas según `imdbRating`.
  - Películas con mayor recaudación.
  - Películas más votadas.

## Implementación Técnica

### Tecnologías Usadas

- **OMDb API**: Para obtener datos sobre películas y series.
- **AJAX**: Para realizar solicitudes asíncronas a la API sin recargar la página.
- **JavaScript (ES6)**: Para manejar la lógica del cliente y las interacciones del usuario.
- **HTML/CSS**: Para estructurar y estilizar la interfaz de usuario.

### Estructura del Código

- **Carga Inicial**: Se configura un evento `window.onload` para inicializar los elementos interactivos y configurar los manejadores de eventos.
- **Búsqueda y Resultados**: La función `buscar()` gestiona las solicitudes a la API y actualiza el DOM con los resultados obtenidos.
- **Scroll Infinito**: Implementado mediante el evento `scroll` para cargar más resultados cuando el usuario se desplaza hacia abajo.
- **Detalles de Películas/Series**: La función `detalles()` obtiene información detallada de un elemento seleccionado y actualiza la vista correspondiente.

### Manejo de Errores

- Se proporciona una imagen por defecto si no hay disponible una imagen específica para una película o serie.
- Mensajes claros para errores en las búsquedas o cuando no hay resultados disponibles.

## Instalación y Configuración

1. Clona este repositorio en tu máquina local.
2. Asegúrate de tener acceso a la [OMDb API](https://www.omdbapi.com/) y obtener una clave API válida.
3. Configura tu entorno local para servir archivos HTML (puedes usar un servidor local como `http-server`).
4. Modifica el archivo JavaScript para incluir tu clave API en las solicitudes a OMDb.

## Contribuciones

Las contribuciones son bienvenidas. Por favor, sigue las pautas estándar para contribuir a proyectos open-source.

---

## Pagina en producción

https://github.com/serporion/BuscardorPeliculas



Este README proporciona una visión general del proyecto, sus características principales, implementación técnica y pasos para comenzar a trabajar con él.

Citations:
[1] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/44432439/551ee7b6-bf54-4e91-b995-52c7c4098c26/paste.txt
[2] https://www.omdbapi.com
[3] https://developers.google.com/chart?hl=es-419
