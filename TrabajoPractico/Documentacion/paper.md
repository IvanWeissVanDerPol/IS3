# UNIVERSIDAD NACIONAL DE ASUNCIÓN
## FACULTAD POLITÉCNICA – SEDE SAN LORENZO
### DISCIPLINA: INGENIERÍA DE SOFTWARE III
**PROFESOR**: Luis Gilberto Salinas 
**TEMA**: INFORME FINAL  
**GRUPO**: NÚMERO 7  
**INTEGRANTES**:  
- Ivan Weiss Van Der Pol
- Camila Maidana  
- jovana alvarez  
- Fran sanabria   

**TRABAJO PRÁCTICO**  
SAN LORENZO, 2024  

---

# Introducción
## Descripción del trabajo
En este trabajo, nos enfocamos en realizar pruebas exhaustivas sobre un Sistema de Gestión de Contenidos (CMS). Este sistema está diseñado para gestionar publicaciones, usuarios y categorías, ofreciendo una plataforma robusta y eficiente para la creación y administración de contenido digital.

## En qué consiste la actividad y en qué radica la importancia
La actividad consiste en validar los requerimientos del CMS y buscar fallas en sus funcionalidades. Las pruebas de software tienen como objetivo principal encontrar y corregir errores antes de que el sistema sea entregado al usuario final. Esta validación es crucial para asegurar que el sistema funcione según lo esperado y cumpla con los estándares de calidad necesarios.

## Objetivos
- Realizar pruebas sobre el sistema CMS para validar sus requerimientos.
- Identificar y documentar fallas en las funcionalidades del sistema.
- Asegurar que el sistema cumple con los requerimientos funcionales y no funcionales definidos.
- Evaluar la calidad de la interfaz gráfica y la experiencia del usuario.
- Ejecutar pruebas de estrés para determinar el rendimiento del sistema bajo condiciones de carga elevada.

## Importancia de las pruebas en el desarrollo de software
Las pruebas de software son fundamentales en el ciclo de vida del desarrollo de software. Probar el sistema permite detectar errores y problemas que podrían afectar negativamente la experiencia del usuario final. A través de pruebas rigurosas, se mejora la calidad, seguridad y rendimiento del sistema, asegurando que el producto final sea confiable y eficiente.

---

# Metodología utilizada y Planificación de Actividades
**Contacto Inicial**: Reunión inicial con los desarrolladores del sistema, obtención del código fuente, la documentación, y los requerimientos.

**Preparación del entorno**: Se realiza un vistazo inicial al código, se reúnen los recursos necesarios para ejecutar el sistema adecuadamente, y se ejecuta con datos ya cargados, creando un entorno listo para ser probado.

**Planificación de pruebas**: Elaboración de casos de prueba, elección de herramientas a utilizar y distribución del trabajo entre los miembros del equipo.

**Pruebas**: Se llevan a cabo las pruebas planificadas.

**Evaluación del sistema**: Se verifican los resultados de las pruebas y se compara el funcionamiento del sistema con los requerimientos para determinar si el comportamiento es el deseado.

**Informe**: Preparación del paper con todos los detalles de los procesos seguidos para la formulación y ejecución de las pruebas, así también se realizan las diapositivas para la presentación, y un video explicativo.

---

# Metodología de Pruebas
## Pruebas de Caja Blanca
### Inspección de código [Python]
Se emplearon herramientas específicas para este propósito. **Understand for Java** y **GeroneSoft's Code Counter Pro Software** se utilizaron para evaluar la complejidad ciclomática y métricas relacionadas con las líneas de código. También se utilizó **Radon** para análisis detallado.

## Resultados de la Inspección de Código
| Archivo                            | Nombre                      | Tipo    | Complejidad Ciclomática |
| ---------------------------------- | --------------------------- | ------- | ----------------------- |
| proyecto_is2\cms\gcloud.py         | GoogleCloudMediaFileStorage | Clase   | A (2)                   |
| proyecto_is2\cms\views.py          | principal                   | Función | B (10)                  |
| proyecto_is2\cms\views.py          | obtener_publicaciones       | Función | B (10)                  |
| proyecto_is2\comentarios\apps.py   | ComentariosConfig           | Clase   | A (1)                   |
| proyecto_is2\comentarios\forms.py  | CommentForm                 | Clase   | A (2)                   |
| proyecto_is2\comentarios\models.py | Comment                     | Clase   | A (2)                   |
| proyecto_is2\comentarios\views.py  | comentar                    | Función | A (3)                   |


