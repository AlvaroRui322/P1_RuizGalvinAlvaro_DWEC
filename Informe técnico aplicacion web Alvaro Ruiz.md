## 5. Modelos de ejecución

Los modelos de ejecución en cliente y servidor son arquitecturas de software que básicamente determinan dónde se ejecuta el código de una aplicación. 
El funcionamiento básico de la arquitectura cliente servidor es la siguiente: El cliente hace una petición al servidor de algún recurso de nuestra aplicación y el servidor recibe la petición, procesa los resultados a mostrar y lo muestra de nuevo al cliente.
En esta imagen se puede observar el funcionamiento de esta arquitectura de manera gráfica:

![Funcionamiento básico del modelo cliente - servidor](./imagenes/funcionamiento%20modelo%20cliente%20servidor.png)

Dentro de la arquitectura cliente - servidor existen 3 tipos:
- Arquitectura de dos capas: En este tipo el cliente solicita recursos y el servidor responde directamente con sus propios recursos sin niguna capa extra.
- Arquitectura de tres capas: Se compone de una capa para el cliente, otra para el servidor y otra denominada servidor de datos que proporciona al servidor los datos necesarios para procesar el servicio que solicita el cliente.
- Arquitectura de N capas: Es como la arquitectura de 3 capas solo que usando N servidores que brindan un servicio en específico al servidor cada uno. 

### Modelo de ejecución en cliente

Este modelo implica que la mayor parte de la carga de procesamiento ocurre en el dispositivo (cliente). Aquí, los datos y la lógica se ejecutan localmente. Las tecnologías involucradas incluyen lenguajes como JavaScript, HTML y CSS, que permiten la interacción directa con el usuario del navegador. Un ejemplo típico es cuando un sitio web responde a la interacción del usuario sin necesidad de comunicarse constantemente con el servidor, como ocurre con animaciones o validaciones de formularios en tiempo real.

#### Ventajas
- Menor latencia: Las acciones del usuario no requieren enviar solicitudes al servidor, lo cual se traduce en una reducción del tiempo de espera.
- Experiencias interactivas: Las aplicaciones pueden reaccionar rápidamente a los eventos del usuario, lo que mejora la usabilidad.

#### Desventajas
- Limitado por el dispositivo: La capacidad de procesamiento depende del hardware del cliente, que puede ser menos potente que un servidor dedicado.


### Modelo de ejecución en servidor

En este modelo el servidor realiza la mayor parte del procesamiento. El cliente envía solicitudes y recibe las respuestas procesadas por el servidor, que puede encargarse de la gestión de bases de datos, procesamiento de la lógica y almacenamiento. Varios ejemplos pueden ser aplicaciones web que dependen de consultas a bases de datos o sistemas que manejan grandes cantidades de información en segundo plano, como Facebook o Netflix, donde el contenido y las solicitudes se gestionan desde servidores remotos

#### Ventajas
- Mayor capacidad de procesamiento: Los servidores están diseñados para manejar múltiples peticiones a la vez y procesar grandes volúmenes de datos, ofreciendo más rendimiento que los dispositivos clientes.
- Seguridad y centralización: Los datos sensibles pueden gestionarse y protegerse mejor cuando están almacenados y procesados en servidores, lo que facilita la administración.

#### Desventajas
- Dependencia del servidor: Si el servidor falla, todos los clientes que dependen de él no podrán acceder al servicio.
- Latencia: Cada vez que el cliente necesita algo, debe esperar a que el servidor procese la solicitud, lo que puede aumentar los tiempos de respuesta.

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

Los lenguajes de programación más utilizados en el desarrollo web 
## 7. Tecnologías a utilizar

### Lenguajes a utilizar

Para el desarrollo de mi aplicación utilizaré:
- HTML5 para crear la estructura de la aplicación web.
- CSS3 para definir el diseño y la presentación visual de mi aplicación.
- JavaScript para programar la lógica de la aplicación.

### Frameworks

Por lo que investigué (ya que nunca vi ninguno de los frameworks que voy a mencionar) los frameworks más usados para el desarrollo web en JavaScript son React.js para el Frontend y Node.js para el Backend.

- React.js lo usaría como dije anteriormente para el desarrollo en frontend. React facilita la creación de componentes reutilizables y ofrece una excelente gestión del estado de la aplicación. En este curso daremos React, por lo que en un 99,9% usaré este framework de Javascript para el frontend.
- Node.js lo usaré en el lado del servidor. Por lo visto node es un entorno que permite ejecutar JavaScript en el servidor, por lo que eso significa que unificaría el desarrollo de la aplicación tanto en cliente como en servidor usando un único lenguaje.

### Herramientas de desarrollo 

He optado por el uso de Visual Studio Code como herramienta debido a que es muy versátil para el desarrollo y ofrece una gran variedad de extensiones y funciones para facilitar el trabajo. Además para el control de versiones usaré git y github que ya lo hemos utilizado en otros años.


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
- [Arquitectura cliente servidor: qué es, tipos y ejemplos](https://www.arsys.es/blog/todo-sobre-la-arquitectura-cliente-servidor)
- [¿Qué es el modelo cliente-servidor? Pros y contras](https://www.ionos.mx/digitalguide/servidores/know-how/modelo-cliente-servidor/)
- [Cliente-servidor](https://es.wikipedia.org/wiki/Cliente-servidor)
- [¿Qué tendencias en Desarrollo Web veremos en el 2023?](https://blog.impulse.lat/que-tendencias-en-desarrollo-web-veremos-en-el-2023)
- [Tecnologías Web Más Populares](https://wheelhub.es/blog/tipos-de-tecnologia-web/)
- [Descripción de las tecnologías JavaScript](https://developer.mozilla.org/es/docs/Web/JavaScript/JavaScript_technologies_overview)
- [10 motivos para usar Node.js para desarrollar aplicaciones web](https://www.universia.net/es/actualidad/habilidades/10-motivos-usar-nodejs-desarrollar-aplicaciones-web-1154033.html)
