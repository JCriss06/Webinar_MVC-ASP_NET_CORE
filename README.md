# Taller ASP-NET Core

Este repositorio alberga una aplicación web dinámica, diseñada para la **administración eficiente de listas de tareas**. El proyecto se desarrolló utilizando la plataforma **ASP.NET Core** y sigue rigurosamente el patrón **Modelo-Vista-Controlador (MVC)**.

---
### Funcionalidades Clave

La aplicación incluye las siguientes capacidades esenciales para la gestión de datos y usuarios:

* *Autenticación de Usuarios:* Se requiere un proceso de inicio de sesión para garantizar que **cada usuario acceda únicamente a su lista de tareas privada**.
* **Modelo de Persistencia con CRUD:** Implementación completa de las cuatro operaciones básicas de la base de datos:
    * **Creación (Create):** Permite ingresar nuevas tareas.
    * **Lectura (Read):** Muestra una visualización clara de las tareas existentes.
    * **Actualización (Update):** Facilita la modificación de los detalles de cualquier tarea.
    * **Eliminación (Delete):** Proporciona la opción de remover tareas de la lista.
* **Mecanismos de Búsqueda y Ordenamiento:** La lista de tareas puede ser **filtrada por criterios como prioridad** o **reordenada** para mejorar la organización.

---

## Instrucciones para ejecutar el Proyecto

Sigue estos pasos para configurar y ejecutar la aplicación en tu entorno local:

### 1. Obtener el Código Fuente

Utiliza Git para clonar el repositorio en tu máquina:
```bash
git clone [https://github.com/tu-usuario/nombre-del-repositorio.git](https://github.com/tu-usuario/nombre-del-repositorio.git)
```
### 2. Abrir la Solución
Carga el proyecto dentro de tu entorno de desarrollo preferido, ya sea Visual Studio o Visual Studio Code.

### 3. Preparación de la Base de Datos
El proyecto utiliza SQLite y Entity Framework Core para la base de datos.
* Verifica la cadena de conexión en el archivo appsettings.json.
* Asegúrate de que las migraciones estén aplicadas ejecutando el siguiente comando desde la terminal en la carpeta raíz del proyecto:
```bash
Bashdotnet ef database update
```

### 4. Inicializar y Acceder a la Aplicación
Ejecuta el proyecto desde la terminal:
```bash
dotnet run
```
La aplicación se cargará en el navegador. Por defecto, puedes acceder a ella en: http://localhost:5000 (o la dirección que te indique la consola, como https://localhost:7151).

---

## Tecnologías Empleadas
El desarrollo se basó en el siguiente stack tecnológico:
* Framework: ASP.NET Core 7.0 
* ORM: Entity Framework Core 
* Base de Datos: SQLite
* Estilos: Bootstrap para un diseño responsivo 
* Lenguaje Principal: C#
---
## Estructura del Repositorio
La organización del proyecto se adhiere al estándar MVC de ASP.NETCore:
* Controllers/ - Manejadores de la lógica de la aplicación (Controladores MVC)
* Models/ - Definiciones de datos y lógica de negocio 
* Views/ - Plantillas de la interfaz de usuario (Vistas Razor) 
* wwwroot/ - Almacena los recursos web estáticos (CSS, JS, imágenes) 
* appsettings.json - Contiene la configuración de la aplicación, como la cadena de conexión a la base de datos 
* README.md - Documentación esencial del proyecto