### Inspección del modelo de datos
Se realizó de forma manual, sin utilizar herramientas de software. Se evaluaron las restricciones de integridad, triggers y redundancias para asegurar la consistencia de los datos.

# Pruebas ad hoc
### Evaluación de Casos de Prueba
Consistió en la prueba de las funcionalidades descritas en la documentación, tanto happy path como casos más complejos, inválidos y vacíos. Se registró la respuesta del sistema en cada caso y se sugieren algunas mejoras y/o correcciones.

#### Ejemplos de Casos de Prueba
1. **Prueba de inicio de sesión con credenciales válidas (RF-02, RF-03)**
   - **Objetivo**: Verificar que el sistema permite el inicio de sesión con credenciales válidas.
   - **Precondiciones**: El usuario debe tener una cuenta registrada en el sistema.
   - **Datos de Prueba**: Usuario: usuario0, Contraseña: contraseña_valida
   - **Pasos**:
     1. Navegar a la página de inicio de sesión.
     2. Ingresar el nombre de usuario y la contraseña válidos.
     3. Hacer clic en el botón "Iniciar sesión".
   - **Resultado Esperado**: El usuario es redirigido a la página principal del sistema y puede acceder a las funcionalidades del sistema.
   - **Resultado Obtenido**: El usuario es redirigido a la página principal del sistema y puede acceder a las funcionalidades del sistema.


### Evaluación de Requerimientos
Se evaluó cada requerimiento funcional, determinando su cumplimiento. Se encontró que la mayoría de los requerimientos están implementados correctamente, aunque algunos mensajes de error necesitan ser más descriptivos  .


# Evaluación de la Interfaz Gráfica
Se consideraron aspectos como la confortabilidad de la vista, la correctitud de los formularios y la facilidad de uso. La interfaz gráfica es amigable y relativamente simple de usar, aunque algunas opciones son difíciles de encontrar y la navegación puede ser confusa para los usuarios .


## Pruebas de Rendimiento
Se realizaron pruebas de rendimiento al sistema con la herramienta **JMeter**. Se probaron múltiples cargas para evaluar el comportamiento del sistema bajo condiciones de estrés.

### Resultados de las Pruebas de Estrés
| Número de peticiones | Promedio ms | Min ms | Max ms | Std. Dev. ms | Error % | Rendimiento sec | KB/seg recibido | KB/seg enviado | Bytes promedio |
| -------------------- | ----------- | ------ | ------ | ------------ | ------- | --------------- | --------------- | -------------- | -------------- |
| 500                  | 4762        | 59     | 9207   | 2633.99      | 0 %     | 26.1/sec        | 930.57          | 2.95           | 36563          |
| 1000                 | 9323        | 50     | 18188  | 5249.33      | 0 %     | 26.2/sec        | 935.30          | 2.97           | 36563          |
| 2000                 | 18428       | 49     | 35906  | 10348.07     | 0 %     | 26.4/sec        | 941.01          | 2.99           | 36563          |
| 3000                 | 27689       | 52     | 53926  | 15571.32     | 0 %     | 26.3/sec        | 940.42          | 2.98           | 36563          |
| 4000                 | 36918       | 52     | 60017  | 19838.80     | 22.30 % | 28.6/sec        | 794.84          | 3.24           | 28428.8        |
| 5000                 | 45617       | 56     | 92522  | 22887.27     | 43.50 % | 28.1/sec        | 570.86          | 3.18           | 20901.2        |
| 6000                 | 50200       | 54     | 92520  | 21551.30     | 59.20 % | 31.2/sec        | 460.30          | 3.53           | 15112.5        |
  .


### Planificación de Actividades
Se anexó la distribución de trabajo, duración, fecha de inicio y fin de las actividades y recursos asignados. Las actividades están planificadas de manera que se puedan realizar en el tiempo establecido y con los recursos disponibles. 

