```markdown
# Literalura 📚

Literalura es una aplicación de consola desarrollada en Java que permite explorar y registrar libros desde la API de Gutendex.  
Forma parte del desafío del programa Oracle ONE en Alura LATAM y combina conceptos como consumo de API REST, persistencia en base de datos, y uso de JPA.

## 🚀 Funcionalidades

- Buscar libros por título usando la API de Gutendex.
- Guardar libros en una base de datos local (PostgreSQL).
- Consultar libros por:
  - Título
  - Autor
  - Idioma
  - Año de publicación
- Listar todos los libros registrados en la base de datos.
- Interfaz de consola amigable.

## 🧰 Tecnologías y herramientas

- Java 17
- Spring Boot
- Spring Data JPA
- PostgreSQL
- API Rest de [Gutendex](https://gutendex.com/)
- Maven

## 🗄️ Estructura del Proyecto

- `Main`: Punto de entrada de la aplicación.
- `Principal`: Lógica principal de interacción con el usuario.
- `modelo`: Clases que representan las entidades como Libro y Autor.
- `repositorio`: Interfaces JPA para la persistencia.
- `servicio`: Lógica de negocio y conexión con la API externa.

## ⚙️ Configuración e instalación

1. Clona el repositorio:

   ```bash
   git clone https://github.com/Itemt/literalura.git
   cd literalura
   ```

2. Asegúrate de tener PostgreSQL en funcionamiento y crea una base de datos:

   ```sql
   CREATE DATABASE literalura;
   ```

3. Configura el archivo `application.properties` con tus credenciales de PostgreSQL:

   ```properties
   spring.datasource.url=jdbc:postgresql://localhost:5432/literalura
   spring.datasource.username=tu_usuario
   spring.datasource.password=tu_contraseña
   spring.jpa.hibernate.ddl-auto=update
   ```

4. Compila y ejecuta la aplicación:

   ```bash
   mvn clean install
   mvn spring-boot:run
   ```

## 📌 Notas

- La API de Gutendex solo está disponible en inglés, por lo que los resultados pueden variar dependiendo del título ingresado.
- Puedes extender esta aplicación agregando validaciones, interfaz gráfica o exportación de datos.

## 📄 Licencia

Este proyecto está bajo la Licencia MIT.

---

¡Gracias por visitar este proyecto! Si deseas colaborar o reportar un problema, no dudes en abrir un issue o pull request. 🚀
```
