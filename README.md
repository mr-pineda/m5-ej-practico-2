# Pagina demo de Hospital Nacional

## Contexto

En este proyecto, los estudiantes deberán implementar el consumo de una API para obtener y mostrar datos del sistema del hospital, como la información de doctores o servicios médicos.
Utilizando useEffect y useState, se espera que realicen peticiones asíncronas, gestionen el estado y manejen los errores de manera eficiente. Podrán utilizar Fetch API o Axios según su preferencia.

Trabajo práctico para desarrollar una página web de hospital que debe contener las siguientes páginas:

1. Vista Principal Home
2. Vista del About
3. Vista de Contact

## Cómo correr el proyecto:

1. Descargar el contenido de este repositorio en el computador. Puede ser clonando el repositorio o descargando el .zip:

   - **Clonar el repositorio**: Puede hacerlo con cualquier gestor de repositorios. Si tiene git instalado, puede abrir una terminal en algun diretorio y ejecutar:

   ```bash
   git clone url_de_este_repo
   ```

   - Si no tiene git instalado puede presionar el botón verde `<> Code` que está en esta página y seleccionar la opción `Download ZIP`.
     1. Descargue el archivo .zip en algun directorio conocido _(ej: Escritorio, Documentos, etc.)_.
     2. Descomprima el archivo .zip

2. Abrir una terminal denntro de la carpeta.
3. Ejecutar `yarn dev` y se mostrará el link para ver la pagina ejecutada en localhost.

## TO-DO (Rúbrica):

1. Protección de Rutas con React Router DOM (1.5 puntos)

   - [x] Implementa seguridad en las rutas del sistema del hospital, asegurando que solo los usuarios autenticados puedan acceder a ciertas secciones (como la gestión del equipo médico o los registros de pacientes).
     - [x] Utiliza React Router DOM para gestionar las rutas protegidas.
     - [x] Asegúrate de que las rutas públicas (como la página principal) sean accesibles sin autenticación.

2. Implementación de Autenticación de Usuarios y Roles (1.5 puntos)

   - [x] Integra un sistema básico de autenticación de usuarios que permita el login en la aplicación del hospital.
     - [x] Los usuarios deben autenticarse para acceder a secciones protegidas.
     - [x] Implementa roles (por ejemplo, doctor y administrador) para que ciertos usuarios solo tengan acceso a áreas específicas según su rol.

3. Consumo de APIs Protegido con API Key y JWT (1.5 puntos)

   - [ ] Asegura el consumo de APIs utilizando una API Key y JWT. Los datos sensibles (como la información de pacientes o citas) deben ser accesibles solo si el usuario ha iniciado sesión y tiene un JWT válido.
     - [ ] Implementa la verificación del token JWT en las solicitudes a la API.
     - [ ] Muestra un mensaje de error si el token no es válido o ha expirado, y redirige al usuario a la página de inicio de sesión.

4. Prevención de Vulnerabilidades Comunes (1.5 puntos)

   - [ ] Implementa medidas de seguridad en la web del hospital para prevenir ataques comunes como:
     - [x] Clickjacking: Protege la aplicación para que no pueda ser incrustada en iframes no autorizados.
     - [ ] XSS (Cross-Site Scripting): Escapa o limpia cualquier entrada del usuario que pueda inyectar código malicioso.
     - [ ] SQL Injection: Asegúrate de que las solicitudes a la API estén protegidas contra inyecciones de SQL.
     - [ ] Ataque DoS: Implementa mecanismos para mitigar posibles ataques de denegación de servicio.

5. Encriptación de Datos en el Front-End (1 punto)

   - [ ] Utiliza técnicas de encriptación de datos para proteger la información sensible en el front-end, como las contraseñas de los usuarios o los datos personales de los pacientes.
     - [ ] Asegúrate de que los datos se encripten antes de ser enviados a la API.
