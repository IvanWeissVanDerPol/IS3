# Planificación de las Actividades

## Introducción
La planificación adecuada de las actividades es esencial para el éxito de cualquier proyecto. En esta sección, detallamos la planificación de las actividades del trabajo práctico de pruebas exhaustivas sobre el Sistema de Gestión de Contenidos (CMS).

## Tabla de Planificación

| Id  | Nombre de tarea                                                                          | Duración | Comienzo | Fin  | Predecesoras        | Nombres de los recursos  |
|-----|------------------------------------------------------------------------------------------|----------|----------|------|---------------------|--------------------------|
| 1   | Reunión inicial con los desarrolladores del sistema, obtención del código fuente y documentación | 3 horas  | 01/06/24 | 01/06/24 |                     | Iván, Cami, Fran, Jova   |
| 2   | Instalación de software necesario y ejecución inicial                                     | 1 hora   | 02/06/24 | 02/06/24 | 1                   | Iván, Cami, Fran, Jova   |
| 3   | Inspección de código                                                                      | 2 días   | 03/06/24 | 04/06/24 | 1, 2                | Iván, Cami               |
| 4   | Inspeccionar características de facilidad de prueba                                       | 1 día    | 05/06/24 | 05/06/24 | 1, 2, 3             | Iván, Jova               |
| 5   | Análisis del modelo de datos                                                              | 1 día    | 06/06/24 | 06/06/24 | 1, 2, 3             | Cami, Fran               |
| 6   | Pruebas de inspección de código                                                           | 2 días   | 07/06/24 | 08/06/24 | 1, 2, 3             | Iván, Jova               |
| 7   | Realización de casos de prueba                                                            | 3 días   | 09/06/24 | 11/06/24 | 1, 2, 3, 4          | Cami, Fran               |
| 8   | Pruebas de stress                                                                         | 1 día    | 12/06/24 | 12/06/24 | 1, 2, 3, 4          | Iván, Jova               |
| 9   | Verificación de los requerimientos funcionales y no funcionales                           | 4 días   | 13/06/24 | 16/06/24 | 1, 2, 3             | Cami, Fran               |
| 10  | Evaluación de la interfaz gráfica                                                         | 1 día    | 17/06/24 | 17/06/24 | 1, 2, 3             | Iván, Jova               |
| 11  | Realización del paper                                                                     | 3 días   | 18/06/24 | 20/06/24 | 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 | Todos                   |
| 12  | Realización de diapositivas para presentación                                             | 1 día    | 21/06/24 | 21/06/24 | 11                  | Cami, Fran               |
| 13  | Organización de la presentación                                                           | 2 días   | 22/06/24 | 23/06/24 | 12                  | Todos                   |

## Diagrama de Gantt
A continuación se presenta el diagrama de Gantt que visualiza la planificación de las actividades:

![Diagrama de Gantt](TrabajoPractico/Documentacion/Online Gantt 20240623.png)

## Detalles de las Actividades
### 1. Reunión inicial con los desarrolladores del sistema
- **Objetivo**: Obtener el código fuente y la documentación necesaria para iniciar el proyecto.
- **Duración**: 3 horas
- **Recursos**: Iván, Cami, Fran, Jova

### 2. Instalación de software necesario y ejecución inicial
- **Objetivo**: Configurar el entorno de desarrollo y asegurar que el sistema CMS se ejecuta correctamente.
- **Duración**: 1 hora
- **Recursos**: Iván, Cami, Fran, Jova

### 3. Inspección de código
- **Objetivo**: Revisar el código fuente para identificar posibles errores y áreas de mejora.
- **Duración**: 2 días
- **Recursos**: Iván, Cami

### 4. Inspeccionar características de facilidad de prueba
- **Objetivo**: Evaluar si el sistema cumple con las características teóricas de facilidad de prueba.
- **Duración**: 1 día
- **Recursos**: Iván, Jova

### 5. Análisis del modelo de datos
- **Objetivo**: Verificar la integridad y normalización del modelo de datos.
- **Duración**: 1 día
- **Recursos**: Cami, Fran

### 6. Pruebas de inspección de código
- **Objetivo**: Realizar pruebas detalladas de inspección de código utilizando herramientas específicas.
- **Duración**: 2 días
- **Recursos**: Iván, Jova

### 7. Realización de casos de prueba
- **Objetivo**: Desarrollar y ejecutar casos de prueba para validar las funcionalidades del sistema.
- **Duración**: 3 días
- **Recursos**: Cami, Fran

### 8. Pruebas de stress
- **Objetivo**: Determinar el rendimiento del sistema bajo condiciones de alta carga.
- **Duración**: 1 día
- **Recursos**: Iván, Jova

### 9. Verificación de los requerimientos funcionales y no funcionales
- **Objetivo**: Asegurar que el sistema cumple con los requerimientos especificados.
- **Duración**: 4 días
- **Recursos**: Cami, Fran

### 10. Evaluación de la interfaz gráfica
- **Objetivo**: Evaluar la usabilidad y la experiencia del usuario.
- **Duración**: 1 día
- **Recursos**: Iván, Jova

### 11. Realización del paper
- **Objetivo**: Documentar todos los hallazgos y resultados del proyecto.
- **Duración**: 3 días
- **Recursos**: Todos

### 12. Realización de diapositivas para presentación
- **Objetivo**: Preparar las diapositivas para la presentación final del proyecto.
- **Duración**: 1 día
- **Recursos**: Cami, Fran

### 13. Organización de la presentación
- **Objetivo**: Ensayar y organizar la presentación final.
- **Duración**: 2 días
- **Recursos**: Todos

## Riesgos y Mitigaciones
### Riesgos Identificados
- **Retrasos en la entrega del código fuente**: Puede afectar la planificación inicial.
- **Problemas técnicos durante la instalación del software**: Podrían retrasar el inicio de las actividades.
- **Alta complejidad del código**: Podría requerir más tiempo del previsto para la inspección y pruebas.

### Estrategias de Mitigación
- **Comunicación constante con los desarrolladores**: Asegurar que el código fuente y la documentación se entreguen a tiempo.
- **Preparación de un entorno de desarrollo alternativo**: Tener un plan de respaldo para la instalación del software.
- **Asignación de recursos adicionales**: En caso de encontrar alta complejidad, asignar más tiempo y recursos para la inspección y pruebas del código.

## Conclusión
La planificación detallada de las actividades nos permite tener una visión clara del trabajo necesario para completar el proyecto de pruebas exhaustivas sobre el CMS. La coordinación efectiva y la gestión de riesgos son clave para asegurar el éxito del proyecto.