---
# Comparación entre las características de facilidad de prueba con las características exhibidas por el sistema

- **Operabilidad**: 
  El sistema muestra un comportamiento generalmente esperado cuando se realizan acciones estándar. Sin embargo, se presentan errores al intentar realizar acciones fuera del rango esperado. Por ejemplo, la barra de búsqueda no encuentra usuarios o categorías, pero sí encuentra contenidos correctamente. Esto indica que la funcionalidad de búsqueda necesita mejorar para ser más robusta y completa.

- **Observabilidad**:
  El sistema ofrece mensajes informativos cuando se realizan la mayoría de las acciones. Sin embargo, hay ocasiones en las que los mensajes son insuficientes o contienen información incorrecta. Un ejemplo de esto es al ingresar credenciales incorrectas durante el inicio de sesión, donde el mensaje de error es poco descriptivo y no especifica el problema exacto.

- **Controlabilidad**:


- **Capacidad de Descomposición**:
  El sistema está bien descompuesto en módulos claros y manejables, como Seguridad, Proyecto y Desarrollo. Cada módulo tiene su propia responsabilidad, lo que facilita la prueba y el mantenimiento del sistema. La estructura modular está bien definida con archivos dedicados a configuraciones, usuarios, publicaciones, y scripts específicos para cada funcionalidad, como activación de publicaciones, búsqueda, calificaciones, y visualización de códigos QR.

- **Simplicidad**:
  La interfaz gráfica del sistema es amigable y relativamente simple de usar. Se utiliza un diseño limpio con colores adecuados y tipos de fuentes que facilitan la lectura. No obstante, algunas opciones son difíciles de encontrar, y la navegación puede resultar confusa para los usuarios. La falta de un apartado de ayuda disponible también limita la simplicidad de uso, especialmente para nuevos usuarios que podrían necesitar orientación.


---

# Inspección de Código
En la inspección del código se analizaron los archivos fuentes [Lenguaje de Programación].

## Complejidad Ciclomática del Código [Lenguaje de Programación]
La complejidad ciclomática es una métrica que ayuda a evaluar la complejidad de un programa de software al contar los caminos de ejecución independientes en el código. Su objetivo es identificar áreas de código complejas que puedan requerir mejoras en términos de mantenibilidad y entendimiento.

### Listado de complejidad mayor o igual a 10:
| Nombre                          | Tipo             | Complejidad Ciclomática |
| ------------------------------- | ---------------- | ----------------------- |
| principal | Función | 10                |
| obtener_publicaciones | Función | 10                 |
| actualizar | Función | 10                 |

### Listado por rangos:
| Rango      | Cantidad   |
| ---------- | ---------- |
| A (1-5)    | 117 |
| B (6-10)   | 10 |
| C (11-20)  | 0 |
| D (21-50)  | 0 |
| E (51-100) | 0 |
| F (>100)   | 1 |

## Métricas de líneas de código y comentarios
| Tipo                      | Cantidad   |
| ------------------------- | ---------- |
| Total de Líneas           | 3713 |
| Total de Líneas de código | 2268 |
| Total de Líneas en blanco | 681 |
| Total de Comentarios      | 184 |

El código muestra una proporción significativa de comentarios, representando un porcentaje elevado del [Porcentaje]% del total de líneas.

## Mensajes de errores y advertencias
| Tipo                   | Cantidad   |
| ---------------------- | ---------- |
| Errores                | 70 |
| Convenciones de código | 466 |
| Advertencias           | 40 |
| Refactorizaciones      | 46 |

El código obtuvo una calificación de [Calificación] según [Herramienta].

---

# Análisis del Modelo de Datos

## Checklist del Modelo de la Base de Datos

### Restricciones de Integridad

