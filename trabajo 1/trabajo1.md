# Describa un ejemplo de un sistema distribuido en base a los estudiado    
Los sistemas distruibos son una coleccion de host independiente y autónomos conectados atraves de una red 
de comunicación o bien es una colección de servicios a los que se accede atraves de interfaces basadas en 
la red.

   Segun lo estudiado y un poco de analice, un sistema distribuido son un conjunto de computadoras conectadas entre si,como sabemos cada una de ella esta en un cierto punto del mundo pues ese es su proposito estar separadas fisicamente para poder abastecer a muchas personas atraves de una misma red.

Los sistemas distribuidos son utilizados para muchos casos se podria decir, un ejemplo podria ser los juegos en linea que son multijugador a como sabemos este tipo de juego generalmente se espearce por el mundo es ahi donde la empresa necesita uno de esto. 




## Breve resumen de las arquitecturas
1.	Arquitecturas en capas.<p> 

La idea básica para el estilo en capas es sencilla: los componentes se estructuran  a modo de capas, donde al componente de la capa se le permite llamar a componentes de la capa, pero no del resto de capas. Este estilo se ha adoptado ampliamente en la comunidad de redes. Una observación clave es que el control generalmente fluye de capa a capa: las peticiones se mueven hacia abajo en la jerarquía mientras que los resultados se mueven hacia arriba.
2. Arquitecturas basadas en objetos. <p>

Las arquitecturas basadas en objetos. En esencia, cada objeto corresponde a lo que hemos definido como componente, y estos componentes se conectan a través de un mecanismo de llamadas a procedimientos (remotos). Sin ser sorprendente, esta arquitectura de software coincide con la arquitectura de sistemas cliente-servidor que describimos antes. La arquitectura basada en capas y la basada en objetos aún son los estilos más importantes utilizados para implementar grandes sistemas de software.
3. Arquitecturas centradas en datos.<p>

Las arquitecturas centradas en datos evolucionaron alrededor de la idea de que los procesos se comunican a través de un repositorio común (activo o pasivo). Se puede argumentar que, para sistemas distribuidos, estas arquitecturas son tan importantes como las basadas en capas y objetos. Por ejemplo, un punto a favor que han desarrollado las aplicaciones en red es que se basan en un sistema de archivos distribuidos compartidos donde casi todas las comunicaciones se realizan a través de archivos. De manera similar, los sistemas distribuidos basados en la web, los procesos se comunican a través de servicios de datos compartidos basados en la web.
 4. Arquitecturas basadas en eventos.
En las arquitecturas basadas en eventos, los procesos se comunican básicamente a través de la propagación de eventos, los que opcionalmente transportan datos,


    
## Arquitecturas descentralizadas
    Son una consecuencia directa de dividir aplicaciones para obtener una interfaz de usuario, componentes de procesamiento, y un nivel de datos. Los diferentes niveles corresponden directamente a la organización lógica de las aplicaciones. En la mayor parte de los ambientes de negocios, el procesamiento distribuido equivale a organizar una aplicación cliente-servidor en la forma de una arquitectura multiniveles. Nos referimos a este tipo de distribución como distribución vertical. La característica clásica de la distribución vertical es que se logra colocando lógicamente los diferentes componentes en diferentes máquinas. El término se relaciona con el concepto de fragmentación vertical según es utilizado en bases de datos relacionales distribuidas, donde significa que las tablas se dividen por ancho de columna, y posteriormente se distribuyen a través de diversas máquinas (Oszu y Valduriez, 1999).

    Desde un punto de vista de administración de sistemas, tener una distribución vertical puede ayudar puesto que: las funciones están lógica y físicamente divididas en diversas máquinas, y cada máquina se configura a la medida para un grupo específico de funciones. Sin embargo, la distribución vertical es sólo una manera de organizar aplicaciones cliente-servidor.En arquitecturas modernas, con frecuencia lo que cuenta es la distribución de clientes y servidores, y a esto nos referimos como distribución horizontal.  En este tipo de distribución, un cliente o un servidor pueden dividirse físicamente en partes lógicas equivalentes, pero cada parte opera en su propio espacio del conjunto de datos, lo que equilibra la carga.  En esta sección veremos un
    tipo de arquitectura moderna, llamada sistemas punto a punto, que da soporte a la distribución horizontal.

    Desde una perspectiva de alto nivel, todos los procesos que constituyen un sistema de punto a punto son iguales. Esto significa que las funciones que necesitan realizarse están representadas por cada proceso constituyente del sistema distribuido. Como consecuencia, mucha de la interacción
    ocurrida entre los procesos es simétrica: cada proceso actuará como cliente y servidor al mismo tiempo (a esto se le denomina también que actúa como sirviente).

    Dado este comportamiento simétrico, las arquitecturas de punto a punto evolucionan alrededor de la forma de cómo organizar los procesos en una red sobrepuesta, es decir, una red en la que los nodos estén formados por los procesos, y los vínculos representan los posibles canales de comunicación (a los cuales generalmente se les conoce como conexiones TCP). En general, un proceso no puede comunicarse directamente con otro proceso cualquiera, en vez de eso, necesita enviar mensajes a través de los canales de comunicación disponibles.

    Existen dos tipos de redes sobrepuestas: las que están estructuradas, y las que no lo están. Estos dos tipos son ampliamente tratados en Lua y colaboradores (2005), junto con muchos ejemplos. Aberer y colaboradores (2005) proporciona una arquitectura de referencia que permite hacer una comparación más formal de los diferentes tipos de sistemas de punto a punto. Androutsellis-Theotokis y Spinellis (2004) proporcionan una explicación desde una perspectiva de distribución de contenidos.


## Arquitecturas hibridas
    Estos sistemas se utilizan en internet donde los
    servidores se colocan “al borde” de la red. Este borde está formado por el límite que hay entre las redes empresariales y la internet real, por ejemplo, como lo proporciona un proveedor de servicios de internet (ISP, por sus siglas en inglés). De igual manera, donde los usuarios finales en
    casa se conectan a internet, a través de su ISP, podemos considerar que éste se encuentra al bordede internet.

    Los usuarios finales, o clientes en general, se conectan a internet mediante un servidor lateral.

    El objetivo principal del servidor lateral es proporcionar contenido, probablemente después de realizar un filtrado y descodificar funciones. Más interesante resulta el hecho de que una colección de servidores laterales pueda utilizarse para optimizar la distribución de contenido y aplicaciones. El modelo básico es que, para una organización específica, un servidor lateral actúa como servidor de origen a partir del cual se origina todo el contenido. Ese servidor puede utilizar otros servidores laterales para replicar páginas web y similares (Leff y cols., 2004; Nayate y cols., 2004; y Rabinovich
    y Spatscheck, 2002).

