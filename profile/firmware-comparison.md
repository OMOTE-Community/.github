## Firmware
There are currently two firmwares available for OMOTE. They are completely independent from each other, and they have no common base. You can choose which one to use.

 &nbsp;| OMOTE-Firmware| OMOTE-Firmware-object-oriented
------------ | ------------- | -------------
summary | - more end user features<br>- mainly pure C, probably easier to understand<br>- extensive Wiki explaining the software | - less end user features<br>- pure C++, probably higher complexity<br>- currently no Wiki
simulator for running the<br>firmware on a PC|- Linux, Windows, macOS<br>- MQTT<br>- keypad simulator<br>[Wiki](https://github.com/OMOTE-Community/OMOTE-Firmware/wiki/Software-simulator-for-fast-creating-and-testing-of-LVGL-GUIs) | - Linux, Windows<br>- WebSockets<br>- MQTT (soon)
infrared sender | - some predefined IR devices and 20 IR protocols<br>- more IR protocols can be added easily<br>[Wiki](https://github.com/OMOTE-Community/OMOTE-Firmware/wiki/How-to-understand-and-modify-the-firmware#supported-devices) | supported
infrared receiver, see which IR<br>codes is your old remote sending | &#10003; | &#10003;
BLE keyboard<br>GUI to manage bonds <br>e.g. for Amazon Fire TV, Nvidia Shield, and others | &#10003; [Wiki](https://github.com/OMOTE-Community/OMOTE-Firmware/wiki/How-to-understand-and-modify-the-firmware#pairing-ble-devices)| &#10005;
MQTT | - sending<br>- [receiving](https://github.com/OMOTE-Community/OMOTE-Firmware/wiki/How-to-understand-and-modify-the-firmware#subscribe-to-mqtt-topics) | - sending <br> - receiving (in future)
support of [MQTT keyboard](https://github.com/OMOTE-Community/esp32-mqtt-keyboard) (control a hardware keyboard simulator connected to your media device) | &#10003; | &#10005;
WebSockets | &#10005; | &#10003;
Home Assistant WebSocket API framework | &#10005; | &#10003;
scenes | &#10003; [Wiki](https://github.com/OMOTE-Community/OMOTE-Firmware/wiki/How-to-understand-and-modify-the-firmware#scenes) | &#10005;
scene specific commands for keypad | &#10003; [Wiki](https://github.com/OMOTE-Community/OMOTE-Firmware/wiki/How-to-understand-and-modify-the-firmware#hardware-keys) | handling key presses in a priority manner available (for an upcoming scene implementation)
scene specific GUIs<br>dynamic creation of GUIs (not one single list of GUIs from left to right) | &#10003; [Wiki](https://github.com/OMOTE-Community/OMOTE-Firmware/wiki/How-to-understand-and-modify-the-firmware#scene-specific-guis) | &#10005;
command pattern (can be used by keypad and GUI) | &#10003; [Wiki](https://github.com/OMOTE-Community/OMOTE-Firmware/wiki/How-to-understand-and-modify-the-firmware#commands) | &#10005;
support of short press, repeated press<br>and long press of keypad | &#10003; [Wiki](https://github.com/OMOTE-Community/OMOTE-Firmware/wiki/How-to-understand-and-modify-the-firmware#hardware-keys) | &#10005;
special firmware for checking hardware | &#10003; [Wiki](https://github.com/OMOTE-Community/OMOTE-Firmware/wiki/How-to-understand-and-modify-the-firmware#which-is-the-right-firmware-to-compile)| &#10005;
lvgl version | - 8.4<br>- 9.x (optional, more [memory](https://github.com/OMOTE-Community/OMOTE-Firmware/wiki/How-to-understand-and-modify-the-firmware#memory) needed) | - 9.2<br>&nbsp;
Littlefs filesystem | &#10005; | support of storage of json config in flash
supported OMOTE hardware | up to rev5 | up to rev4 (rev5 soon)
