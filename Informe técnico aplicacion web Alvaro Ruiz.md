## 5. Modelos de ejecución

Los modelos de ejecución en cliente y servidor son arquitecturas de software que básicamente determinan dónde se ejecuta el código de una aplicación. 
El funcionamiento básico de la arquitectura cliente servidor es la siguiente: El cliente hace una petición al servidor de algún recurso de nuestra aplicación y el servidor recibe la petición, procesa los resultados a mostrar y lo muestra de nuevo al cliente.
En esta imagen se puede observar el funcionamiento de esta arquitectura de manera gráfica:

![Funcionamiento básico del modelo cliente - servidor](./imagenes/funcionamiento%20modelo%20cliente%20servidor.png)

Dentro de la arquitectura cliente - servidor existen 3 tipos:
- Arquitectura de dos capas: En este tipo el cliente solicita recursos y el servidor responde directamente con sus propios recursos sin niguna capa extra.
- Arquitectura de tres capas: Se compone de una capa para el cliente, otra para el servidor y otra denominada servidor de datos que proporciona al servidor los datos necesarios para procesar el servicio que solicita el cliente.
- Arquitectura de N capas: Es como la arquitectura de 3 capas solo que usando N servidores que brindan un servicio en específico al servidor cada uno. 




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



### 7.1 Lenguajes de programación y lenguajes de marcas
Para llevar a cabo este proyecto tengo planteada la utilización de HTML5, CSS3 y JavaScript como lenguajes principales

## 8. Compatibilidad en navegadores

La compatibilidad entre navegadores es un reto común en el desarrollo web, ya que cada uno puede interpretar JavaScript, HTML y CSS de manera diferente. Esto puede provocar que una página web no se vea o funcione igual en todos los navegadores.

### JavaScript

JavaScript es esencial para la interactividad, pero no todos los navegadores soportan igual las características más modernas, como async/await o la API Fetch. Los Navegadores antiguos como Internet Explorer suelen tener más problemas con estas funciones. Para solucionarlo, se usan polyfills (que emulan funciones modernas) y transpiladores como Babel, que convierten el código actual en uno más antiguo y compatible.

### HTML y CSS

HTML y CSS también presentan problemas de compatibilidad, sobre todo con nuevas propiedades como CSS Grid o Flexbox. Herramientas como los autoprefixers añaden automáticamente prefijos necesarios para asegurar que los estilos funcionen en todos los navegadores (por ejemplo, -webkit- para Safari). Además el uso de reset.css o normalize.css ayuda a que los navegadores interpreten el código de manera más uniforme.

### Impacto de JavaScript con HTML y CSS

Combinar JavaScript con HTML y CSS puede afectar tanto a la compatibilidad como al rendimiento. Usar mucho JavaScript para modificar el contenido puede hacer la página más lenta, sobre todo en navegadores antiguos. Es mejor dejar que HTML y CSS manejen la estructura y el diseño siempre que sea posible.

### Soluciones y herramientas

Para evitar problemas de compatibilidad, se deben hacer pruebas en varios navegadores. Herramientas como BrowserStack permiten simular diferentes entornos. Además, las herramientas de desarrollo de cada navegador facilitan la detección y corrección de errores.

## Referencias

- [How to solve Javascript Browser Compatibility issues](https://www.browserstack.com/guide/resolve-javascript-cross-browser-compatibility-issues)
- [How to Handle JavaScript Cross-Browser Compatibility issues](https://blog.pixelfreestudio.com/how-to-handle-javascript-cross-browser-compatibility-issues/https://blog.pixelfreestudio.com/how-to-handle-javascript-cross-browser-compatibility-issues/)
- [Cross-Browser Compatibility Testing](https://www.freecodecamp.org/news/cross-browser-compatibility-testing-best-practices-for-web-developers/)
- [Handling common HTML and CSS problems](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Cross_browser_testing/HTML_and_CSS)
- 
