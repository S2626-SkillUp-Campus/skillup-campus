
# SkillUp Campus - Mapeo de funcionalidades

## Funcionalidades del MVP

| Funcionalidad | Tipo de prueba | Prioridad |
|---|---|---|
| Registro de usuario | Funcional / UI / API | Alta |
| Login | Funcional / UI / API | Alta |
| Catálogo público de cursos | Funcional / UI / API | Alta |
| Inscripción a cursos | Funcional / UI / API | Crítica |
| Panel personal del alumno | Funcional / UI / API | Alta |
| Acceso del alumno a sus clases | Funcional / UI / API | Crítica |
| Gestión de usuarios | Funcional / UI / API | Alta |
| Panel de administrador | Funcional / UI / API | Alta |
| Crear cursos | Funcional / UI / API | Alta |
| Editar cursos | Funcional / UI / API | Alta |
| Eliminar cursos | Funcional / UI / API | Crítica |
| Roles y permisos | Funcional / API | Crítica |

## Escenarios borde

### Registro
- Intentar registrarse dejando campos obligatorios vacíos.
- Ingresar un email con formato incorrecto.
- Registrarse utilizando un email ya existente.
- Ingresar una contraseña que no cumpla los requisitos.
- Ingresar contraseñas diferentes cuando se solicita confirmación.
- Ingresar datos con una longitud excesiva.

### Login
- Ingresar una contraseña incorrecta.
- Intentar ingresar con un email inexistente.
- Intentar iniciar sesión dejando campos vacíos.
- Ingresar datos con formato incorrecto.
- Intentar acceder a una sección protegida sin iniciar sesión.

### Catálogo e inscripción
- Intentar acceder a un curso que no existe.
- Intentar inscribirse dos veces al mismo curso.
- Intentar inscribirse sin estar autenticado.
- Intentar acceder a un curso eliminado.

### Panel del alumno
- Intentar acceder al panel sin iniciar sesión.
- Intentar acceder a clases de un curso en el que no está inscripto.
- Intentar acceder a información perteneciente a otro alumno.

### Administrador y seguridad
- Un alumno intenta acceder al panel de administrador.
- Un alumno intenta crear un curso.
- Un alumno intenta editar un curso.
- Un alumno intenta eliminar un curso.
- Un alumno intenta acceder directamente a una URL del administrador.
- Un alumno intenta ejecutar una operación administrativa mediante la API.
- Un usuario no autenticado intenta realizar una operación protegida.

## Funcionalidades fuera de alcance

- Pagos reales.
- Aplicación móvil.
- Streaming o video nativo.
- Chat entre usuarios.
- Certificados.
- Notificaciones automáticas por email.

## Requisitos de autenticación y permisos

* El usuario debe poder registrarse para crear una cuenta.
* El usuario debe iniciar sesión para acceder a las funcionalidades privadas.
* El panel personal del alumno requiere autenticación.
* El panel de administrador y sus funcionalidades requieren autenticación y permisos de administrador.
* El sistema debe diferenciar los permisos entre alumnos y administradores.
* Un alumno no debe poder acceder al panel de administrador.
* Un alumno no debe poder crear, editar ni eliminar cursos.
* Un usuario no autenticado no debe poder ejecutar operaciones protegidas.
* Las operaciones administrativas deben estar protegidas también a nivel de API.

