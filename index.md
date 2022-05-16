### ESP32S3 Dev kit

Bienvenido al AIoT: Internet de las Cosas + Inteligencia Artificial

Si llegaste hasta aquí, sabrás que estás en la avanzada tecnológica de estos chips, por lo que la información actual es limitada, breve y cambiará todos los días.
A continuación te ofrecemos la información más básica hasta el momento. En la medida de lo posible la iremos actualizando.  También puedes ir a las fuentes directas que te ofrecemos a continuación.

Para comenzar a utilizar tu ESP32 y encontrar toda la información técnica, te recomendamos las siguientes ligas:

* Pinout   
![esp32s3 pinout](https://raw.githubusercontent.com/cosismo/esp32-s3/gh-pages/Nodemcu-esp-s3-12k-kit-pin-definition.png)

* Facebook.
[Grupo de Facebook en español sobre Internet de las Cosas](https://www.facebook.com/groups/724628401049648/)

* La guía más básica para iniciar a programar el ESP32S3 con el IDF es la que sigue:  
[Get Started ESP32S3](https://docs.espressif.com/projects/esp-idf/en/latest/esp32s3/get-started/index.html)

Si la sigues al pie de la letra, en menos de 30 minutos podrás correr el ejemplo "hello world" o el "blink".

* El foro oficial del fabricante (Espressif) incluye
[El post del avance en el soporte del IDF para el ESP32S3 ](https://www.esp32.com/viewtopic.php?t=21906)

* Para el soporte de Arduino,  ̶t̶e̶n̶d̶r̶á̶ ̶q̶u̶e̶ ̶c̶o̶n̶c̶l̶u̶í̶r̶s̶e̶ ̶e̶l̶ ̶p̶a̶s̶o̶ ̶a̶n̶t̶e̶r̶i̶o̶r̶ ̶(̶e̶l̶ ̶s̶o̶p̶o̶r̶t̶e̶ ̶e̶n̶ ̶e̶l̶ ̶I̶D̶F̶)̶ ̶y̶a̶ ̶q̶u̶e̶ ̶d̶e̶p̶e̶n̶d̶e̶ ̶d̶e̶ ̶a̶q̶u̶é̶l̶.̶
 En el repositorio del proyecto de Arduino ESP32 hay abierto un caso donde se ve el avance:  
[Caso en Github Arduino ESP32 sobre el avance del soporte al S3 para el ESP32S3 ](https://github.com/espressif/arduino-esp32/issues/5594)  

Actualización 4/04/2022: La versión de la librería Arduino-ESP32 que soportará ESP32S3 es la 2.03 y en este momento ya se ha liberado el RC1 de esta versión.
Puede instalarse con el método usaual con el archivo JSON:  
https://github.com/espressif/arduino-esp32/releases/download/2.0.3-RC1/package_esp32_dev_index.json  
La página del release:
[https://github.com/espressif/arduino-esp32/releases/tag/2.0.3-RC1](https://github.com/espressif/arduino-esp32/releases/tag/2.0.3-RC1)  
 ̶A̶c̶t̶u̶a̶l̶i̶z̶a̶c̶i̶ó̶n̶ ̶2̶4̶/̶0̶1̶/̶2̶0̶2̶2̶:̶ ̶h̶a̶y̶ ̶e̶n̶ ̶e̶s̶t̶e̶ ̶m̶o̶m̶e̶n̶t̶o̶ ̶u̶n̶a̶ ̶r̶a̶m̶a̶ ̶e̶n̶ ̶e̶l̶ ̶p̶r̶o̶y̶e̶c̶t̶o̶ ̶d̶e̶ ̶g̶i̶t̶h̶u̶b̶ ̶q̶u̶e̶ ̶y̶a̶ ̶d̶a̶ ̶s̶o̶p̶o̶r̶t̶e̶ ̶p̶a̶r̶c̶i̶a̶l̶ ̶y̶ ̶e̶l̶ ̶c̶a̶s̶o̶ ̶h̶a̶ ̶s̶i̶d̶o̶ ̶m̶a̶r̶c̶a̶d̶o̶ ̶c̶o̶m̶o̶ ̶"̶T̶e̶s̶t̶ ̶n̶e̶e̶d̶e̶d̶"̶.̶ ̶L̶o̶s̶ ̶d̶e̶s̶a̶r̶r̶o̶l̶l̶a̶d̶o̶r̶e̶s̶ ̶p̶r̶o̶m̶e̶t̶e̶n̶ ̶h̶a̶c̶e̶r̶ ̶e̶l̶ ̶m̶e̶r̶g̶e̶ ̶e̶n̶ ̶l̶o̶s̶ ̶p̶r̶ó̶x̶i̶m̶o̶s̶ ̶d̶í̶a̶s̶ ̶/̶s̶e̶m̶a̶n̶a̶s̶.̶ ̶
̶S̶i̶ ̶t̶i̶e̶n̶e̶s̶ ̶c̶o̶n̶o̶c̶i̶m̶i̶e̶n̶t̶o̶s̶ ̶d̶e̶ ̶c̶ó̶m̶o̶ ̶i̶n̶s̶t̶a̶l̶a̶r̶ ̶l̶a̶ ̶l̶i̶b̶r̶e̶r̶í̶a̶ ̶d̶e̶s̶d̶e̶ ̶o̶t̶r̶o̶ ̶b̶r̶a̶n̶c̶h̶,̶ ̶p̶u̶e̶d̶e̶s̶ ̶a̶y̶u̶d̶a̶r̶ ̶c̶o̶n̶ ̶l̶a̶s̶ ̶p̶r̶u̶e̶b̶a̶s̶.̶ ̶ ̶
̶É̶s̶t̶e̶ ̶e̶s̶ ̶e̶l̶ ̶b̶r̶a̶n̶c̶h̶:̶
̶[̶h̶t̶t̶p̶s̶:̶/̶/̶g̶i̶t̶h̶u̶b̶.̶c̶o̶m̶/̶e̶s̶p̶r̶e̶s̶s̶i̶f̶/̶a̶r̶d̶u̶i̶n̶o̶-̶e̶s̶p̶3̶2̶/̶t̶r̶e̶e̶/̶e̶s̶p̶3̶2̶-̶s̶3̶-̶s̶u̶p̶p̶o̶r̶t̶]̶(̶h̶t̶t̶p̶s̶:̶/̶/̶g̶i̶t̶h̶u̶b̶.̶c̶o̶m̶/̶e̶s̶p̶r̶e̶s̶s̶i̶f̶/̶a̶r̶d̶u̶i̶n̶o̶-̶e̶s̶p̶3̶2̶/̶t̶r̶e̶e̶/̶e̶s̶p̶3̶2̶-̶s̶3̶-̶s̶u̶p̶p̶o̶r̶t̶)̶ ̶ ̶
El tracking de los avances:  
[https://github.com/espressif/arduino-esp32/discussions/6197](https://github.com/espressif/arduino-esp32/discussions/6197)  
La discusión:  
[https://github.com/espressif/arduino-esp32/issues/5594](https://github.com/espressif/arduino-esp32/issues/5594)  

* ESP32S3 Datasheet 
[ESP32S3 Datasheet (Prerelease version 0.5) ](https://github.com/cosismo/esp32-s3/raw/gh-pages/esp32-s3_datasheet_en.pdf)

¡Suerte!
   Equipo Cosismo




