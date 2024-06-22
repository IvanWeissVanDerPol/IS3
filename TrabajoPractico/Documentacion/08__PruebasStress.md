# Pruebas de Estrés

### 2.2 Herramientas Utilizadas
- **JMeter**: Utilizado para realizar las peticiones en paralelo a la página inicial de login del sistema.

### 2.3 Proceso de Pruebas
Se realizo peticiones en paralelo de la pagina principal del software.

## 3. Casos de Prueba de Estrés
### 3.1 Descripción de Casos de Prueba

| Número de Peticiones | Número de Hilos (Threads) | Periodo de Incremento (Ramp-Up Period) | Número de Repeticiones (Loop Count) |
| -------------------- | ------------------------- | -------------------------------------- | ----------------------------------- |
| 500                  | 500                       | 10                                     | 1                                   |
| 1000                 | 1000                      | 20                                     | 1                                   |
| 2000                 | 2000                      | 40                                     | 1                                   |
| 3000                 | 3000                      | 60                                     | 1                                   |
| 4000                 | 4000                      | 80                                     | 1                                   |
| 5000                 | 5000                      | 90                                     | 1                                   |
| 6000                 | 6000                      | 100                                    | 1                                   |

## 4. Resultados de las Pruebas de Estrés

| Número de peticiones | Promedio ms | Min ms | Max ms | Std. Dev. ms | Error % | Rendimiento  sec | KB/seg recibido | KB/seg enviado | Bytes promedio |
| -------------------- | ----------- | ------ | ------ | ------------ | ------- | ---------------- | --------------- | -------------- | -------------- |
| 500                  | 4762        | 59     | 9207   | 2633.99      | 0 %     | 26.1/sec         | 930.57          | 2.95           | 36563          |
| 1000                 | 9323        | 50     | 18188  | 5249.33      | 0 %     | 26.2/sec         | 935.30          | 2.97           | 36563          |
| 2000                 | 18428       | 49     | 35906  | 10348.07     | 0 %     | 26.4/sec         | 941.01          | 2.99           | 36563          |
| 3000                 | 27689       | 52     | 53926  | 15571.32     | 0 %     | 26.3/sec         | 940.42          | 2.98           | 36563          |
| 4000                 | 36918       | 52     | 60017  | 19838.80     | 22.30 % | 28.6/sec         | 794.84          | 3.24           | 28428.8        |
| 5000                 | 45617       | 56     | 92522  | 22887.27     | 43.50 % | 28.1/sec         | 570.86          | 3.18           | 20901.2        |
| 6000                 | 50200       | 54     | 92520  | 21551.30     | 59.20 % | 31.2/sec         | 460.30          | 3.53           | 15112.5        |


### 5.1 Conclusiones
Se concluye que el servidor la cual se realizo la pruba cuenta con un buen rendimiento ya que a partir de 4000 peticiciones en paralelo empieza a responder con errores con un 22.3 % de las peticiones.

### 5.2 Recomendaciones
Para el sistema se recomienda ejecutar en infraestructuras dedicadas y aisladas, ya que esto puede afectar el rendimiento de la misma.

### 7. Especificaciones del Entorno de Pruebas
Las características de la máquina en que se realizaron las pruebas son las siguientes:
- **Procesador**: AMD Ryzen 7 5700X 3.4 Ghz 16 Core CPU 
- **RAM**: 32GB 3200 Mhz DDR4
- **Almacenamiento**: 3 TB SSD

