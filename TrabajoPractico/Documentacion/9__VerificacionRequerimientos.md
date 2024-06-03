# Verificación del Cumplimiento de los Requerimientos Funcionales y No Funcionales

## 1. Resumen Ejecutivo
Este documento tiene como objetivo verificar el cumplimiento de los requerimientos funcionales y no funcionales del sistema. La verificación se realiza para asegurar que el sistema cumple con las especificaciones definidas y funciona según lo esperado. Los resultados clave de esta verificación se resumen a continuación:
- [Resumen breve de los resultados clave]

## 2. Introducción
### 2.1 Propósito
Describir el objetivo del documento y la importancia de verificar el cumplimiento de los requerimientos del sistema.

### 2.2 Definiciones, Acrónimos y Abreviaturas
-**RF-#**: Requerimiento Funcional.
-**RNF-#**: Requerimiento No Funcional.
-**Scrum**: Marco de gestión de proyectos ágil.
-**Kanban**: Herramienta de gestión visual de proyectos.
-**SSO**: Single Sign-On, procedimiento de autenticación único.

### 2.3 Alcance
Este documento presenta una descripción del propósito de un Sistema de Administración de Contenido Web y detalla tanto los requerimientos funcionales como no funcionales necesarios para su creación.

## 3. Metodología de Verificación
### 3.1 Herramientas Utilizadas
- [Herramienta 1]: Descripción de cómo se utilizó.
- [Herramienta 2]: Descripción de cómo se utilizó.

### 3.2 Proceso de Verificación
Describir el proceso seguido para la verificación, incluyendo los pasos y criterios de evaluación.

## 4. Detalles de la Evaluación
### Requerimientos Funcionales

