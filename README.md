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
1.  **https://github.com/junior514/APIMusic**

## Capturas de Pantalla / Prototipos

Aquí puedes ver algunos prototipos e interfaces iniciales de la aplicación OrbitSong:

* **Pantalla de Inicio de Sesión:**
    ![Pantalla de Inicio de Sesión](URL_DE_TU_IMAGEN_DE_LOGIN.png)

* **Pantalla de Registro:**
    ![Pantalla de Registro](URL_DE_TU_IMAGEN_DE_REGISTRO.png)

* **Pantalla Principal (Ejemplo):**
    ![Pantalla Principal](URL_DE_TU_IMAGEN_PRINCIPAL.png)

## Integrantes


1.  Paico Valverde Brayan.
2.  Paico Valverde Junior.
3.  Frans Espinoza Pilco
4.  Garcia Bracho Maickel Adrian
5.  Cristhoper Thomy Gotto Santa Cruz


