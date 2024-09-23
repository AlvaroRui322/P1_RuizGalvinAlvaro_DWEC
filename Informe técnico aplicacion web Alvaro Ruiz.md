## 5. Modelos de ejecución
Los modelos de ejecución en cliente y servidor son arquitecturas de software que básicamente determinan dónde se ejecuta el código de una aplicación. 
El funcionamiento básico de la arquitectura cliente servidor es la siguiente: El cliente hace una petición al servidor de algún recurso de nuestra aplicación y el servidor recibe la petición, procesa los resultados a mostrar y lo muestra de nuevo al cliente.
En esta imagen se puede observar el funcionamiento de esta arquitectura de manera gráfica:

![Funcionamiento básico del modelo cliente - servidor](./imagenes/funcionamiento%20modelo%20cliente%20servidor.png)

A continuación voy a pasar a describir y explicar las principales características, diferencias y ejemplos de uso de ambas arquitecturas

### Modelo de ejecución en Cliente
En este modelo el código se ejecutaría directamente en el dispositivo del usuario

### Modelo de ejecución en Servidor

### Ventajas e inconvenientes

### Tabla comparativa de ambos modelos

| Característica             | Ejecución en Cliente                                              | Ejecución en Servidor                                           |
| -------------------------- | ----------------------------------------------------------------- | --------------------------------------------------------------- |
| Ubicación del procesamiento | En el dispositivo del cliente (navegador o aplicación).           | En el servidor remoto.                                          |
| Interactividad              | Muy alta, actualizaciones en tiempo real sin recargar la página.  | Menor, requiere comunicación continua con el servidor.           |
| Rendimiento                 | Depende de la potencia del dispositivo del usuario.               | Depende de la capacidad del servidor.                            |
| Seguridad                   | Mayor riesgo de manipulación, ya que el código es visible para el usuario. | Mayor control de seguridad, el código no es visible para el cliente. |
| Carga de datos              | Los recursos se cargan al principio, lo que puede aumentar el tiempo de carga inicial. | Los datos se cargan dinámicamente según la solicitud.            |
| Escalabilidad               | Escalable mediante la distribución de la carga en los dispositivos de los usuarios. | Escalable aumentando los recursos del servidor o mediante balanceo de carga. |

## 6. Lenguajes de programación web

## 7. Tecnologías a utilizar

## 8. Compatibilidad en navegadores