| Código       | Descripción                                                                                       | Cumplimiento | Detalles de Prueba                                                                                       |
|--------------|---------------------------------------------------------------------------------------------------|--------------|-----------------------------------------------------------------------------------------------------------|
|**Inicio de sesión** |  |  |  |
RF-01 | El sistema permitirá el acceso al sitio web sin la necesidad de iniciar sesión.|  |  |
RF-02 | El sistema permitirá el inicio de sesión mediante una aplicación dedicada a este propósito con la provisión de un username y password.|  |  |
RF-03 | La aplicación de inicio de sesión del sistema verificará que las credenciales proporcionadas por el usuario son correctas y válidas.	|  |  |
RF-04 | El sistema deberá mostrar una barra de búsqueda para categorías, usuarios y contenidos.|  |  |
RF-05 | El sistema deberá mostrar publicaciones de tipo público de todas las categorías en caso de que el usuario no esté con una sesión iniciada.|  |  |
RF-06 | El sistema permitirá la visualización del perfil de usuario.|  |  |
RF-07 | El usuario podrá seleccionar una categoría para recibir publicaciones de esta en la pestaña de inicio.|  |  |
RF-09 | El sistema mostrará un listado completo de categorías en la opción de “Categorías” que se ubicará en la barra lateral cada uno con su nombre.|  |  |
RF-10 | Al pulsar en el nombre de la categoría, el sistema listará publicaciones de dicha categoría en la misma pantalla.|  |  |
|**Roles** |  |  |  |
RF-11 | El sistema contará con un rol que posea permisos orientados a la administración (administrador).|  |  |
RF-13 | El administrador podrá modificar los roles existentes.|  |  |
RF-14 | El administrador podrá  asignar roles a los usuarios.|  |  |
RF-15 | El administrador podrá acceder a la configuración del sistema.|  |  |
|**Permisos** |  |  |  |
RF-17 | El sistema permitirá modificar permisos no críticos de roles ya existentes.|  |  |
RF-18 | El sistema deberá permitir quitar un rol a los usuarios.|  |  |
RF-19 | El sistema permitirá asignar roles a los usuarios.|  |  |
RF-21 | El sistema deberá permitir al usuario poder acceder a cualquier publicación disponible en la categoría seleccionada.|  |  |
RF-22 | El sistema deberá permitir solo a los usuarios con permisos crear contenido.|  |  |
RF-23 | El sistema deberá permitir a los usuarios con permisos editar publicaciones.|  |  |
RF-24 | El sistema deberá permitir crear contenido dentro de una categoría.|  |  |
RF-25 | El sistema deberá permitir crear nuevas categorías.|  |  |
RF-26 | El sistema deberá permitir modificar categorías ya existentes.|  |  |
RF-27 | El sistema permitirá al autor visualizar sus publicaciones dentro de la pestaña “Mi perfil”.|  |  |
RF-28 | El sistema deberá permitir crear nuevos contenidos de texto.|  |  |
RF-29 | El sistema deberá permitir crear nuevos contenidos multimedias.|  |  |
RF-30 | El sistema deberá permitir crear nuevos contenidos comerciales.|  |  |
RF-31 | El sistema deberá permitir a los usuarios comentar publicaciones .|  |  |
RF-32 | El sistema deberá permitir la visualización de comentarios.|  |  |
RF-33 | El sistema permitirá la posibilidad de dar likes a una publicación.|  |  |
RF-34 | El sistema deberá permitir compartir publicaciones.|  |  |
|**Categoría** |  |  |  |
RF-35 | El sistema deberá generar un código identificador para cada publicación constando de la abreviatura de la categoría seguido de un número autogenerado que vaya incrementando según se creen más publicaciones.|  |  |
RF-36 | El administrador podrá crear categorías.|  |  |
RF-37 | El administrador podrá editar categorías.|  |  |
RF-38 | El administrador o todo aquel usuario que tenga permiso podrá eliminar publicaciones.|  |  |
|**Flujo de aprobación** |  |  |  |
RF-40 | El sistema permitirá al autor o todo aquel usuario que tenga permiso ver el estado de cada publicación desde un tablero kanban.|  |  |
RF-41 | El sistema permitirá el cambio de estado de una publicación de “En revisión” a “Publicado”.|  |  |
RF-42 | El sistema permitirá el cambio de estado de una publicación de “En revisión” a “Rechazado”.|  |  |
RF-43 | El sistema requerirá una justificación junto a cada publicación rechazada.|  |  |
RF-44 | El sistema permitirá el cambio de estado de una publicación de “Borrador” a “En revisión”.|  |  |
RF-45 | El publicador o todo aquel usuario que tenga permiso puede rechazar publicaciones.|  |  |
RF-46 | El sistema deberá mandar todo contenido rechazado al estado de borrador.|  |  |
RF-47 | El publicador o todo aquel usuario que tenga permiso puede aceptar publicaciones.|  |  |
RF-48 | El autor debe contar con permisos para poder publicar en categorías sin moderación.|  |  |
|**Likes/views** |  |  |  |
RF-49 | El sistema deberá contabilizar las visualizaciones.|  |  |
RF-50 | El sistema permitirá la posibilidad de quitar un like ya dado a una publicación.|  |  |
RF-51 | El sistema deberá permitir la visualización de las veces que una publicación se compartió.|  |  |
RF-52 | El sistema deberá contabilizar los likes de cada publicación.|  |  |
RF-53 | El sistema generará un enlace al compartir una publicación.|  |  |
RF-54 | El sistema contabilizará las veces compartidas.|  |  |
|**Vigencia de publicaciones** |  |  |  |
RF-55 | El sistema permitirá añadir una fecha de vigencia a la hora de crear una publicación.|  |  |
RF-56 | El sistema pasará al estado “Inactivo” toda publicación cuya fecha de vigencia haya caducado.|  |  |
|**Registro de Historial** |  |  |  |
RF-57 | El sistema notificará a los autores cuando una publicación pasa del estado “En revisión” a “Publicado”.|  |  |
RF-58 | El sistema notificará a los autores cuando una publicación pasa del estado “En revisión” a “Rechazado”.|  |  |
RF-59 | El sistema notificará a los autores cuando una publicación pasa del estado “Publicado” a “Borrador”.|  |  |
RF-60 | El sistema notificará a los autores cuando una publicación pasa del estado “Publicado” a “Inactivo”.|  |  |
|**Registro de Historial** |  |  |  |
RF-61 | El sistema deberá registrar todos los cambios de estado realizados en una publicación.|  |  |
RF-62 | El sistema deberá mostrar todos los cambios de estado realizados de una publicación.|  |  |
|**Reportes estadísticos** |  |  |  |
RF-63 | El sistema permitirá generar reportes estadísticos de las publicaciones con más likes.|  |  |
RF-64 | El sistema permitirá generar reportes estadísticos de las publicaciones con más visualizaciones.|  |  |
RF-65 | El sistema permitirá generar reportes estadísticos de las publicaciones más compartidas.|  |  |
|**Inicio de sesión** |  |  |  |
RF-66 | El sistema permitirá el inicio de sesión mediante una aplicación dedicada a este propósito con la provisión de un username y password.
RF-67 | La aplicación de inicio de sesión del sistema verificará que las credenciales proporcionadas por el usuario son correctas y válidas.|  |  |
RF-68 | El sistema deberá mostrar publicaciones de tipo público de todas las categorías en caso de que el usuario no esté con una sesión iniciada.|  |  |
RF-69 | El usuario podrá seleccionar una categoría para recibir publicaciones de esta en la pestaña de inicio.|  |  |
RF-70 | El sistema mostrará publicaciones destinadas a visitantes, a usuarios con sesión activa y a suscriptores con sesión activa.|  |  |
RF-71 | El sistema mostrará un listado completo de categorías en la opción de “Categorías” que se ubicará en la barra lateral cada uno con su nombre.|  |  |
RF-72 | Al pulsar en el nombre de la categoría, el sistema listará publicaciones de dicha categoría en la misma pantalla.|  |  |
|**Roles** |  |  |  |
RF-73 | El sistema contará con un rol que posea permisos orientados a la administración (administrador).|  |  |
RF-74 | El administrador podrá listar roles existentes en el sistema.|  |  |
RF-75 | El administrador podrá modificar los roles existentes.|  |  |
RF-76 | El administrador podrá  asignar roles a los usuarios.|  |  |
RF-77 | El administrador podrá acceder a la configuración del sistema.|  |  |
RF-78 | El sistema contará con roles predefinidos cada uno con permisos correspondientes a las funciones que deben cumplir en el sistema.|  |  |
RF-79 | El sistema deberá permitir listar permisos.|  |  |
|**Categoría** |  |  |  |
RF-80 | El sistema deberá permitir crear contenido dentro de una categoría.|  |  |
RF-81 | El administrador podrá crear categorías.|  |  |
RF-82 | El administrador podrá editar categorías.|  |  |
RF-83 | El sistema contará con un formulario único para la creación de contenido en cualquier categoría.|  |  |



