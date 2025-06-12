# OrbitSong

## Descripción General

OrbitSong es una aplicación móvil de música en desarrollo, diseñada para ofrecer una experiencia de usuario fluida para la gestión y reproducción de contenido musical. Esta aplicación se conecta a una API RESTful personalizada desarrollada con **Spring Boot**, que a su vez se encarga de la interacción con la base de datos **MySQL** para el almacenamiento y recuperación de toda la información relacionada con los usuarios, canciones, artistas y listas de reproducción.

## Características Principales (en desarrollo)

* **Gestión de Usuarios:** Permite a los usuarios registrarse, iniciar sesión y gestionar sus perfiles.
* **Exploración de Música:** Posibilidad de buscar y explorar canciones, álbumes y artistas.
* **Listas de Reproducción:** Creación y gestión de listas de reproducción personalizadas.
* **Reproducción de Audio:** Integración para la reproducción de archivos de audio (funcionalidad a ser implementada).
* **Conexión a API:** Interacción con un backend robusto para el manejo de datos.

## Arquitectura

La aplicación sigue una arquitectura cliente-servidor:

* **Frontend (Aplicación Móvil):** Desarrollada en Android (Java), se encarga de la interfaz de usuario y la lógica de presentación.
* **Backend (API RESTful):** Desarrollada con **Spring Boot**, sirve como intermediario entre la aplicación móvil y la base de datos. Se encarga de la lógica de negocio, la autenticación y la autorización.
* **Base de Datos:** **MySQL**, gestionada a través de MySQL Workbench, almacena toda la información persistente de la aplicación (usuarios, canciones, etc.).

## Tecnologías Utilizadas

### Frontend (Android)
* **Lenguaje de Programación:** Java
* **Frameworks/Librerías:** Retrofit (para la comunicación con la API), Glide (o similar para carga de imágenes), etc.

### Backend (API)
* **Framework:** Spring Boot
* **Lenguaje de Programación:** Java
* **Base de Datos:** MySQL

### Base de Datos
* **Sistema de Gestión de Bases de Datos (SGBD):** MySQL
* **Herramienta de Gestión:** MySQL Workbench

## Estructura del Proyecto (Frontend - Android)

El proyecto Android está organizado de la siguiente manera:

* `app/src/main/java/com/example/orbitsong`: Contiene el código fuente de la aplicación.
    * `activities`: Actividades principales de la aplicación (ej. `GenerarActivity`, `InicioSesionActivity`, `RegistroActivity`).
    * `api`: Clases relacionadas con la comunicación con la API.
        * `ApiClient`: Cliente HTTP para realizar peticiones.
        * `ApiService`: Interfaz que define los endpoints de la API.
    * `models`: Clases que representan los modelos de datos (ej. `Usuario`).
* `app/src/main/res`: Recursos de la aplicación (layouts, drawables, valores, etc.).

## Instalación y Configuración (Para desarrollo)

### Requisitos
* Android Studio
* Java Development Kit (JDK)
* Un emulador de Android o un dispositivo físico.
* MySQL Workbench (para la gestión de la base de datos).
* Un entorno de desarrollo para Spring Boot (IDE como IntelliJ IDEA o Eclipse con Spring Tools Suite, Maven o Gradle).

### Pasos
1.  **Clonar los repositorios:**
    ```bash
    git clone [https://github.com/tu-usuario/OrbitSong-App.git](https://github.com/tu-usuario/OrbitSong-App.git)
    git clone [https://github.com/tu-usuario/OrbitSong-API.git](https://github.com/tu-usuario/OrbitSong-API.git) # Asume un repositorio separado para la API
    ```
2.  **Configurar la Base de Datos (MySQL):**
    * Crea una base de datos en MySQL (ej. `orbitsong_db`).
    * Importa el script SQL de tu esquema de base de datos (si lo tienes) usando MySQL Workbench o línea de comandos.
    * Asegúrate de que las credenciales de la base de datos en tu aplicación Spring Boot sean correctas.
3.  **Configurar y Ejecutar el Backend (Spring Boot API):**
    * Abre el proyecto `OrbitSong-API` en tu IDE (ej. IntelliJ IDEA).
    * Revisa el archivo `application.properties` (o `application.yml`) para configurar la conexión a tu base de datos MySQL (URL, usuario, contraseña).
    * Ejecuta la aplicación Spring Boot. Por defecto, suele ejecutarse en el puerto 8080.
4.  **Configurar y Ejecutar el Frontend (Android App):**
    * Abre el proyecto `OrbitSong-App` en Android Studio.
    * En la clase `ApiClient` (o donde definas la URL base de tu API), asegúrate de que la URL apunte a tu servidor Spring Boot (ej. `http://10.0.2.2:8080/` para emuladores de Android que apuntan a localhost, o la IP de tu máquina si usas un dispositivo físico).
    * Sincroniza Gradle (`Sync Project with Gradle Files`).
    * Selecciona un emulador o un dispositivo conectado y ejecuta la aplicación.

## Capturas de Pantalla / Prototipos

Aquí puedes ver algunos prototipos e interfaces iniciales de la aplicación OrbitSong:

* **Pantalla de Inicio de Sesión:**
    ![Pantalla de Inicio de Sesión](URL_DE_TU_IMAGEN_DE_LOGIN.png)

* **Pantalla de Registro:**
    ![Pantalla de Registro](URL_DE_TU_IMAGEN_DE_REGISTRO.png)

* **Pantalla Principal (Ejemplo):**
    ![Pantalla Principal](URL_DE_TU_IMAGEN_PRINCIPAL.png)

## Contribuciones

¡Las contribuciones son bienvenidas! Si deseas contribuir, por favor:

1.  Haz un fork del repositorio.
2.  Crea una nueva rama (`git checkout -b feature/nueva-funcionalidad`).
3.  Realiza tus cambios y commitea (`git commit -am 'Add new functionality'`).
4.  Haz push a la rama (`git push origin feature/nueva-funcionalidad`).
5.  Crea un nuevo Pull Request.

## Licencia

Este proyecto está bajo la Licencia [MIT / Apache 2.0 / etc.]. Consulta el archivo `LICENSE` para más detalles.

## Contacto
