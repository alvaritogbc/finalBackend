Microservicios con Spring Boot


Este repositorio contiene un conjunto de microservicios desarrollados con Spring Boot. Proporciona funcionalidades como autenticación JWT, documentación de API con Swagger, y se puede desplegar utilizando Docker.

Características
Spring Boot v3.3.1: Framework robusto para el desarrollo de aplicaciones Java.
Docker v26.1.1: Facilita la contenedorización de aplicaciones.
JWT: Tokens JSON Web para una autenticación segura.
Swagger: Herramienta para la documentación de APIs.
Estructura del Proyecto
CrudOrders: Microservicio dedicado a la gestión de órdenes.
CrudProducts: Microservicio dedicado a la gestión de productos.
Requisitos Previos
Java JDK 17 o superior
Docker
Docker Compose
Postman
Dependencias y Versiones
Swagger:

springdoc-openapi-starter-webmvc-ui: 2.5.0
springdoc-openapi-ui: 1.6.14
JWT:

jjwt-api: 0.11.5
jjwt-impl: 0.11.5
jjwt-jackson: 0.11.5
Mockito:

mockito-core: Usando la versión definida por Spring Boot Starter Test
mockito-junit-jupiter: Usando la versión definida por Spring Boot Starter Test
Instalación
Clonar el repositorio:

sh
Copiar código
git clone https://github.com/ezete13/AppSpringBoot-Microservicios.git
Navegar al directorio del proyecto:

sh
Copiar código
cd AppSpringBoot-Microservicios
Construir los contenedores de Docker:

sh
Copiar código
docker-compose build
Levantar los servicios:

sh
Copiar código
docker-compose up
Uso
Accede a la documentación de Swagger:

CrudProducts: http://localhost:8083/swagger-ui/index.html
CrudOrders: http://localhost:8082/swagger-ui/index.html
Endpoints Principales
Autenticación:
POST /auth/login: Iniciar sesión y recibir un token JWT.
POST /auth/register: Registrar un nuevo usuario.
Productos:
GET /products: Obtener la lista de productos.
POST /products: Crear un nuevo producto.
PUT /products/{id}: Actualizar un producto existente.
DELETE /products/{id}: Eliminar un producto.
Órdenes:
GET /orders: Obtener la lista de órdenes.
POST /orders: Crear una nueva orden.
PUT /orders/{id}: Actualizar una orden existente.
DELETE /orders/{id}: Eliminar una orden.
Contribuciones
¡Tu colaboración es bienvenida! Puedes enviar pull requests con nuevas características, mejoras o correcciones de errores.

Créditos
Este proyecto fue desarrollado por Álvaro Durán.

Licencia
Este proyecto está licenciado bajo la Licencia MIT - consulta el archivo LICENSE.md para más detalles.
