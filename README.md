# EscornaSnap
EscornaSnap! - Escornabot controlado desde Snap! - Proyecto Noise>

Esto es una versión preliminar, donde voy a tratar de describir los pasos a seguir. Si encuentras algún fallo, no lo tienes muy claro, o para resolver cualquier duda, estamos en Twitter: @proyectonoise.

1.- Antes de nada, para controlar Escornabot con EscornaSnap, te aviso que necesitas tener Bluetooth en el Escornabot y en el PC. Podrías conectarte por cable USB pero te va a resultar un tanto engorroso. (Aunque, si el cable USB es largo, para hacer pruebas, sirve).

2.- Debes descargar e instalar Snap4Arduino en http://snap4arduino.rocks/ Tienes versiones para varios sistemas operativos.
Snap4Arduino (creado por Bernat Romagosa) es una versión de Snap! para ser usada con Arduino (Snap! es un entorno de programación de bloques, creado por Jens Mönig, parecido a Scratch pero con muchísimas más posibilidades que te permiten usar programación más avanzada).

3.- Dentro de Snap4Arduino debes importar los bloques de EscornaSnap, que hay en este repositorio, con extensión .XML
La forma más sencilla es arrastrar el archivo dentro de Snap4Arduino. 

4.- Debes cargar, desde el entorno Arduino, el Firmata para Escornabot, que puedes encontrar en este repositorio. Para subirlo al Arduino Nano del Escornabot, debes usar el cable USB. (Este firmata es una adaptación para Escornabot, del creado en el Citilab)

5.- Una vez transferido, debes conectar el módulo Bluetooth a Escornabot. Pero antes debes quitar el cable USB, para que no interfiera con el módulo bluetooth. 
Para ello, conecta el módulo Bluetooth (Yo uso el HC04, pero supongo que el HC06 funcionará también) al Arduino Nano: el pin TX del módulo con el pin RX del Arduino y el pin RX del módulo con el pin TX del Arduino. Los pines de alimentación del módulo irán a alimentación (5 V. y GND). En el Escornabot modelo Audacius irán a las correspondientes conexiones de la protoboard y si no hay  huecos suficientes habrá que hacer un puente a las lineas disponibles de la protoboard para así dsponer de alimentación. En otros modelos de Escornabot ya hay pines para conectar directamente el módulo Bluetooth.

6.-  Emparejar el Bluetooth del PC y el módulo.

7.- Una vez emparejado. Desde Snap4Arduno, en los bloques que aparecen al pulsar la pestaña 'Arduino' ,de color azul claro, pulsa el botón 'Connect Arduino'. Elige el puerto correspondiente (si te salen 2 puertos del módulo Bluetooth, generalmente es el primero). Debería, despues, salir un mensaje indicando que ha conectado correctamente.

8.- Pulsa el botón gris 'otros' y verás los bloques de EscornaSnap. que puedes usar para manejar Escornabot. Es conveniente que antes de empezar caulquier programa, uses en primer lugar el bloque 'Iniciar EscornaSnap' dónde tendrás que poner los valores de lectura analógica de cada uno de los botones. Si no sabes de qué estoy hablando, imagino que eres nuevo en el mundo Escornabot. Si es así, te aconsejo que visites antes la web de Pablo Rubio (escornafan) https://pablorubma.cc/ donde podrás encontrar toda al información imaginable acerca de Escornabot.

9.- Disfruta de EscornaSnap. ¡A programar!