##### Requerimientos No Funcionales

| Código       | Descripción                                                                                       | Cumplimiento | Detalles de Prueba                                                                                       |
|--------------|---------------------------------------------------------------------------------------------------|--------------|-----------------------------------------------------------------------------------------------------------|
RNF-1 | Se deberá contar con acceso a internet para poder utilizar el sistema.|  |  |
RNF-2 | El sistema deberá ser operado desde una computadora.|  |  |
RNF-3 | El sistema no permitirá crear permisos.|  |  |
RNF-4 | El sistema no permitirá eliminar permisos.|  |  |
RNF-5 | El sistema no mostrará las publicaciones cuyos estados están en “Inactivo”.|  |  |
RNF-6 | El sistema no permitirá crear plantillas. |  |  |
RNF-7 | El sistema no permitirá crear plantillas.|  |  |
RNF-8 | El sistema no permitirá crear roles.|  |  |
RNF-9 | El sistema no permitirá eliminar roles.|  |  |


## 5. Análisis de Impacto
Describir el impacto potencial de cualquier incumplimiento de los requerimientos en el sistema y en los usuarios. Incluir una evaluación de los riesgos asociados y posibles consecuencias.

## 6. Recomendaciones
### 6.1 Acciones Correctivas
Sugerir las siguientes acciones para abordar los requerimientos que no se cumplieron:
- [Requerimiento No Cumplido]: [Recomendación de acción correctiva]
- [Requerimiento No Cumplido]: [Recomendación de acción correctiva]

### 6.2 Mejoras Futuras
- [Recomendación para mejora futura 1]
- [Recomendación para mejora futura 2]

## 7. Conclusiones
Después de realizar la verificación de los requerimientos funcionales y no funcionales, se concluye que el sistema [cumple/no cumple] con las especificaciones definidas. [Descripción adicional de los hallazgos y posibles recomendaciones.]

## 8. Anexos
Incluir cualquier documentación adicional, como capturas de pantalla de pruebas, logs, o informes detallados de herramientas de análisis.
- [Anexo 1: Capturas de pantalla]
- [Anexo 2: Logs de prueba]
- [Anexo 3: Informes de análisis]
