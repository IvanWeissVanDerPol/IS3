# UNIVERSIDAD NACIONAL DE ASUNCIÓN
## FACULTAD POLITÉCNICA – SEDE SAN LORENZO
### DISCIPLINA: INGENIERÍA DE SOFTWARE III
**PROFESOR**:   
**TEMA**: INFORME FINAL  
**GRUPO**: NÚMERO xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx  
**INTEGRANTES**:  
- Ivan Weiss Van Der Pol
- [NOMBRE INTEGRANTE 2]  
- [NOMBRE INTEGRANTE 3]  
- [NOMBRE INTEGRANTE 4]  

**TRABAJO PRÁCTICO**  
SAN LORENZO, 2024  

---

# Introducción
Las pruebas de software permiten controlar la calidad y funcionalidad de cualquier producto que se desarrolle; son la mejor garantía de que este no presenta fallos y se comporta adecuadamente.

El trabajo consiste en verificar el correcto funcionamiento y la buena implementación de un proyecto de software, además de buscar puntos débiles y puntos de mejora.

Para ello es necesario inspeccionar y entender el código, analizar el modelo de datos, verificar que se cumplan con los requerimientos del sistema, evaluar la interfaz gráfica y, claramente, realizar pruebas.

El proyecto de software a examinar es el **[NOMBRE DEL PROYECTO]**, elaborado por [NOMBRE DESARROLLADOR 1], [NOMBRE DESARROLLADOR 2] y [NOMBRE DESARROLLADOR 3]. Este proyecto permite implementar la metodología ágil Scrum, junto con tableros Kanban, para el desarrollo de proyectos, donde se cuentan con equipos de desarrollos, con roles específicos.

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
### Inspección de código [Lenguaje de Programación]
Se emplearon herramientas específicas para este propósito. **[Herramienta 1]** fue utilizada para evaluar la complejidad ciclomática y métricas relacionadas con las líneas de código, mientras que **[Herramienta 2]** se encargó de verificar errores, convenciones de código, identificar advertencias y sugerir posibles mejoras en la estructura del código.

### Inspección del modelo de datos
Se realizó de forma manual, sin utilizar herramientas de software.

## Pruebas de Caja Negra
### Evaluación de Casos de Prueba
Consistió en pruebas de datos esperados, datos nulos y datos no esperados o fuera de rango. Se registró la respuesta del sistema en cada caso y se sugieren algunas mejoras y/o correcciones.

### Evaluación de Requerimientos
Se evaluó cada requerimiento funcional, determinando su cumplimiento. No se encontraron requerimientos no funcionales.

### Evaluación de la Interfaz Gráfica
Se consideraron aspectos como la confortabilidad de la vista, la correctitud de los formularios, y la facilidad de uso.

### Pruebas de Rendimiento
Se realizaron pruebas de rendimiento al sistema con la herramienta **[Herramienta de Pruebas de Rendimiento]**.

### Planificación de Actividades
Se anexo la distribución de trabajo, duración, fecha de inicio y fin de las actividades y recursos asignados; además del gráfico de Gantt para las actividades planificadas.

---

# Comparación entre las características de facilidad de prueba con las características exhibidas por el sistema
- **Operabilidad**: El sistema presenta errores al intentar realizar acciones fuera de lo esperado, a pesar de esto, en líneas generales el sistema opera de una manera esperada.
- **Observabilidad**: El sistema presenta mensajes informativos a la hora de realizar la mayoría de las acciones, en ciertos casos faltan mensajes o contienen información incorrecta.
- **Controlabilidad**: Los controles de validez de los datos son realizados antes de aplicar permanentemente los cambios.
- **Capacidad de Descomposición**: El sistema se encuentra subdividido en tres módulos: Seguridad, Proyecto y Desarrollo.
- **Simplicidad**: El sistema presenta una interfaz gráfica amigable, aunque algunas opciones son difíciles de encontrar.

---

# Inspección de Código
En la inspección del código se analizaron los archivos fuentes [Lenguaje de Programación].

## Complejidad Ciclomática del Código [Lenguaje de Programación]
La complejidad ciclomática es una métrica que ayuda a evaluar la complejidad de un programa de software al contar los caminos de ejecución independientes en el código. Su objetivo es identificar áreas de código complejas que puedan requerir mejoras en términos de mantenibilidad y entendimiento.

### Listado de complejidad mayor o igual a 10:
| Nombre | Tipo | Complejidad Ciclomática |
|--------|------|-------------------------|
| [Nombre de la Función/Método 1] | [Función/Método] | [Valor] |
| [Nombre de la Función/Método 2] | [Función/Método] | [Valor] |
| [Nombre de la Función/Método 3] | [Función/Método] | [Valor] |

### Listado por rangos:
| Rango | Cantidad |
|-------|----------|
| A (1-5) | [Cantidad] |
| B (6-10) | [Cantidad] |
| C (11-20) | [Cantidad] |
| D (21-50) | [Cantidad] |
| E (51-100) | [Cantidad] |
| F (>100) | [Cantidad] |

## Métricas de líneas de código y comentarios
| Tipo | Cantidad |
|------|----------|
| Archivos analizados | [Cantidad] |
| Total de Líneas | [Cantidad] |
| Total de Líneas de código | [Cantidad] |
| Total de Líneas en blanco | [Cantidad] |
| Total de Comentarios | [Cantidad] |

