# Adafruit Data Logger PlatformIO
----
## Description

> This project uses platform io IDE to display humidity and temperature on an OLED display and send it to io.adafruit.com.

## External Libraries

### Adafruit_GFX
by Adafruit to manage the displaying items on the OLED, So thanks to Adafruit. To install Adafruit_GFX from PIO (PlatformIO) home choose libraries and type Adafruit_GFX in search textbox, when apper click install.

### Adafruit_SSD1306
by Adafruit to use the OLED in arduino IDE, thanks again to Adafruit. To install Adafruit_SSD1306 from PIO (PlatformIO) home choose libraries and type Adafruit_SSD1306 in search textbox, when apper click install.

### ArduinoJson
We are using andruino json library by Benoît Blanchon to create and read the configration file in the SPIFFS, Benoît Blanchon thank you. To install ArduinoJson from PIO (PlatformIO) home choose libraries and type ArduinoJson in search textbox, when apper click install.

### Adafruit_MQTT_Library﻿

 Last external library we use in this project is the adafruit MQTT library by Adafruit, big thanks to Adafruit. To Install the adafruit MQTT library for from PIO (PlatformIO) home choose libraries and type adafruit MQTT  in search textbox, when apper click install.
 
## How It Works

The ESP8266 reads the temperature and the humidity through the DHT11 sensor. It connects to the Adafruit IO website through WiFi and sends the sensor readings to the feeds through MQTT. We have setup a Webserver on the ESP8266 to configure the Adafruit IO logging parameters:

   1. Start/Stop sending the data.
   2. The frequency of sending.
   3. Adafruit IO API key.
   
All this is done through the “control settings” HTML page that’s hosted in ESP8266 web server.

----
## Thanks
