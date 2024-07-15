# API de Foro - Documentación

## Descripción
Esta API proporciona funcionalidades para administrar un foro, permitiendo a los usuarios autenticarse, gestionar temas, publicar respuestas, y administrar usuarios. Está diseñada para simular las operaciones internas de un sistema de foro.

## Propósito
El propósito principal de este proyecto es ofrecer una interfaz backend robusta para la gestión de interacciones de usuarios en un foro virtual. Permite registrar usuarios, crear y actualizar temas, y gestionar respuestas asociadas a estos temas.

## Tecnologías Utilizadas
- Java
- Spring Boot
- Spring Security
- Spring Data JPA
- Hibernate
- JWT para autenticación
- Base de datos relacional (se debe especificar el motor de base de datos utilizado, si aplica)

## Estructura del Proyecto
El proyecto está estructurado en varios controladores REST que manejan diferentes aspectos de la funcionalidad del foro:

- **Autenticación**: Gestión de autenticación de usuarios.
- **Temas**: Creación, actualización, listado y eliminación de temas.
- **Respuestas**: Publicación, actualización, listado y eliminación de respuestas asociadas a temas.
- **Usuarios**: Registro, actualización, listado y eliminación de usuarios.
- **Manejo de Errores**: Gestión de errores comunes mediante un manejador global.

## Endpoints Principales
- **Autenticación**: `POST /login`
- **Temas**: 
  - `POST /topicos`: Crear un nuevo tema.
  - `GET /topicos`: Obtener la lista de temas.
  - `GET /topicos/{id}`: Obtener detalles de un tema específico.
  - `PUT /topicos`: Actualizar un tema existente.
  - `DELETE /topicos/{id}`: Eliminar un tema existente.
- **Respuestas**: 
  - `POST /respuestas`: Publicar una nueva respuesta.
  - `GET /respuestas`: Obtener la lista de respuestas.
  - `GET /respuestas/{id}`: Obtener detalles de una respuesta específica.
  - `PUT /respuestas`: Actualizar una respuesta existente.
  - `DELETE /respuestas/{id}`: Eliminar una respuesta existente.
- **Usuarios**: 
  - `POST /usuarios`: Registrar un nuevo usuario.
  - `GET /usuarios`: Obtener la lista de usuarios.
  - `GET /usuarios/{id}`: Obtener detalles de un usuario específico.
  - `PUT /usuarios`: Actualizar un usuario existente.
  - `DELETE /usuarios/{id}`: Eliminar un usuario existente.
