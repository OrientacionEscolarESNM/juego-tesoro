# Búsqueda del Tesoro AR 🏴‍☠️🧩

Un juego interactivo de búsqueda del tesoro desarrollado con Realidad Aumentada (WebAR) utilizando **8th Wall** y **Firebase**. 

## Descripción

Este proyecto es una experiencia inmersiva donde los jugadores deben buscar y escanear diferentes marcadores (Image Targets) en el mundo real. Al escanerlos utilizando la cámara de su dispositivo móvil, descubren pistas, resuelven rompecabezas y avanzan en la búsqueda del tesoro.

El juego cuenta con:
- **Experiencia WebAR**: No requiere descargar ninguna aplicación; funciona directamente desde el navegador móvil gracias a la tecnología de 8th Wall.
- **Seguimiento de Imágenes (Image Targets)**: Reconocimiento de marcadores en el entorno para mostrar contenido 3D, videos o pistas.
- **Sistema de Misiones (Quests)**: Los jugadores progresan a través de una historia interactiva.
- **Panel de Administración**: Un dashboard para monitorear el progreso de los jugadores y gestionar la experiencia.
- **Persistencia de Datos**: Utiliza Firebase (Realtime Database / Firestore) para guardar el progreso, registros y ranking de los jugadores en tiempo real.

## Tecnologías Utilizadas

- **8th Wall**: Motor de WebAR para reconocimiento de imágenes y posicionamiento espacial.
- **Firebase**: Backend as a Service (BaaS) para la gestión de usuarios y almacenamiento de datos.
- **HTML / CSS / JavaScript**: Estructura, estilos y lógica del juego.
- **A-Frame / Three.js** *(implícito en 8th Wall)*: Para la renderización de los elementos de Realidad Aumentada.

## Estructura del Proyecto

- `index.html`: Punto de entrada de la aplicación y experiencia de jugador.
- `admin.html`: Panel de control para administradores.
- `assets/`: Carpeta que contiene recursos multimedia como imágenes, videos (`.mp4`), modelos 3D y audios (`.mp3`).
- `image-targets/`: Contiene la configuración y miniaturas de los marcadores (targets) que 8th Wall debe reconocer.
- `bundle.js`: Lógica del juego compilada.
- `firebase-config.js`: Credenciales y configuración de conexión con Firebase.

## Despliegue

Este proyecto está configurado para ser alojado como una página web estática. Actualmente se recomienda su despliegue a través de **GitHub Pages**, lo cual facilita la distribución masiva con soporte HTTPS (necesario para acceder a la cámara en WebAR).

Para jugar, simplemente escanea el código QR del evento o abre la URL del proyecto en el navegador (Safari en iOS o Chrome en Android) de tu dispositivo móvil.
