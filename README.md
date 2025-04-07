
# Proyecto de Saludo Personalizado

Este es un proyecto simple que consta de un **frontend** y un **backend** para mostrar un mensaje de saludo personalizado basado en el nombre que ingresa el usuario. El frontend solicita el nombre a través de un formulario, y el backend responde con un mensaje personalizado usando una API.

## Tecnologías utilizadas

- **Frontend:**
  - HTML
  - CSS
  - JavaScript
- **Backend:**
  - Node.js
  - Express.js
  - CORS
  - Morgan 

## Descripción

El proyecto consiste en una aplicación que permite al usuario ingresar su nombre en un campo de texto y recibir un saludo personalizado en respuesta. La aplicación consta de dos partes:
- **Frontend:** Se encarga de la interfaz de usuario (HTML, CSS y JavaScript), enviando una solicitud al servidor con el nombre ingresado.
- **Backend:** Usa Node.js y Express.js para crear un servidor que maneja las solicitudes del frontend y responde con un mensaje de saludo.

### Características principales:
- **Formulario interactivo** donde el usuario puede ingresar su nombre.
- **Solicitud a un servidor** usando `fetch()` para obtener un mensaje de saludo personalizado.
- **Manejo de CORS** para permitir solicitudes entre diferentes puertos.

## Requisitos

- **Node.js** y **npm** instalados en tu máquina.

## Instalación

1. **Clona el repositorio:**

   ```bash
   git clone https://github.com/avilafelix998/Trabajo-Pr-ctico-N-1-Frontend-Backend.git
   ```

2. **Instala las dependencias del backend:**

   Navega a la carpeta del proyecto y ejecuta:

   ```bash
   npm install
   ```

3. **Instala las dependencias del frontend:**

   Si usas un servidor de desarrollo como `live-server` o solo abres el archivo HTML en tu navegador, no necesitas instalaciones adicionales. 

## Uso

### 1. **Backend (Servidor Node.js)**

- Abre una terminal en la carpeta del proyecto y ejecuta el servidor backend con el siguiente comando:

  ```bash
  npm run dev
  ```

  Esto iniciará el servidor en el puerto `3000`. Verás un mensaje en la terminal que dice:

  ```bash
  Servidor escuchando en el puerto http://localhost:3000
  ```

### 2. **Frontend (Interfaz de Usuario)**

- Abre el archivo `index.html` en tu navegador o usa un servidor local para cargar el archivo HTML. Esto mostrará la interfaz de usuario donde puedes ingresar tu nombre y hacer clic en el botón "Saludar".

### 3. **Flujo de trabajo:**
   - El usuario ingresa su nombre en el campo de texto y presiona el botón **"Saludar"**.
   - El frontend envía una solicitud `GET` al servidor backend con el nombre del usuario.
   - El backend responde con un saludo personalizado que se muestra en la página.



## Endpoints de la API

- **GET `/saludo/:nombre`**
  
  Este endpoint recibe un parámetro `nombre` en la URL y devuelve un saludo personalizado.

  **Ejemplo:**

  Solicitud:
  ```http
  GET http://localhost:3000/saludo/Juan
  ```

  Respuesta:
  ```text
  Hola, Juan!
  ```

