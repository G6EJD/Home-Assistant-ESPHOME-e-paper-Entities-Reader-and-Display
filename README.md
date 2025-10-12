# Home-Assistant-ESPHOME-e-paper-Entities-Reader-and-Display
Using ESPHOME to read HA Entity values, then display the values on an e-paper display, in this example the 1.54" unit, but there is an example for 7.5"V2 display too.

How to install the yaml code, based on either a WaveShare e-paper driver or XIAO or any other ESP32 connected to an e-paper display:

Waveshare e-paper driver: https://www.waveshare.com/wiki/E-Paper_ESP32_Driver_Board

XIAO (Seeed) e-paper driver board: https://wiki.seeedstudio.com/xiao_esp32s3_getting_started/
AND the extra added on: https://wiki.seeedstudio.com/xiao_eink_expansion_board_v2/
Solder the pins to the xiao board, then insert into the e-paper carrier board (the right way around!).
Open the black clip on the display socket.Plug your display into the board, then close the black clip down.

1. Install ESPHOME on your Home AssistantInstall as a Home Assistant Add-On:
    In Home Assistant, go to Settings > Add-ons > Add-on Store.
    Search for "ESPHome" and click Install.
    Start the ESPHome add-on and access its web interface.
2. Create a new DEVICE (bottom right), then NEXT, then NEW DEVICE SETUP, give it a name say "SENSOR_READER'
3. Choose the device if Waveshare then an ESP32 or if XIAO then ESP32S3
4. Choose SKIP
5. Now either create a SECRET file and enter your WiFi credentials in there, or enter your detials in the WiFi section:
      ssid: yourSSID
      password: your password
6. Now view the yaml file in this repository for your chosen display, in this eample it is the 1.54" display, then copy the conecnts from PORTAL to the bottom and paste in your file.
7. Now upload to your board, usually via a manual install.
8. Choose INSTALL (top right), choose MANUALLY, wait for the code to compile, then save the resultant file, NEW FORMAT option.
9. NOW, choose INSTALL again, and the PLUGGED INTO THIS COMPUTER option.
10. Select the web inteface, then select your device USB port, now follow the instructions to select your firmware file, then install.
11. That's it...
