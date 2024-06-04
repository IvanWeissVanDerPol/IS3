
# Casos de Pruebas
Para seleccionar las funciones más importantes del sistema y realizar pruebas exhaustivas, es necesario identificar aquellas funcionalidades que son críticas para el funcionamiento y la usabilidad del sistema. A continuación, se enumeran algunas de las funciones más importantes basadas en los requerimientos funcionales y el contexto general del sistema:

## Funcionalidades mas importantes
1. **Inicio de Sesión y Autenticación**
   - **RF-02**: El sistema permitirá el inicio de sesión mediante una aplicación dedicada a este propósito con la provisión de un username y password.
   - **RF-03**: La aplicación de inicio de sesión del sistema verificará que las credenciales proporcionadas por el usuario son correctas y válidas.

2. **Gestión de Usuarios**
   - **RF-06**: El sistema permitirá la visualización del perfil de usuario.
   - **RF-19**: El sistema permitirá asignar roles a los usuarios.

3. **Publicación de Contenidos**
   - **RF-24**: El sistema deberá permitir crear contenido dentro de una categoría.
   - **RF-27**: El sistema permitirá al autor visualizar sus publicaciones dentro de la pestaña “Mi perfil”.
   - **RF-28**: El sistema deberá permitir crear nuevos contenidos de texto.

4. **Interacción con Publicaciones**
   - **RF-33**: El sistema permitirá la posibilidad de dar likes a una publicación.
   - **RF-34**: El sistema deberá permitir compartir publicaciones.
   - **RF-31**: El sistema deberá permitir a los usuarios comentar publicaciones.

5. **Gestión de Categorías**
   - **RF-25**: El sistema deberá permitir crear nuevas categorías.
   - **RF-36**: El administrador podrá crear categorías.

6. **Flujo de Aprobación**
   - **RF-41**: El sistema permitirá el cambio de estado de una publicación de “En revisión” a “Publicado”.
   - **RF-42**: El sistema permitirá el cambio de estado de una publicación de “En revisión” a “Rechazado”.


# Casos de Prueba Propuestos

## Inicio de Sesión y Autenticación

### Prueba de inicio de sesión con credenciales válidas (RF-02, RF-03)
- **Objetivo**: Verificar que el sistema permite el inicio de sesión con credenciales válidas.
- **Precondiciones**: El usuario debe tener una cuenta registrada en el sistema.
- **Datos de Prueba**:
  - Usuario: usuario_valido
  - Contraseña: contraseña_valida
- **Pasos**:
  1. Navegar a la página de inicio de sesión.
  2. Ingresar el nombre de usuario y la contraseña válidos.
  3. Hacer clic en el botón "Iniciar sesión".
- **Resultado Esperado**: El usuario es redirigido a la página principal del sistema y puede acceder a las funcionalidades del sistema.
- **Resultado Obtenido**: [Completar]
- **Problemas Encontrados**: [Completar]
- **Sugerencias**: [Completar]

### Prueba de inicio de sesión con credenciales inválidas (RF-02, RF-03)
- **Objetivo**: Verificar que el sistema no permite el inicio de sesión con credenciales inválidas.
- **Precondiciones**: El usuario debe tener una cuenta registrada en el sistema.
- **Datos de Prueba**:
  - Usuario: usuario_invalido
  - Contraseña: contraseña_invalida
- **Pasos**:
  1. Navegar a la página de inicio de sesión.
  2. Ingresar el nombre de usuario y la contraseña inválidos.
  3. Hacer clic en el botón "Iniciar sesión".
- **Resultado Esperado**: El sistema muestra un mensaje de error indicando que las credenciales son incorrectas.
- **Resultado Obtenido**: [Completar]
- **Problemas Encontrados**: [Completar]
- **Sugerencias**: [Completar]

### Prueba de recuperación de contraseña (si aplica)
- **Objetivo**: Verificar que el sistema permite la recuperación de la contraseña.
- **Precondiciones**: El usuario debe tener una cuenta registrada en el sistema.
- **Datos de Prueba**:
  - Email: email_registrado
- **Pasos**:
  1. Navegar a la página de inicio de sesión.
  2. Hacer clic en el enlace "Olvidé mi contraseña".
  3. Ingresar el email registrado.
  4. Hacer clic en el botón "Recuperar contraseña".
- **Resultado Esperado**: El sistema envía un email con instrucciones para recuperar la contraseña.
- **Resultado Obtenido**: [Completar]
- **Problemas Encontrados**: [Completar]
- **Sugerencias**: [Completar]

## Gestión de Usuarios

### Prueba de visualización del perfil de usuario (RF-06)
- **Objetivo**: Verificar que el sistema permite la visualización del perfil de usuario.
- **Precondiciones**: El usuario debe estar autenticado en el sistema.
- **Pasos**:
  1. Navegar a la página principal del sistema.
  2. Hacer clic en el enlace "Perfil".
- **Resultado Esperado**: El sistema muestra los datos del perfil del usuario.
- **Resultado Obtenido**: [Completar]
- **Problemas Encontrados**: [Completar]
- **Sugerencias**: [Completar]

### Prueba de asignación de roles a un usuario (RF-19)
- **Objetivo**: Verificar que el sistema permite asignar roles a los usuarios.
- **Precondiciones**: El usuario debe tener permisos de administrador.
- **Datos de Prueba**:
  - Usuario: usuario_a_asignar
  - Rol: rol_a_asignar
- **Pasos**:
  1. Navegar a la página de administración de usuarios.
  2. Seleccionar el usuario al que se le asignará un rol.
  3. Asignar el rol correspondiente.
  4. Guardar los cambios.
