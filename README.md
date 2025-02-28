# Dashboard Seguro - Migración de Funciones

Este proyecto es un panel de administración seguro diseñado para gestionar la migración de funciones entre bases de datos de PostgreSQL. A través de una interfaz de usuario interactiva y fácil de usar, se pueden configurar los detalles de las bases de datos de origen y destino, así como las funciones a migrar.

## Propósito

El propósito de este sistema es facilitar la migración de funciones almacenadas en PostgreSQL de una base de datos de origen a una base de datos de destino. Los usuarios pueden ingresar la configuración necesaria (como la IP, puerto, usuario y contraseña de las bases de datos) y seleccionar la base de datos y funciones a migrar.

## Funcionalidad

- **Configuración de la Base de Datos de Destino:**
  - IP del servidor PostgreSQL de destino.
  - Puerto del servidor.
  - Usuario y contraseña para autenticarse en el servidor.
  - Selección de bases de datos a replicar.
  
- **Configuración de la Base de Datos de Origen:**
  - IP del servidor PostgreSQL de origen.
  - Puerto del servidor.
  - Usuario y contraseña para autenticarse en el servidor.
  - Nombre de la base de datos de origen.

- **Configuración de la Función:**
  - Esquema donde se encuentra la función.
  - Nombre de la función a migrar.
  - Tipo de retorno de la función.
  - Argumentos de entrada necesarios para la ejecución de la función.

- **Ejecutar SQL:**
  - Permite ejecutar la función seleccionada en el servidor de origen y replicarla en el servidor de destino.

## Interfaz de Usuario

La interfaz está dividida en tres secciones principales, cada una representada por una pestaña:

1. **Destino:** Permite configurar el servidor PostgreSQL de destino, incluyendo la IP, puerto, usuario, contraseña y las bases de datos que se desean replicar.
2. **Origen:** Permite configurar el servidor PostgreSQL de origen, especificando la IP, puerto, usuario, contraseña y la base de datos de origen.
3. **Función:** Permite configurar los detalles de la función a migrar, como el esquema, nombre de la función, tipo de retorno y argumentos de entrada.

## Instrucciones de Uso

1. **Acceso:** El usuario debe estar autenticado en el sistema para acceder al panel.
2. **Configuración del Destino:**
   - Rellenar los campos con la IP, puerto, usuario y contraseña del servidor PostgreSQL de destino.
   - Seleccionar las bases de datos a replicar.
3. **Configuración del Origen:**
   - Rellenar los campos con la IP, puerto, usuario y contraseña del servidor PostgreSQL de origen.
   - Ingresar el nombre de la base de datos de origen.
4. **Configuración de la Función:**
   - Especificar el esquema, nombre de la función, tipo de retorno y los argumentos necesarios.
5. **Ejecutar SQL:** Después de configurar todas las opciones, hacer clic en el botón "Ejecutar SQL" para realizar la migración.

## Tecnologías Utilizadas

- **Bootstrap 5:** Para la interfaz de usuario, proporcionando una experiencia responsive y moderna.
- **Laravel (Backend):** Para la gestión de la lógica de migración de datos entre las bases de datos.
- **PostgreSQL:** Como sistema de gestión de bases de datos.
- **AJAX (JavaScript):** Para cargar dinámicamente las bases de datos disponibles en el servidor de destino.

## Instalación

1. Usa el repositorio:
   ```bash
   https://devops.tiquetevirtual.com