El código muestra una proporción significativa de comentarios, representando un porcentaje elevado del [Porcentaje]% del total de líneas.

## Mensajes de errores y advertencias
| Tipo | Cantidad |
|------|----------|
| Errores | [Cantidad] |
| Convenciones de código | [Cantidad] |
| Advertencias | [Cantidad] |
| Refactorizaciones | [Cantidad] |

El código obtuvo una calificación de [Calificación] según [Herramienta].

---

# Análisis del Modelo de Datos
## Checklist del Modelo de la Base de Datos
### Restricciones de Integridad
| Tipo | Observaciones |
|------|---------------|
| De Entidad | |
| Toda fila debe tener una clave principal | [Estado] |
| Los valores de la clave deben ser únicos | [Estado] |
| Los valores no deben ser nulos | [Estado] |
| Los valores no pueden estar duplicados | [Estado] |
| De Dominio | |
| Comprobación de validez | [Estado] |
| Restricción del tipo de dato | [Estado] |
| Comprobación del formato | [Estado] |
| Comprobación de los valores posibles en una columna | [Estado] |
| De Referencia | |
| Evita la eliminación de filas de una tabla a la que se hace referencia | [Estado] |
| Evita la modificación de la clave principal si una clave externa hace referencia a la fila | [Estado] |
| Actualización sobre la tabla hija del valor de la clave externa, y verificar correspondencia con el valor de la clave principal en la tabla padre | [Estado] |

### Triggers
| Items | Observaciones |
|-------|---------------|
| Triggers de inserción definidos | [Estado] |
| Triggers de modificación definidos | [Estado] |
| Triggers de eliminación definidos | [Estado] |
| Triggers de violación de restricción de integridad definidos | [Estado] |
| Triggers de intervalo de tiempo definidos | [Estado] |
| Son suficientes para controlar las operaciones ABM | [Estado] |
| Se utiliza para evitar inconsistencia en caso de redundancia controlada | [Estado] |

### Redundancias
| Items | Observaciones |
|-------|---------------|
| Redundancias creadas | [Estado] |
| Constraints definidos para evitar inconsistencias al crear | [Estado] |
| Medidas para evitar inconsistencias en actualizaciones | [Estado] |

### Código SQL
| Items | Observaciones |
|-------|---------------|
| Consultas SQL definidas | [Estado] |
| Codificación estándar de consultas | [Estado] |
| Reutilización del código SQL | [Estado] |

### Normalización
| Items | Observaciones |
|-------|---------------|
| Primera Forma Normal | [Estado] |
| Segunda Forma Normal | [Estado] |
| Tercera Forma Normal | [Estado] |
| Forma Normal Boyce-Cood | [Estado] |
| Cuarta Forma Normal | [Estado] |

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
El documento ERS contiene un total de [Cantidad de Requerimientos] Requerimientos Funcionales, los cuales se organizan en los siguientes módulos:
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
|----------|---------|------------|-----------|--------------|
| [Cantidad de Requerimientos] | [Cantidad que Cumplen] | [Cantidad que No Cumplen] | [Porcentaje que Cumplen] | [Porcentaje que No Cumplen] |

---

# Evaluación de la Interfaz Gráfica
En términos generales, la interfaz posee un diseño simple pero amigable, sin una utilización excesiva de colores ni opciones muy ocultas en menús de difícil acceso. A continuación se presenta una tabla con los criterios que fueron tomados en cuenta para la evaluación y las observaciones realizadas:

## Confortabilidad de la vista
| Criterio | Observaciones |
|----------|---------------|
| Colores | [Observación] |
| Tipos de fuente | [Observación] |
| Tamaños de fuentes | [Observación] |
| Imágenes | [Observación] |

## Formularios
| Items | Observaciones |
|-------|---------------|
| Cantidad de campos | [Observación] |
| Facilidad de carga | [Observación] |
| Indicación de campos requeridos | [Observación] |
| Validaciones | [Observación] |

## Facilidad de uso
| Items | Observaciones |
|-------|---------------|
| Navegabilidad | [Observación] |
| Disposición de los controles | [Observación] |
| Disponibilidad de ayuda | [Observación] |
| Búsquedas | [Observación] |

---

# Conclusiones
Los resultados obtenidos son, en general, aceptables. Sin embargo, el sistema exhibe comportamientos inadecuados en diversas situaciones de ejecución sencilla. Además, no se ha logrado cumplir con una cantidad considerable de los requerimientos establecidos.

Aunque la interfaz gráfica resulta amigable para el usuario, puede resultar confuso navegar por algunas secciones del proyecto. Por consiguiente, la calidad del software se sitúa en un nivel intermedio y es necesario realizar ajustes para poder utilizar esta aplicación en un entorno formal.

La realización de pruebas exhaustivas fue fundamental para evaluar la calidad del software y detectar los errores presentes. Estos fallos no son fácilmente identificables a simple vista, por lo que sería un error entregar una versión aparentemente final a un cliente sin llevar a cabo dichas evaluaciones.

La realización de pruebas de software puede implicar un trabajo arduo y extenso. Por tanto, resulta importante llevar a cabo una planificación adecuada y una distribución eficiente de las tareas involucradas.

El trabajo de un evaluador de software es de naturaleza compleja, pero sus esfuerzos dan frutos. No hay duda de que llevar a cabo este análisis fue una decisión acertada, y se recomienda realizarlo en proyectos futuros para asegurar siempre altos estándares de calidad.
