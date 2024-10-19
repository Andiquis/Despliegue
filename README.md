# Despliegue

Este tutorial describe cómo desplegar aplicaciones web en Internet utilizando **ngrok**.

### Requisitos Previos

1. **XAMPP**: Asegúrate de que el servidor local de XAMPP esté en funcionamiento.  
   - Inicia el servidor local de XAMPP.
   - Obtén el puerto actual en el que está corriendo el servidor local (por defecto, suele ser `80` o `443`).

### Pasos para Desplegar

1. **Descargar ngrok**:
   - Descarga el archivo `ngrok.exe` desde [ngrok.com](https://ngrok.com/).

2. **Autenticación**:
   - Inicia sesión en la página de ngrok y obtén tu token de autenticación.
   - Agrega el token en la terminal de Windows con el siguiente comando:
     ```
     ngrok config add-authtoken YOUR_AUTHTOKEN  ó ./ngrok.exe config add-authtoken YOUR_AUTHTOKEN
     ```

3. **Iniciar ngrok**:
   - Ejecuta el siguiente comando en la terminal, reemplazando `<PUERTO_DE_TU_SERVIDOR_XAMP>` con el puerto que obtuviste anteriormente:
     ```
     ./ngrok http <PUERTO_DE_TU_SERVIDOR_XAMP>
     ```

### Resultados

Una vez que el servidor esté corriendo, deberías ver un mensaje similar a:

Forwarding https://d2b2-181-176-94-45.ngrok-free.app -> https://localhost:<PUERTO>
- **Enlace de acceso a tu aplicación**:  
  Accede a tu aplicación utilizando la siguiente URL (especifica la ruta según tu proyecto):  


https://d2b2-181-176-94-45.ngrok-free.app/proyecto/index.php


- **Enlace de control de ngrok**:  
Controla tu sesión de ngrok desde la siguiente URL:  
https://localhost:<PUERTO>
