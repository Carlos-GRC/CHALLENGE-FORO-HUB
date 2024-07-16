# FORO HUB API

## Descripción
Esta API forma parte del curso de Backend con Java y Spring Boot en Alura en colaboración con Oracle. Su objetivo es gestionar consultas desde el lado del cliente en un entorno de foro, utilizando HTTP y bases de datos MySQL. El desarrollo se realiza con Java, Spring Boot, JPA y Hibernate.

Para acceder al foro, los usuarios deben registrarse. Al registrarse, se les asigna automáticamente el rol de usuario "USER". Los usuarios con este rol tienen acceso restringido a ciertas consultas, mientras que los usuarios con rol "ADMIN" tienen permisos completos. Las contraseñas de los usuarios se almacenan encriptadas con BCrypt. La autenticación se realiza mediante tokens, manteniendo sesiones STATELESS. Los usuarios pueden crear, actualizar y eliminar tópicos del foro, así como responder a ellos y cerrarlos cuando se considere necesario. Los tópicos están asociados a cursos o lecciones específicas.
## Funcionalidades
La API permite:

- Registro y autenticación de usuarios
- Creación de nuevos mensajes (con validación para evitar duplicados de título y contenido)
- Listado de todos los tópicos
- Consulta de un tópico específico
- Actualización y borrado de mensajes

## Tecnologías Utilizadas
- Spring Boot
- Spring Security
- JWT (JSON Web Tokens)
- JPA (Java Persistence API)
- Flyway (Control de versiones de bases de datos)
- MySQL
- Lombok (Para reducir el código boilerplate)
