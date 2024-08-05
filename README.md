# BusinessTracker

BusinessTracker es una aplicación web desarrollada en Java que permite la gestión de empresas y productos, así como el control del stock. Utiliza varias tecnologías modernas para proporcionar una solución robusta y eficiente para la administración de datos empresariales.

## Características

- **Gestión de Empresas:** Alta, edición y listado de empresas.
- **Gestión de Productos:** Alta, edición y listado de productos.
- **Gestión de Stock:** Registro y gestión del inventario de productos.
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

- **src/main/java/com/masanz/ut2/businesstracker:**
  - **ServerMain.java:** Clase principal para iniciar el servidor.
  - **dao/:** Clases DAO para la gestión de datos.
    - `EmpresasDao.java`
    - `ProductosDao.java`
    - `StockDao.java`
  - **db/:** Inicialización de la base de datos.
    - `InicializarDb.java`
  - **dto/:** Clases DTO para transferir datos.
    - `Empresa.java`
    - `Producto.java`
    - `Stock.java`
  - **service/:** Lógica de negocio.
    - `Tareas.java`

- **resources/:**
  - `create-tables.sql:` Script SQL para la creación de tablas.
  - `log4j2.xml:` Configuración de Log4j2.
  - **templates/:** Plantillas FreeMarker para las vistas.

- **public/:**
  - `bootstrap.min.css:` Estilos CSS.
  - `bootstrap.bundle.min.js:` JavaScript de Bootstrap.

## Requisitos Previos

- **JDK 8 o superior**
- **Maven 3.6.0 o superior**
- **IntelliJ IDEA** (opcional, pero recomendado)

## Instalación
   ```sh
   git clone <URL del repositorio>
   cd BusinessTracker
   mvn clean install
   mvn exec:java -Dexec.mainClass="com.masanz.ut2.businesstracker.ServerMain"
  ```
Contribuciones
Las contribuciones son bienvenidas. Para contribuir, por favor sigue estos pasos:

Realiza un fork del repositorio.
Crea una rama con la nueva funcionalidad (git checkout -b nueva-funcionalidad).
Realiza los cambios necesarios y haz commit (git commit -am 'Añadir nueva funcionalidad').
Sube los cambios a tu fork (git push origin nueva-funcionalidad).
Crea un Pull Request para revisar los cambios.
