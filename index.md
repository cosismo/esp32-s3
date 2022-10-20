### ESP32S3 Dev kit

### Última Actualización: 20/octubre/2022
Bienvenido al AIoT: Internet de las Cosas + Inteligencia Artificial

Si llegaste hasta aquí, sabrás que estás en la avanzada tecnológica de estos chips, por lo que la información actual es limitada, breve y cambiará con frecuencia. Te recomendamos revisarla constantemente.
A continuación te ofrecemos la información más básica hasta el momento. En la medida de lo posible la iremos actualizando.  También puedes ir a las fuentes directas que te ofrecemos a continuación.

Para comenzar a utilizar tu ESP32S3 y encontrar toda la información técnica, te recomendamos las siguientes ligas:

* Pinout   
![esp32s3 pinout](https://raw.githubusercontent.com/cosismo/esp32-s3/gh-pages/Purple-S3-pinout.png)


* Facebook.
[Grupo de Facebook en español sobre Internet de las Cosas](https://www.facebook.com/groups/724628401049648/)

* Actualización 20/10/2022. La versión 2.05, liberada el 16/09/2022 funciona con esta placa. Sólo es necesario actualizar la versión de Adafruit Pixel a la última disponible (1.10.6) para qeu funcione con el sketch que se incluye en la parte de abajo de este documento (Sketch Blink LED RGB en Arduino IDE).
* Actualización 17/09/2022:  En nuestras pruebas y por reportes hemos notado que la versión que funciona consistentemente con el ESP32S3 es la 2.0.3 Es la que te recomendamos.   NOTA IMPORTANTE:  LA VERSIÓN 2.0.4 HA REPORTADO PROBLEMAS Y NO FUNCIONA CON ESTA PLACA. AÚN SI LA REGRESAS A LA VERSIÓN 2.0.3 PUEDE SEGUIR PRESENTANDO PRESENTANDO PROBLEMAS Y QUIZÁ SEA NECESARIO QUE LA BORRES MANUALMENTE Y VUELVAS A INSTALARLA.  EL DÍA DE AYER (16/09/2022) SE LIBERÓ LA VERSIÓN 2.0.5 PERO NO NOS HA SIDO POSIBLE HACER PRUEBAS, QUIZÁ ESTO YA SE HAYA RESUELTO.
Puede instalarse con el método usual con el archivo JSON:  
[https://github.com/espressif/arduino-esp32/releases/download/2.0.3/package_esp32_dev_index.json](https://github.com/espressif/arduino-esp32/releases/download/2.0.3/package_esp32_dev_index.json)  
La página del release:
[https://github.com/espressif/arduino-esp32/releases/tag/2.0.3](https://github.com/espressif/arduino-esp32/releases/tag/2.0.3)
las primeras pruebas as hemos corrido usando la placa ESP32S3 Dev Module en el menú de Arduino IDE.  Puedes empexar con el ejemplo chip_id, que es de los más sencillos.
Por ser muy nueva la librería de Arduino, seguramente encontrarás varios bugs. El más notable para esta placa es que no puede reconocer los 16MB de Flash, sino sólo 4MB. Esto es un error conocido y está resuelto, sólo que hay que esperar a la liberación de la nueva versión.  Si eres usuario avanzado, al final de este documento te apuntamos al reporte en github y cómo solucionarlo. 

* Ejemplo Básico de sketch blink para Arduino IDE ESP32-S3:  
[Video Blink LED RGB en Arduino IDE](https://www.youtube.com/watch?v=5k669MCECUY&ab_channel=CosismoIoT)  
[Sketch Blink LED RGB en Arduino IDE](https://gist.github.com/cosismo/5c7ef47be6f8b82ce6f2192ec6813e6a)  
Las configuraciones relevantes de Arduino IDE sugeridas:
Board: ESP32S3 Dev Board
Flash Mode: DIO 80MHz
Flash Size: 16MB (128Mb)
PSRAM: QSPI PSRAM
Partition Scheme: 16MB Flash (3MB APP /9.9MB FATFS)
Conectar al puerto marcado como COM (NO al marcado como USB)

* La opción alternativa al Arduino IDE es usar el SDK proporcionado por el fabricante del chip, Espressif. Es el ESP-IDF, que se actualiza mucho más rápido que el Arduino IDE (que está basado en éste)  y también es más avanzado ya que tiene acceso a toda la API del chip. Puede requerir un mayor esfuerzo, por lo que sólo se recomienda para usuarios avanzados y profesionales.  La guía más básica para iniciar a programar el ESP32S3 con el IDF es la que sigue:  
[Get Started ESP32S3 ES-IDF](https://docs.espressif.com/projects/esp-idf/en/latest/esp32s3/get-started/index.html)
Si la sigues al pie de la letra, en menos de 30 minutos podrás correr el ejemplo "hello world" o el "blink".

* Si prefieres Python, MicroPython también soporta oficialmente el esp32s3. Puedes buscar información en su página oficial:  
[Micropython ESP32S3](https://micropython.org/download/GENERIC_S3/) 

* El foro oficial del fabricante (Espressif) incluye
[El post del avance en el soporte del IDF para el ESP32S3 ](https://www.esp32.com/viewtopic.php?t=21906)


* ESP32S3 Datasheet (chip)
[ESP32S3 Datasheet (Prerelease version 0.5) ](https://github.com/cosismo/esp32-s3/raw/gh-pages/esp32-s3_datasheet_en.pdf)

### Problemas conocidos:  





¡Suerte!  

   Equipo Cosismo




