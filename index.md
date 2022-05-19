### ESP32S3 Dev kit

### Última Actualización: 19/mayo/2022

Bienvenido al AIoT: Internet de las Cosas + Inteligencia Artificial

Si llegaste hasta aquí, sabrás que estás en la avanzada tecnológica de estos chips, por lo que la información actual es limitada, breve y cambiará con frecuencia. Te recomendamos revisarla constantemente.
A continuación te ofrecemos la información más básica hasta el momento. En la medida de lo posible la iremos actualizando.  También puedes ir a las fuentes directas que te ofrecemos a continuación.

Para comenzar a utilizar tu ESP32 y encontrar toda la información técnica, te recomendamos las siguientes ligas:

* Pinout   
![esp32s3 pinout](https://raw.githubusercontent.com/cosismo/esp32-s3/gh-pages/Nodemcu-esp-s3-12k-kit-pin-definition.png)
![esp32s3 pinout](https://raw.githubusercontent.com/cosismo/esp32-s3/gh-pages/Nodemcu-esp-s3-12k-kit-pin-definition-01.png)


* Facebook.
[Grupo de Facebook en español sobre Internet de las Cosas](https://www.facebook.com/groups/724628401049648/)

* Actualización 4/04/2022:  La última versión de la librería (2.0.3) Arduino-ESP32 ya tiene soporte para ESP32-S3 
Puede instalarse con el método usual con el archivo JSON:  
[https://github.com/espressif/arduino-esp32/releases/download/2.0.3/package_esp32_dev_index.json](https://github.com/espressif/arduino-esp32/releases/download/2.0.3/package_esp32_dev_index.json)  
La página del release:
[https://github.com/espressif/arduino-esp32/releases/tag/2.0.3](https://github.com/espressif/arduino-esp32/releases/tag/2.0.3)
las primeras pruebas as hemos corrido usando la placa ESP32S3 Dev Module en el menú de Arduino IDE.  Puedes empexar con el ejemplo chip_id, que es de los más sencillos.
Por ser muy nueva la librería de Arduino, seguramente encontrarás varios bugs. El más notable para esta placa es que no puede reconocer los 8MB de Flash, sino sólo 4MB. Esto es un error conocido y está resuelto, sólo que hay que esperar a la liberación de la nueva versión.  Si eres usuario avanzado, al final de este documento te apuntamos al reporte en github y cómo solucionarlo. 

* La opción alternativa al Arduino IDE es usar el SDK proporcionado por el fabricante del chip, Espressif. Es el ESP-IDF, que se actualiza mucho más rápido que el Arduino IDE (que está basado en éste)  y también es más avanzado ya que tiene acceso a toda la API del chip. Puede requerir un mayor esfuerzo, por lo que sólo se recomienda para usuarios avanzados y profesionales.  La guía más básica para iniciar a programar el ESP32S3 con el IDF es la que sigue:  
[Get Started ESP32S3 ES-IDF](https://docs.espressif.com/projects/esp-idf/en/latest/esp32s3/get-started/index.html)
Si la sigues al pie de la letra, en menos de 30 minutos podrás correr el ejemplo "hello world" o el "blink".

* Si prefieres Python, MicroPython también soporta oficialmente el esp32s3. Puedes buscar información en su página oficial:  
[Micropython ESP32S3](https://micropython.org/download/GENERIC_S3/) 

* El foro oficial del fabricante (Espressif) incluye
[El post del avance en el soporte del IDF para el ESP32S3 ](https://www.esp32.com/viewtopic.php?t=21906)

* ESP32S3 Diagrama Esquemático (Dev Kit)
[Nodemcu-esp-s3-12k-kit Schematic](https://github.com/cosismo/esp32-s3/raw/gh-pages/Nodemcu-esp-s3-12k-kit_schematic.pdf)

* ESP32S3 Drivers USB CH340 (Dev Kit) 
El chip USB a ttl de esta placa es muy común y muy probablemente tu máquina Windows, Mac o Linux lo detectará automáticamente. Si tienes problemas te recomendamos que revises esta página:  
[Drivers CH340](https://cosismo.github.io/usbttl-ch340/)


* ESP32S3 Datasheet (chip)
[ESP32S3 Datasheet (Prerelease version 0.5) ](https://github.com/cosismo/esp32-s3/raw/gh-pages/esp32-s3_datasheet_en.pdf)

### Problemas conocidos:  

* Arduino IDE no reconoce 8MB de flash de esta placa. Si se cambia la partición a 8MB entra en loop de reiniciarse. Esto no es un problema ni con la placa ni propiamente con la librería de Arduino, sino con la utilería para subir el archivo esptool. Fue detectada y resuelta por los desarrolladores pero aún no está actualizada en la libreríade Arduino noi en el ESP-IDF. Puedes encontrar el workaround con el patch en el Issue en github:
https://github.com/espressif/arduino-esp32/issues/6453  



¡Suerte!  

   Equipo Cosismo