| Tipo                                                                                                                                              | Observaciones |
| ------------------------------------------------------------------------------------------------------------------------------------------------- | ------------- |
| **De Entidad**                                                                                                                                    |               |
| Toda fila debe tener una clave principal                                                                                                          | Cumplido      |
| Los valores de la clave deben ser únicos                                                                                                          | Cumplido      |
| Los valores no deben ser nulos                                                                                                                    | Cumplido      |
| Los valores no pueden estar duplicados                                                                                                            | Cumplido      |
| **De Dominio**                                                                                                                                    |               |
| Comprobación de validez                                                                                                                           | Cumplido      |
| Restricción del tipo de dato                                                                                                                      | Cumplido      |
| Comprobación del formato                                                                                                                          | Cumplido      |
| Comprobación de los valores posibles en una columna                                                                                               | Cumplido      |
| **De Referencia**                                                                                                                                 |               |
| Evita la eliminación de filas de una tabla a la que se hace referencia                                                                            | Cumplido      |
| Evita la modificación de la clave principal si una clave externa hace referencia a la fila                                                        | Cumplido      |
| Actualización sobre la tabla hija del valor de la clave externa, y verificar correspondencia con el valor de la clave principal en la tabla padre | Cumplido      |


 **De Entidad**:
   - Todas las tablas tienen una clave primaria definida.
   - Las claves primarias garantizan que los valores sean únicos y no nulos.
   - No se permiten valores duplicados en las claves primarias.
 **De Dominio**:
   - Los tipos de datos están definidos para cada columna, lo que garantiza la validez, formato y restricción de tipo de datos.

 **De Referencia**:
   - Las claves foráneas están definidas con restricciones para evitar la eliminación y modificación de filas referenciadas.
   - Las actualizaciones sobre las tablas hijas mantienen la correspondencia con las claves principales en las tablas padres.


### Triggers

| Items                                                                   | Observaciones |
| ----------------------------------------------------------------------- | ------------- |
| Triggers de inserción definidos                                         | No Definidos  |
| Triggers de modificación definidos                                      | No Definidos  |
| Triggers de eliminación definidos                                       | No Definidos  |
| Triggers de violación de restricción de integridad definidos            | No Definidos  |
| Triggers de intervalo de tiempo definidos                               | No Definidos  |
| Son suficientes para controlar las operaciones ABM                      | No Definidos  |
| Se utiliza para evitar inconsistencia en caso de redundancia controlada | No Definidos  |

 **Triggers**:
   - No se han definido triggers en las tablas, lo cual puede ser una oportunidad para mejorar el control de operaciones ABM y evitar inconsistencias.

### Redundancias

| Items                                                      | Observaciones |
| ---------------------------------------------------------- | ------------- |
| Redundancias creadas                                       | Cumplido      |
| Constraints definidos para evitar inconsistencias al crear | Cumplido      |
| Medidas paraevitar inconsistencias en actualizaciones      | Cumplido      |
 
 **Redundancias**:
   - Se han definido constraints para evitar inconsistencias en la creación y actualización de datos, y se han identificado redundancias controladas en algunas tablas.



### Código SQL

| Items                              | Observaciones |
| ---------------------------------- | ------------- |
| Consultas SQL definidas            | No Definido   |
| Codificación estándar de consultas | No Definido   |
| Reutilización del código SQL       | No Definido   |

 **Código SQL**:
   - No se definieron consultas SQL estándar ni reutilización de código SQL en el modelo de datos proporcionado. Esto puede ser una mejora futura para estandarizar y reutilizar consultas.

### Normalización

| Items                   | Observaciones |
| ----------------------- | ------------- |
| Primera Forma Normal    | Cumplido      |
| Segunda Forma Normal    | Cumplido      |
| Tercera Forma Normal    | Cumplido      |
| Forma Normal Boyce-Cood | Cumplido      |
| Cuarta Forma Normal     | No Aplicable  |

 **Normalización**:
   - Las tablas cumplen con las primeras tres formas normales (1NF, 2NF y 3NF) y la forma normal de Boyce-Codd (BCNF), asegurando la eliminación de redundancias y dependencias anómalas.
   - La cuarta forma normal (4NF) no es aplicable en este contexto debido a la ausencia de multivalores.

Este análisis muestra que el modelo de datos está bien estructurado en términos de integridad y normalización, pero carece de triggers y consultas SQL estándar que podrían mejorar el control y la eficiencia del sistema.

---

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

### Casos de Prueba Propuestos

#### Inicio de Sesión y Autenticación
- **Prueba de inicio de sesión con credenciales válidas** (RF-02, RF-03)
- **Prueba de inicio de sesión con credenciales inválidas** (RF-02, RF-03)
- **Prueba de recuperación de contraseña** (si aplica)

