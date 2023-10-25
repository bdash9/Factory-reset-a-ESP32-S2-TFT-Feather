# Factory-reset-a-ESP32-S2-TFT-Feather

What should you do if your Adafruit ESP32-S2 tft Feather is locked up.

Hold BOOT while pressing reset. It doesn't show as a drive but as a serial port. You can try installing an Arduino program; that way should reinstall the bootloader too. This probably wont work.
On a MAC it might show the drive mounted.


https://adafruit.github.io/Adafruit_WebSerial_ESPTool/


See this guide:
https://learn.adafruit.com/adafruit-esp ... rduino-ide

You can also reinstall the UF2 bootloader:
https://learn.adafruit.com/adafruit-esp ... bootloader


*** If the ESP32 is able to connect then use this tool ***

https://adafruit.github.io/Adafruit_WebSerial_ESPTool/
 
Hit Erase first.

Then hit boot and reset. Reconnect.

Then click program
Then click choose a file
Select **combined.bin **
https://learn.adafruit.com/adafruit-magtag/install-uf2-bootloader


Wait for it to upload…green bar…

Hit reset when done

Uploaded a uf2 factory reset from Adafruit…
https://learn.adafruit.com/adafruit-esp32-s2-tft-feather/factory-reset

**adafruit-esp32-s2-tft-feather-factory-reset.UF2**

_____________________________________________________________
Used this elsewhere and figured it could be useful...
# esptool.py --chip esp32 --port /dev/ttyUSB0 erase_flash

