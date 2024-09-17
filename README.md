# Servicio de Gestión de Inventario

## Descripción

El **Servicio de Gestión de Inventario** es un microservicio que gestiona el inventario de productos en un sistema de pedidos. Permite agregar productos, obtener información sobre ellos y actualizar la cantidad disponible. Este servicio es parte de una arquitectura de microservicios y se integra con otros servicios como el Servicio de Gestión de Pedidos y el Servicio de Notificaciones.

## Características

- **Agregar Producto**: Permite añadir nuevos productos al inventario.
- **Obtener Producto**: Recupera información sobre un producto específico.
- **Actualizar Cantidad**: Actualiza la cantidad disponible de un producto.

## Tecnologías

- **Spring Boot**: Framework para la creación de aplicaciones Java.
- **Spring Data JPA**: Para la persistencia de datos en la base de datos.

## Requisitos

- **Java 17** o superior
- **Maven** o **Gradle** (para la gestión de dependencias y construcción del proyecto)
- **Base de Datos**: Configurada en el archivo `application.properties`

## Configuración

### Archivo de Configuración

El archivo de configuración principal es `src/main/resources/application.properties`. Asegúrate de configurar correctamente los parámetros de la base de datos.

Ejemplo de configuración:

```properties
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.username=sa
spring.datasource.password=password
spring.jpa.hibernate.ddl-auto=update
spring.h2.console.enabled=true
