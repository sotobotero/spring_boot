# Spring Boot Person CRUD API with Dozer Mapper
[![Powered by @sotobotero](https://img.shields.io/badge/Powered%20by-%40sotobotero-blue?style=flat-square&logo=twitter)](https://twitter.com/sotobotero)
[![Sotobotero.com](https://img.shields.io/badge/Powered%20by-sotobotero.com-blue?style=flat-square&logo=twitter)](https://sotobotero.com/)

🌟 **Contribuye y Mejora este Proyecto**
¡Este proyecto está en constante evolución y cualquier mejora es bienvenida! 🎉 Si encuentras algo que se pueda optimizar, tienes una idea o quieres corregir errores, no dudes en participar.
📌 Consulta el apartado [Cómo Contribuir](#-cómo-contribuir) para español or [How to Contribute](#-how-to-contribute) for English.


## Descripción
This project is a REST API example built with Spring Boot that demonstrates CRUD operations for managing person data. The application uses Dozer Mapper to efficiently map between domain objects and DTOs, maintaining a clean architecture.

## Features
- Complete CRUD operations for person data
- REST API with best practices implementation
- Object mapping with Dozer Mapper
- Clean, scalable architecture for Spring Boot learners

## Requirements
- Java 8+
- Maven

## Setup
1. Clone the repository:
  ```bash
  git clone https://github.com/sotobotero/spring_boot.git
  ```
2. Navigate to the project directory:
  ```bash
  cd spring_boot
  ```
3. Build and run the application:
  ```bash
  mvn clean install
  mvn spring-boot:run
  ```
## API Usage
### Endpoints
- `GET /person` - Retrieve all persons
  ```bash
  curl -X GET http://localhost:8080/person
  ```
- `GET /person/{id}` - Retrieve a specific person
  ```bash
  curl -X GET http://localhost:8080/person/{id}
  ```

- `POST /person` - Create a new person
  ```bash
  curl -X POST http://localhost:8080/person -H "Content-Type: application/json" -d '{
    "firstName": "John",
    "lastName": "Doe",
    "email": "john.doe@example.com"
  }'
  ```

- `PUT /person/{id}` - Update an existing person
  ```bash
  curl -X PUT http://localhost:8080/person/{id} -H "Content-Type: application/json" -d '{
    "firstName": "John",
    "lastName": "Doe",
    "email": "john.doe@example.com"
  }'
  ```

- `DELETE /person/{id}` - Delete a person
  ```bash
  curl -X DELETE http://localhost:8080/person/{id}
  ```

### Request Example

#### POST /person
```json
{
  "firstName": "John",
  "lastName": "Doe",
  "email": "john.doe@example.com"
}
```
## 🚀 How to Contribute

1. **Fork the Repository**
  Click the "Fork" button in the upper right corner of the repository on GitHub.

2. **Clone Your Fork to Your Computer**
  Open a terminal and run:
  ```bash
  git clone https://github.com/your-username/repository-name.git
  ```
3. Then navigate to the cloned repository directory:
  ```bash
  cd repository-name
  ```

4. **Create a New Branch**
  ```bash
  git checkout -b my-new-branch
  ```

5. **Make Your Changes**
  - Edit the necessary files.
  - Follow the project's conventions.

6. **Save Your Changes**
  Add the modified files and commit:
  ```bash
  git add .
  git commit -m "Brief description of your change"
  ```

7. **Keep Your Branch Updated**
  Ensure you have the latest version of the original repository:
  ```bash
  git remote add upstream https://github.com/original-user/repository-name.git
  git fetch upstream
  git rebase upstream/main
  ```

8. **Push Your Changes to GitHub**
  ```bash
  git push origin my-new-branch
  ```

9. **Create a Pull Request (PR)**
  - Go to your repository on GitHub.
  - Click "Compare & pull request".
  - In the branch section, select your branch as the source.
    Ensure the target branch is the main (or master) branch of the original repository.
  - Write a clear title and description.
  - Click "Create pull request".

10. **Wait for Review**
  The maintainers will review your PR and may request changes. Respond to their comments and adjust your code if necessary.

🎉 **Congratulations!**
If your PR is approved, it will be merged into the original repository. You have contributed to an open-source project! 🚀

## License

This project is open source under the [Licencia MIT](LICENSE).

# Version en Español
## 🚀 Cómo Contribuir
1. **Haz un Fork del Repositorio**
  Haz clic en el botón "Fork" en la esquina superior derecha del repositorio en GitHub.

2. **Clona tu Fork en tu Computadora**
  Abre una terminal y ejecuta:
  ```bash
  git clone https://github.com/tu-usuario/nombre-del-repositorio.git
  ```
3. Luego navega al directorio del repositorio clonado:
  ```bash
  cd nombre-del-repositorio
  ```
4. **Crea una Nueva Rama**
  ```bash
  git checkout -b mi-nueva-rama
  ```
5. **Realiza tus Cambios**
  - Edita los archivos necesarios.
  - Sigue las convenciones del proyecto.
6. **Guarda tus Cambios**
  Añade los archivos modificados y realiza un commit:
  ```bash
  git add .
  git commit -m "Descripción breve de tu cambio"
  ```
7. **Mantén tu Rama Actualizada**
  Asegura que tienes la última versión del repositorio original:
  ```bash
  git remote add upstream https://github.com/usuario-original/nombre-del-repositorio.git
  git fetch upstream
  git rebase upstream/main
  ```
8. **Sube tus Cambios a GitHub**
  ```bash
  git push origin mi-nueva-rama
  ```
9. **Crea un Pull Request (PR)**
  - Ve a tu repositorio en GitHub.
  - Haz clic en "Compare & pull request".
  - En la sección de ramas, selecciona tu rama como origen.
    Asegúrate de que la rama de destino sea la rama principal (main o master) del repositorio original.
  - Escribe un título y una descripción clara.
  - Haz clic en "Create pull request".
10. **Espera la Revisión**
  Los mantenedores revisarán tu PR y pueden solicitar cambios. Responde a sus comentarios y ajusta tu código si es necesario.
🎉 **¡Felicitaciones!**
Si tu PR es aprobado, se fusionará al repositorio original. ¡Has contribuido a un proyecto de código abierto! 🚀