#### Gestión de Usuarios
- **Prueba de visualización del perfil de usuario** (RF-06)
- **Prueba de asignación de roles a un usuario** (RF-19)

#### Publicación de Contenidos
- **Prueba de creación de contenido de texto** (RF-24, RF-28)
- **Prueba de visualización de publicaciones en "Mi perfil"** (RF-27)

#### Interacción con Publicaciones
- **Prueba de dar like a una publicación** (RF-33)
- **Prueba de comentar una publicación** (RF-31)
- **Prueba de compartir una publicación** (RF-34)

#### Gestión de Categorías
- **Prueba de creación de una nueva categoría** (RF-25, RF-36)

#### Flujo de Aprobación
- **Prueba de cambio de estado de publicación a "Publicado"** (RF-41)
- **Prueba de cambio de estado de publicación a "Rechazado"** (RF-42)

Al enfocarse en estas áreas, se puede asegurar que las funciones críticas del sistema sean probadas a fondo para identificar cualquier defecto o área de mejora.

---

# Pruebas de Stress
Las pruebas se realizaron utilizando el software **[Herramienta de Pruebas de Stress]**, se testeó mediante peticiones en paralelo a la página inicial de login del sistema. Se pudo observar un buen rendimiento del servidor, respondiendo hasta [Cantidad de Peticiones] peticiones sin errores.

La tabla de resultados por cada cantidad de peticiones puede ser encontrada en el archivo adjunto.

---

# Cumplimiento de Requerimientos Funcionales y No Funcionales

El documento ERS contiene un total de 65 Requerimientos Funcionales, los cuales se organizan en los siguientes módulos:

- **Módulo de Seguridad**
  - Autenticación
  - Autorización
    - Definición de Permisos
    - Ver Permisos
    - Definición de Roles
    - Ver Roles
    - Crear Roles
    - Modificar Roles
    - Eliminar Roles
    - Asignar Roles
    - Restricciones
  - Usuarios
    - Definición de Usuarios
    - Restricciones
- **Módulo de Proyecto**
  - Ver Proyectos
  - Crear Proyectos
  - Modificar Proyectos
  - Eliminar Proyectos
  - Cancelar Proyectos
  - Restricciones
  - Autorización
  - Ver Permisos de Proyecto
  - Crear Roles de Proyecto
  - Modificar Roles de Proyecto
  - Eliminar Roles de Proyecto
  - Miembros del Proyecto
  - Restricciones
  - Estados
    - Flujo de Estados
    - Restricciones
- **Módulo de Desarrollo**
  - User Stories
    - Ver User Stories
    - Crear User Stories
    - Modificación User Stories
    - Cancelar User Stories
    - Estados de User Stories
  - Sprints
    - Ver Sprints
    - Crear Sprints
    - Modificar Sprints
    - Cancelar Sprints
    - Estados
    - Restricciones
    - Actividades
      - Ver Actividades
      - Crear Actividades
      - Modificar Actividades
      - Eliminar Actividades
  - Kanban
  - Burndown Chart

Podemos observar las estadísticas del cumplimiento de los Requerimientos Funcionales en la siguiente tabla:

| Cantidad | Cumplen | No Cumplen | % Cumplen | % No Cumplen |
| -------- | ------- | ---------- | --------- | ------------ |
| 65       | 60      | 5          | 92.3%     | 7.7%         |
---
# Evaluación de la Interfaz Gráfica

En términos generales, la interfaz posee un diseño simple pero amigable, sin una utilización excesiva de colores ni opciones muy ocultas en menús de difícil acceso. A continuación se presenta una tabla con los criterios que fueron tomados en cuenta para la evaluación y las observaciones realizadas:

## Confortabilidad de la vista

| Criterio           | Observaciones |
| ------------------ | ------------- |
| Colores            | Los colores utilizados son suaves y no fatigan la vista. La paleta de colores es coherente y se mantiene uniforme en todas las pantallas. |
| Tipos de fuente    | Se utilizaron tipos de fuente estándar y legibles. Sin embargo, podría mejorarse la diferenciación entre títulos y contenido para una mejor jerarquía visual. |
| Tamaños de fuentes | Los tamaños de las fuentes son adecuados y permiten una fácil lectura. No obstante, algunos elementos secundarios tienen fuentes un poco pequeñas que podrían dificultar la lectura en pantallas más pequeñas. |
| Imágenes           | Las imágenes son de buena calidad y se utilizan adecuadamente para complementar el contenido sin sobrecargar visualmente las páginas. |

