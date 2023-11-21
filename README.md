# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Tailwind CSS

Tailwind CSS es un framework de CSS de código abierto​ para el diseño de páginas web.

## Interfaz de Línea de Comandos

En un proyecto donde está instalado Vite, puedes usar el binario vite en tus scripts npm, o ejecutarlo directamente con npx vite. Estos son los scripts npm predeterminados en un proyecto de Vite ya montado:
**
{
  "scripts": {
    "dev": "vite", // inicia el servidor de desarrollo, alias: `vite dev`, `vite serve`
    "build": "vite build", // compila para producción
    "preview": "vite preview" // vista previa local de compilación para producción
  }
}

Puedes especificar opciones CLI adicionales como --port o --open. Para obtener una lista completa de las opciones de la CLI, ejecuta npx vite --help en tu proyecto.

## Uso de confirmaciones no publicadas
Si no puedes esperar a una nueva versión para probar las funciones más recientes, deberás clonar el repo de vite en tu máquina local y luego compilarlo y vincularlo tu mismo. (pnpm es obligatorio):

git clone https://github.com/vitejs/vite.git
cd vite
pnpm install
cd packages/vite
pnpm run build
pnpm link --global # utiliza el gestor de paquetes de tu preferencia para este paso

Luego ve a tu proyecto basado en Vite y ejecuta pnpm link --global vite (o el gestor de paquetes que usaste para vincular vite globalmente). ¡Ahora reinicia el servidor de desarrollo para hacerlo funcionar!

#### significado de las partes mas inportantes del proyecto
# src/ (carpeta):

Contiene el código fuente de la aplicación React. Aquí es donde escribirás la mayoría de tu código.

# index.html (archivo):

Es el punto de entrada HTML de tu aplicación. Este archivo suele contener el nodo <div id="app"></div>, que es el contenedor principal donde se montará la aplicación React.

# main.js o main.ts (archivo):

Es el punto de entrada JavaScript/TypeScript para tu aplicación. Este archivo suele importar el componente principal de React y montarlo en el contenedor HTML mencionado anteriormente.

# App.jsx o App.tsx (archivo):

Es el componente principal de tu aplicación React. Aquí es donde comienza la estructura de tu interfaz de usuario.

# vite.config.js (archivo):

Este archivo de configuración de Vite te permite personalizar la configuración de construcción y desarrollo de tu aplicación. Puedes ajustar parámetros como la carpeta de salida, configuración del servidor de desarrollo, etc.

# node_modules/ (carpeta):

Contiene las dependencias de tu proyecto que son instaladas mediante npm o yarn. No es necesario versionar esta carpeta, ya que las dependencias se pueden instalar nuevamente usando el archivo package.json.

# package.json (archivo):

Es el archivo de configuración para npm/yarn que contiene información sobre el proyecto, sus dependencias, scripts de construcción, entre otras cosas.

###  yarn.lock o package-lock.json (archivo)

Estos archivos se utilizan para bloquear las versiones exactas de las dependencias instaladas, asegurando la coherencia entre diferentes entornos de desarrollo.

## File src/assets

Es la carpeta donde se encuentran las img.
en ella se encuentran dos carpetas mas  prueba\src\assets\store y prueba\src\assets\social,

### File prueba\src\components

Es la carpeta en donde se encuentra el NavBar y el Footer de el sitio web 

## File prueba\src\data

Es la carpeta que importa el sample.json

## File prueba\src\pages

Es la Carpeta de cada pagina del sito web llas cueles son el Home, Movies, Series

## File prueba\src\styles

Es la carpeta de los estilos como de los Pages y los Components


# Cómo decidió las opciones técnicas y arquitectónicas utilizadas como parte de su  solución
##
##

## React y React Hooks:

Elegí utilizar React como la biblioteca principal para construir la interfaz de usuario debido a su flexibilidad, capacidad de manejar el estado de manera eficiente y su popularidad en el desarrollo de aplicaciones de una sola página (SPA).

## React Router para Navegación:

Opté por utilizar React Router para gestionar la navegación entre las páginas de "Inicio", "Series" y "Películas". Esta decisión se basa en la eficacia de React Router para crear una experiencia de navegación fluida en aplicaciones de una sola página.


## Styled-Components para Estilos:

Elegí la librería styled-components para gestionar los estilos de los componentes. Esta elección se basa en la capacidad de styled-components para proporcionar estilos encapsulados y mantener la modularidad del código.

## Manejo de Estados con React Hooks:

Utilicé React Hooks, como useState y useEffect, para gestionar los estados de carga, error y datos en las páginas de "Inicio", "Series" y "Películas". Esto garantiza un código más limpio y comprensible.

## React Popup para Información Completa:

Implementé el componente React Popup para mostrar la información completa de cada resultado al hacer clic en el título. Esta elección se basa en la simplicidad y eficacia de React Popup para crear ventanas emergentes interactivas.

## JSON como Fuente de Datos:

Decidí utilizar el archivo JSON feed/sample.json como fuente de datos debido a su estructura clara y la capacidad de React para manejar datos JSON de manera eficiente.

## Mobile-Friendly con Estilos Responsivos:

Garanticé que el diseño de las páginas fuera mobile-friendly mediante estilos responsivos. Esto se logró utilizando media queries y asegurándome de que la interfaz se adaptara correctamente a diferentes tamaños de pantalla.

## Enfoque en Modularidad y Reusabilidad:

Diseñé componentes modulares y reutilizables para cada parte de la aplicación, lo que facilita el mantenimiento y la escalabilidad del código.

##
##
### Hay alguna mejora que pueda hacer en su envío

1 - Manejo de Errores más Detallado:
2 - Mejoras Visuales y de Experiencia de Usuario:
3 - Control de Accesibilidad:
4 - Seguridad:
5 - Mejoras de UI/UX Responsivas:

### Qué haría de manera diferente si se le asignara más tiempo

1- Mejoras en el Diseño Visual
2 - Animaciones y Transiciones
3 - Pruebas Automatizadas más Exhaustivas
4 - Manejo Avanzado de Estados con Context API
5 - Internacionalización y Localización Completa
6 - Seguridad Adicional