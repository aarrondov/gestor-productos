# CommerceSystem

CommerceSystem es una aplicación web desarrollada en Java que permite la gestión de artículos, compras y usuarios. Utiliza varias tecnologías modernas para proporcionar una solución robusta y eficiente para la administración de datos comerciales.

## Características

- **Gestión de Artículos:** Alta, edición y listado de artículos.
- **Gestión de Compras:** Registro y gestión de compras.
- **Gestión de Usuarios:** Alta, edición y listado de usuarios.
- **Interfaz de Usuario:** Formularios y vistas para interactuar con la aplicación.

## Tecnologías Utilizadas

- **Java:** Lenguaje principal del proyecto.
- **Maven:** Gestión de dependencias y construcción del proyecto.
- **FreeMarker:** Motor de plantillas para generar vistas HTML dinámicas.
- **Log4j2:** Biblioteca para el registro de logs.
- **SQL:** Scripts para la creación de tablas en la base de datos.
- **Bootstrap:** Biblioteca CSS/JS para estilos y componentes web.
- **IntelliJ IDEA:** Configuraciones específicas para esta IDE.

## Estructura del Proyecto

- **src/main/java/com/masanz/ut2/commercesystem:**
  - **ServerMain.java:** Clase principal para iniciar el servidor.
  - **dao/:** Clases DAO para la gestión de datos.
    - `ArticulosDao.java`
    - `ComprasDao.java`
    - `UsuariosDao.java`
  - **database/:** Gestión de la base de datos.
    - `DatabaseManager.java`
  - **dto/:** Clases DTO para transferir datos.
    - `Articulo.java`
    - `Compras.java`
    - `Usuario.java`
  - **model/:** Modelos de datos.
    - `Articulo.java`

- **resources/:**
  - `create-tables.sql:` Script SQL para la creación de tablas.
  - `log4j2.xml:` Configuración de Log4j2.
  - **templates/:** Plantillas FreeMarker para las vistas.
    - `articulos.ftl`
    - `home.ftl`
    - `login.ftl`
    - `usuario.ftl`
    - `usuarios.ftl`

## Requisitos Previos

- **JDK 8 o superior**
- **Maven 3.6.0 o superior**
- **IntelliJ IDEA** (opcional, pero recomendado)

## Instalación

1. **Clonar el repositorio:**
   ```sh
   git clone <URL del repositorio>
   cd CommerceSystem
   ```
2. **Compilar el proyecto con Maven:**
    ```sh
   mvn clean install
   ```
3. **Ejecutar la aplicación:**
   ```sh
   mvn exec:java -Dexec.mainClass="com.masanz.ut2.commercesystem.ServerMain"
   ```