## Formularios

| Items                           | Observaciones |
| ------------------------------- | ------------- |
| Cantidad de campos              | La cantidad de campos en los formularios es adecuada y no resulta abrumadora para el usuario. |
| Facilidad de carga              | Los formularios se cargan rápidamente y sin errores, lo que mejora la experiencia del usuario. |
| Indicación de campos requeridos | Los campos requeridos están claramente marcados, lo cual es útil para evitar errores al completar los formularios. |
| Validaciones                    | Las validaciones funcionan correctamente, aunque en algunos casos los mensajes de error podrían ser más descriptivos para ayudar al usuario a corregir sus errores. |

## Facilidad de uso

| Items                        | Observaciones |
| ---------------------------- | ------------- |
| Navegabilidad                | La navegación es intuitiva y las secciones están bien organizadas. Sin embargo, algunas opciones son difíciles de encontrar y podrían beneficiarse de una mejor estructuración de los menús. |
| Disposición de los controles | Los controles están bien dispuestos y son accesibles, lo que facilita su uso. |
| Disponibilidad de ayuda      | No hay una sección de ayuda visible, lo cual podría ser una desventaja para los nuevos usuarios que necesiten orientación. |
| Búsquedas                    | La función de búsqueda funciona bien para contenidos, pero no es efectiva para buscar usuarios o categorías. Esto limita la capacidad de encontrar ciertos tipos de información rápidamente. |


---
# Conclusiones

Los resultados obtenidos son, en general, aceptables. Sin embargo, el sistema exhibe comportamientos inadecuados en diversas situaciones de ejecución sencilla. Además, no se ha logrado cumplir con una cantidad considerable de los requerimientos establecidos.

Aunque la interfaz gráfica resulta amigable para el usuario, puede resultar confuso navegar por algunas secciones del proyecto. Por consiguiente, la calidad del software se sitúa en un nivel intermedio y es necesario realizar ajustes para poder utilizar esta aplicación en un entorno formal.

La realización de pruebas exhaustivas fue fundamental para evaluar la calidad del software y detectar los errores presentes. Estos fallos no son fácilmente identificables a simple vista, por lo que sería un error entregar una versión aparentemente final a un cliente sin llevar a cabo dichas evaluaciones.

La realización de pruebas de software puede implicar un trabajo arduo y extenso. Por tanto, resulta importante llevar a cabo una planificación adecuada y una distribución eficiente de las tareas involucradas.

El trabajo de un evaluador de software es de naturaleza compleja, pero sus esfuerzos dan frutos. No hay duda de que llevar a cabo este análisis fue una decisión acertada, y se recomienda realizarlo en proyectos futuros para asegurar siempre altos estándares de calidad.

## Recomendaciones

1. **Mejorar la Funcionalidad de Búsqueda**: Asegurar que la barra de búsqueda pueda encontrar usuarios y categorías, no solo contenidos.
2. **Mensajes de Error Descriptivos**: Aumentar la claridad de los mensajes de error para que los usuarios puedan entender y corregir fácilmente los problemas.
3. **Mejorar la Navegabilidad**: Reorganizar los menús y opciones para que sean más intuitivos y fáciles de encontrar.
4. **Implementar una Sección de Ayuda**: Incluir una sección de ayuda o tutoriales para asistir a los nuevos usuarios en el uso del sistema.
5. **Validaciones de Formularios**: Hacer que los mensajes de validación de formularios sean más específicos y útiles.
6. **Pruebas Continuas**: Realizar pruebas continuas y exhaustivas durante el desarrollo para asegurar la calidad y detectar errores de manera temprana.

## Agradecimientos

Agradecemos a los profesores y compañeros que colaboraron en la realización de este proyecto. Su apoyo y guía fueron esenciales para completar este análisis exhaustivo del sistema CMS.

---
