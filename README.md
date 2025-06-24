# Prueba Técnica Fullstack/Leader

## Introducción

Para la realización de esta prueba técnica se planteará un posible caso real en el que liderarás el desarrollo de una nueva línea de negocio de principio a fin, te encargarás de hacer la toma de requisitos, la planificación de la arquitectura, el cálculo de costes/tiempo, y las primeras estructuras básicas de los repositorios necesarios para marcar los pasos a seguir por el resto del equipo de desarrollo.

## Proyecto

Un agente del sector turístico con más de 50 años en el sector, se pone en contacto con nosotros para que nos hagamos cargo de su tecnología y le ayudemos a escalar y llevar a cabo sus proyecciones de futuro.

Este proyecto es un buscador de vuelos líder en el sector, y siempre han colaborado con otra consultoría de software, pero con el paso del tiempo, esta tecnología ha quedado anticuada, además de que su actual partner está poniendo muchos frenos en las nuevas mejoras y al espíritu innovador de nuestro cliente.

De hecho esta propuesta sale, porque necesitan de una nueva web moderna y fresca que permita operar con toda su operativa de negocio, pero que use nuevas tecnologías. Su actual consultora se ha negado a realizar esta parte ya que no entra dentro de su zona de confort, y han propuesto buscar otro proveedor que se encargue de esta finalidad (nosotros).

#### Las líneas de negocio del cliente son:

- Una primera versión del software que venden como SaaS a sus propios clientes, donde ofrecen poder reservar y gestionar vuelos a través de su propio código IATA.
- Una conexión HTTP para que se conecten otros agentes turísticos y usar los mismos servicios SaaS pero a través de una API en XML para clientes técnicos u otras agencias turísticas digitales.
- Una copia de todo el sistema que vende como marca blanca a otros agentes turísticos pero con funcionalidades limitadas, con imagen y estilos personalizados.

#### El cliente nos comenta su stack actual:

- El sistema se almacena en máquinas virtuales de Windows, que se replican por entornos y diferentes proyectos.
- Su sistema se divide en 4 principales actores:
  - Un backend en .NET que gestiona datos en una DB y se conecta con proveedores.
  - Un admin Dashboard en .NET para gestionar el software por parte del cliente y sus empleados.
  - Una web en AngularJS para los clientes de nuestro cliente, donde ejecutan búsquedas y reservas de vuelos.
  - Un script que se puede poner en otras web y otorgar parte de la funcionalidad.
- Toda la información se guarda en una base de datos de SQL Server.
- La conexión entre la web de sus clientes y el backend se realiza por API REST.
- La conexión entre el backend y proveedores externos se realiza por XML.
- El admin dashboard y el backend corren en un monolito con el mismo código, donde es el propio backend el que renderiza el HTML.
- La web que vende como marca blanca esta en Angular 10 echo por otra consultora.

#### Preocupaciones del cliente:

- Que su software pueda quedarse anticuado.
- Que no pueda escalar de forma eficiente, ya que planean abrir a toda Sudamérica el próximo año.
- Tener demasiada dependencia de otra consultora que está frenando la innovación.
- Poner en riesgo su actual operativa, ya que el sistema no se puede parar.
- No cumplir con el reglamento europeo o estar expuesto a hackers.
- Que la otra consultora se tome mal las reformas y las boicoteen desde dentro.
- Que el sistema se ralentice por la gran cantidad de datos.
- La pérdida de datos por algún error de software.
- Que le aumenten mucho los costos de servidores por nuestra propuesta.
- Que aumente el costo del motor de búsquedas, ya que su proveedor le cobra por cada búsqueda que se ejecuta en el sistema.
- Que la nueva propuesta no cumpla con toda la operativa de su negocio.
- Que cargemos mucho de trabajo a la otra consultora y se queje.
- Que no pueda llevar a cabo alguna idea porque la otra consultora no la quiere hacer.

#### Que quiere conseguir:

- Una nueva web bonita y adaptable a todos los dispositivos.
- Seguir trabajando con su actual consultora en paralelo.
- Tener una alternativa con nosotros para nuevas funcionalidades que su actual consultora se niegue a hacer.
- Unificar los proyectos del SaaS y la marca blanca para que usen las mismas funcionalidades y así aprovechar el desarrollo de una empresa para la otra.
- Mejorar el filtrado y tiempo de respuesta de los resultados de búsqueda, ya que cada petición nos devuelve unos 100k resultados, y nuestros agentes necesitan filtrarlos por fecha, aerolínea, tipo de operativa, maletas, horarios de llegada/salida, precio, y otros más.
- Tener una solución de analítica completa para su software, ya que ahora mismo no disponen de ninguna, tienen que sacar los datos a mano, y ademas la otra consultora pasa los datos mas antiguos de 5 años a discos duros para que la base de datos no se pete.
- También les gustaría poder medir el tráfico y costes de cada uno de sus clientes, para poder facturar a conciencia a cada uno de ellos.
- Responde a la pregunta, ¿cuál fue tu decisión técnica más polémica?
- Conseguir un SLA del 99.95%.
- Contar con una garantía de calidad que asegure el correcto funcionamiento de la solución.

## Propuesta

Desarrolla la mejor propuesta que puedas, y calcula qué partes podría reducir si el cliente no aprueba el desarrollo.

- Analizar la información recogida.
- Desarrollar una toma de requisitos.
- Planificar una arquitectura (Miro o similar).
- Seleccionar la tecnología y los protocolos de comunicación.
- Infraestructura a usar.
- Planificar un sistema de autenticación seguro y confiable.
- Usar todo lo posible open source.
- Cálculo de costes.
- Número de perfiles y tiempo estimado.
- Responde a la pregunta, ¿cuál fue tu última estimación que fallaste?
- Qué sistema organizativo harías y cómo lo ejecutarías.
- Montar los repositorios necesarios según la tecnología ofrecida.
- Responder a las siguientes preguntas.

## Preguntas

- ¿Cómo manejarías overbooking de tráfico del 1000% durante alguna franja de temporada alta?
- ¿Cómo ahorrarías costes en temporada baja?
- ¿Cómo garantizarías 0 downtime durante una migración?
- ¿Cómo garantizarías la calidad de código y el software?
- ¿Cómo harías un booking confirmation, síncrono o asíncrono?
