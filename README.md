1. Crear una carpeta para el proyecto

Crea una carpeta con el nombre de tu aplicación y entra en ella.

Ejemplo:

Crear carpeta: mi-pwa

Abrir esa carpeta en tu editor de código (VS Code, por ejemplo)

2. Crear los archivos necesarios

Dentro de la carpeta crea estos archivos:

index.html → será la página principal

styles.css → estilos de la app

app.js → lógica de JavaScript

manifest.json → configura la app instalable

service-worker.js → permite que funcione sin internet

carpeta llamada icons → aquí van los iconos de la app

3. Diseñar la página web normal

Primero crea una página web básica (HTML, CSS y JS).
Una PWA siempre empieza como una web normal.

Debe tener:

Un título

Algo de contenido visible

Que funcione correctamente en el navegador

4. Crear el archivo manifest.json

Este archivo le dice al navegador que tu web se puede instalar como aplicación.

Aquí defines:

Nombre de la app

Iconos

Color principal

Cómo se abrirá (pantalla completa)

Página inicial

Sin este archivo NO hay PWA.

5. Agregar los iconos de la aplicación

Debes colocar al menos:

Un icono de 192x192 px

Un icono de 512x512 px

Estos van dentro de la carpeta icons.

Sirven para cuando el usuario instala la app en su celular.

6. Registrar el Service Worker

El service worker es lo que hace que la PWA funcione offline.

Este archivo:

Guarda archivos en caché

Permite abrir la app sin internet

Hace que cargue más rápido

Se registra desde JavaScript (app.js).

7. Configurar el caché en el service-worker.js

Aquí defines qué archivos se guardarán para usarse sin conexión.

Normalmente se guardan:

HTML

CSS

JS

Iconos

8. Probar la aplicación con un servidor local

Las PWA NO funcionan si abres el HTML con doble clic.
Debes usar un servidor local.

Ejemplos:

Live Server (VS Code)

python -m http.server

npx serve

9. Verificar que ya es una PWA

Abre la app en Chrome y revisa:

Herramientas de desarrollador → Application → Manifest

Si todo está bien:
Aparecerá el botón “Instalar aplicación”.

10. Probar modo offline

Apaga el internet y recarga la página.
Si sigue funcionando → tu PWA está correcta.
