# Challenge AluraFlix

## Descripción del proyecto
Aluraflix es una plataforma diseñada para gestionar vídeos, con funcionalidades como listar, registrar, actualizar y eliminar videos, implementando React con JavaScript. Ayudará a poner en práctica y reforzar tus conocimientos en esta librería, tales como componentización, uso de hooks, consumo de API, rutas entre otros.

### ⚠️ Atención
Este proyecto utiliza un servidor local creado con [json-server](https://www.npmjs.com/package/json-server).

## Características
### Gestión de Videos:

- Listar videos
- Registrar (agregar) videos
- Actualizar información de videos
- Eliminar videos

### Funcionalidades de React:
- `Componentización:`Desarrollar una aplicación modular dividiendo la interfaz de usuario en componentes reutilizables.
- `Uso de Hooks:`Implementar y manejar estados y efectos secundarios en componentes funcionales usando hooks como useState, useEffect, etc.
- `Consumo de API:`Realizar peticiones HTTP a una API para obtener, enviar, actualizar y eliminar datos de videos.
- `Manejo de Rutas:`Implementar navegación entre diferentes vistas o páginas dentro de la aplicación utilizando herramientas como React Router.

## Creación de proyecto
Ejecutar el comando:

    npm create vite@latest

Nombre: 
    
    challenge-aluraflix

Seleccionar:

    React
    JavaScript
Ejecutar:

    cd challenge-aluraflix
    npm install
    npm rin dev

### Opcional
En el script del package.json se agrega `start` 

        "scripts": {
        "start": "vite",
        "dev": "vite",
        },

Se ejecuta el proyecto con:

     npm start
Inicia el proyecto en [http://localhost:5173/](http://localhost:5173/) 

## Instalación 🔧
1. Instalar [react-router-dom](https://www.npmjs.com/package/react-router-dom), ejecutando el comando:

        npm i react-router-dom

    Es una dependecia de react que se utiliza para trabajar con las rutas.


2. Instalar [react-icons](https://react-icons.github.io/react-icons/search/#q=MdFavorite)

        npm install react-icons

3. Instalar del paquete de **[React-Loaders-Kit](https://seimodei.github.io/react-loaders-kit-examples/)**, ejecuando en cmd dentro del proyecto:

    npm i --save react-loaders-kit

    Creación del componente Loading.
    Conectar en el App.jsx.

4. Instalar [Styled Components](https://www.npmjs.com/package/styled-components), para escribir css en el JavaScript.

        npm i styled-components

    Documentación de [styled-components](https://styled-components.com/docs/basics)

5. Descargar [Normalize.css](https://necolas.github.io/normalize.css/), para que los navegadores muestren los elementos de forma consistente y acorde con los estándares modernos.

    **Pasos a realizar:**
    1. Ingresar a Normalize.css.
    2. Dar clic en descargar.
    3. Seleccionar el contenido con:
    
            Ctrl + a (selecciona)

            Ctrl + v (pega)

        Se pega el dentro del archio GlobalStyles.jsx, pero se debe eliminar los comentarios.

        *Ruta:*

            src
            ├── components
            │   ├── globalStyles
            │   │   ├── GlobalStyles.jsx

6.  **API falsa con json server**

    **6.1.** Instalar [json-server](https://www.npmjs.com/package/json-server), para Almacenamiento de Datos.

        npm install json-server

    Dentro del **package.json** se agrega automáticamente la siguiente dependencia:

        "json-server": "^1.0.0-beta.0"

    **6.2.** Crear un archivo db.json que tenga esta estructura:

             {
                    "videos": [
                        {
                            "id": 1,
                            "title": "Qué Significa Pensar Como Programador",
                            "category": "FRONT END",
                            "photo": "https://i.ytimg.com/vi/ov7vA5HFe6w/sddefault.jpg",
                            "link": "https://www.youtube.com/embed/ov7vA5HFe6w?si=rFYWWhqKMEWzxiJn",
                            "description": "¿Cuáles son las principales características de un programador? ¿Qué habilidades y competencias debe tener alguien que quiere seguir esa carrera? En este video Christian Velasco nos habla de las principales características de un Programador."
                        },
                    ]
            }

    **6.3.** Ejecutar el siguiente comando para levantar el servidor:

            npx json-server --watch db.json --port 3000

### Opcional

7. Para iniciar el servidor y proyectos al mismo tiempo instalar [concurrently](https://www.npmjs.com/package/concurrently)

        npm install concurrently --save-dev

    **7.1.**  Modificar el package.json agregando en el campo scripts el siguiente script:

        "start": "concurrently \"vite\" \"npx json-server --watch db.json --port 3000\"",


    **7.2.** Debería verse así:

        "scripts": {
            "start": "concurrently \"vite\" \"npx json-server --watch db.json --port 3000\"",
            "dev": "vite",
            "build": "vite build",
            "lint": "eslint . --ext js,jsx --report-unused-disable-directives --max-warnings 0",
            "preview": "vite preview"
        },

    **7.3.** Iniciar el servidor JSON ejecutando:

           npm start

* Se levanta el servidor local, permitiendo acceder a la API REST simulada en http://localhost:3000, y observará el archivo db.json en el puerto 3000 ruta videos:

        http://localhost:3000/videos

* Se levanta el proyecto en:

        http://localhost:5173/


## ✔️ Tecnologías
* [React + Vite](https://vitejs.dev/guide/)
* JavaScript

## Tecnologías secundarias
* Node.js y npm (incluyendo node_modules)
* JSON Server (db.json para simular API)
* VsCode
* Git
* GitHub

### Diseño
* [Figma](https://www.figma.com/design/fq7mKIvvVXYylv8eti3hjm/New-AluraFlix---ESP?node-id=1-106&t=HWLfNcrrMRgRcBBC-0) el quipo de Alura creó un modelo que muestra una representación visual del AluraFlix. Sin embargo, pueden haber algunos cambios en el proceso.

## Personas colaboradoras
**Alura Latam** organizó el Challenge AluraFlix y proporcionó las herramientas de gestión y diseño.