- **Resultado Esperado**: El sistema asigna correctamente el rol al usuario seleccionado.
- **Resultado Obtenido**: [Completar]
- **Problemas Encontrados**: [Completar]
- **Sugerencias**: [Completar]

## Publicación de Contenidos

### Prueba de creación de contenido de texto (RF-24, RF-28)
- **Objetivo**: Verificar que el sistema permite crear contenido de texto dentro de una categoría.
- **Precondiciones**: El usuario debe tener permisos para crear contenido.
- **Datos de Prueba**:
  - Título: Título de Prueba
  - Texto: Contenido de prueba
  - Categoría: Categoría de Prueba
- **Pasos**:
  1. Navegar a la página de creación de contenido.
  2. Ingresar los datos del contenido.
  3. Seleccionar la categoría correspondiente.
  4. Hacer clic en el botón "Guardar".
- **Resultado Esperado**: El sistema guarda y muestra el nuevo contenido en la categoría seleccionada.
- **Resultado Obtenido**: [Completar]
- **Problemas Encontrados**: [Completar]
- **Sugerencias**: [Completar]

### Prueba de visualización de publicaciones en "Mi perfil" (RF-27)
- **Objetivo**: Verificar que el sistema permite visualizar las publicaciones del autor dentro de la pestaña “Mi perfil”.
- **Precondiciones**: El usuario debe haber creado publicaciones previamente.
- **Pasos**:
  1. Navegar a la página principal del sistema.
  2. Hacer clic en el enlace "Mi perfil".
- **Resultado Esperado**: El sistema muestra todas las publicaciones creadas por el usuario.
- **Resultado Obtenido**: [Completar]
- **Problemas Encontrados**: [Completar]
- **Sugerencias**: [Completar]

## Interacción con Publicaciones

### Prueba de dar like a una publicación (RF-33)
- **Objetivo**: Verificar que el sistema permite dar like a una publicación.
- **Precondiciones**: El usuario debe estar autenticado en el sistema.
- **Pasos**:
  1. Navegar a una publicación.
  2. Hacer clic en el botón "Like".
- **Resultado Esperado**: El contador de likes de la publicación aumenta en uno.
- **Resultado Obtenido**: [Completar]
- **Problemas Encontrados**: [Completar]
- **Sugerencias**: [Completar]

### Prueba de comentar una publicación (RF-31)
- **Objetivo**: Verificar que el sistema permite a los usuarios comentar publicaciones.
- **Precondiciones**: El usuario debe estar autenticado en el sistema.
- **Datos de Prueba**:
  - Comentario: Comentario de prueba
- **Pasos**:
  1. Navegar a una publicación.
  2. Ingresar un comentario en el campo correspondiente.
  3. Hacer clic en el botón "Comentar".
- **Resultado Esperado**: El sistema guarda y muestra el comentario en la publicación.
- **Resultado Obtenido**: [Completar]
- **Problemas Encontrados**: [Completar]
- **Sugerencias**: [Completar]

### Prueba de compartir una publicación (RF-34)
- **Objetivo**: Verificar que el sistema permite compartir publicaciones.
- **Precondiciones**: El usuario debe estar autenticado en el sistema.
- **Pasos**:
  1. Navegar a una publicación.
  2. Hacer clic en el botón "Compartir".
- **Resultado Esperado**: El sistema muestra un código QR o un enlace para compartir la publicación.
- **Resultado Obtenido**: [Completar]
- **Problemas Encontrados**: [Completar]
- **Sugerencias**: [Completar]

## Gestión de Categorías

### Prueba de creación de una nueva categoría (RF-25, RF-36)
- **Objetivo**: Verificar que el sistema permite crear nuevas categorías.
- **Precondiciones**: El usuario debe tener permisos de administrador.
- **Datos de Prueba**:
  - Nombre: Categoría de Prueba
  - Descripción: Descripción de prueba
- **Pasos**:
  1. Navegar a la página de administración de categorías.
  2. Ingresar los datos de la nueva categoría.
  3. Hacer clic en el botón "Guardar".
- **Resultado Esperado**: El sistema guarda y muestra la nueva categoría en la lista de categorías.
- **Resultado Obtenido**: [Completar]
- **Problemas Encontrados**: [Completar]
- **Sugerencias**: [Completar]

## Flujo de Aprobación

### Prueba de cambio de estado de publicación a "Publicado" (RF-41)
- **Objetivo**: Verificar que el sistema permite cambiar el estado de una publicación a "Publicado".
- **Precondiciones**: El usuario debe tener permisos para cambiar el estado de las publicaciones.
- **Pasos**:
  1. Navegar a una publicación en estado "En revisión".
  2. Cambiar el estado de la publicación a "Publicado".
  3. Guardar los cambios.
- **Resultado Esperado**: El sistema actualiza el estado de la publicación a "Publicado".
- **Resultado Obtenido**: [Completar]
- **Problemas Encontrados**: [Completar]
- **Sugerencias**: [Completar]

### Prueba de cambio de estado de publicación a "Rechazado" (RF-42)
- **Objetivo**: Verificar que el sistema permite cambiar el estado de una publicación a "Rechazado".
- **Precondiciones**: El usuario debe tener permisos para cambiar el estado de las publicaciones.
- **Pasos**:
  1. Navegar a una publicación en estado "En revisión".
  2. Cambiar el estado de la publicación a "Rechazado".
  3. Guardar los cambios.
- **Resultado Esperado**: El sistema actualiza el estado de la publicación a "Rechazado".
- **Resultado Obtenido**: [Completar]
- **Problemas Encontrados**: [Completar]
- **Sugerencias**: [Completar]
