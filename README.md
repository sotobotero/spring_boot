# Proyecto CRUD de Personas con Spring Boot y Dozer Mapper

Este repositorio es un proyecto de ejemplo creado en **Spring Boot** para gestionar un CRUD (Crear, Leer, Actualizar y Eliminar) de datos sobre personas a través de una API REST. La aplicación utiliza **Dozer Mapper** para el mapeo de objetos de dominio a DTOs, facilitando la conversión de datos y manteniendo una arquitectura limpia y organizada. Este proyecto está diseñado para ser una guía práctica para estudiantes y desarrolladores interesados en aprender sobre el desarrollo de APIs con Spring Boot.

## Características

- **CRUD completo** sobre los datos de personas.
- **API REST** diseñada con buenas prácticas de desarrollo.
- **Mapeo de objetos con Dozer Mapper**, separando las capas de dominio y transporte.
- **Arquitectura limpia y escalable**, ideal para nuevos desarrolladores en Spring Boot.

## Requisitos previos

- **Java 8** o superior
- **Maven** para la gestión de dependencias

## Instalación

1. Clona el repositorio:
   ```bash
   git clone https://github.com/usuario/repo-ejemplo.git
```md
## Navega al directorio del proyecto:
```bash
cd repo-ejemplo
```

## Compila el proyecto y descarga las dependencias:
```bash
mvn clean install
```

## Inicia la aplicación:
```bash
mvn spring-boot:run
```

## Uso de la API
Una vez que la aplicación está en ejecución, puedes probar la API usando herramientas como Postman o curl.

### Endpoints
- **GET** `/api/personas` - Obtener la lista de personas.
- **POST** `/api/personas` - Crear una nueva persona.
- **PUT** `/api/personas/{id}` - Actualizar los datos de una persona.
- **DELETE** `/api/personas/{id}` - Eliminar una persona.

### Ejemplo de solicitud para crear una persona:
```json
POST /api/personas
{
  "nombre": "Juan",
  "apellido": "Pérez",
  "email": "juan.perez@example.com"
}
```

## Contribuir
Las contribuciones son bienvenidas. Puedes contribuir de las siguientes maneras:
1. Forkea el repositorio.
2. Crea una rama para tu contribución.
3. Realiza un pull request y explícanos tu mejora.

## Licencia
Este proyecto está disponible como código abierto bajo la [Licencia MIT](LICENSE).
