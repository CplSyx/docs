### Version 7.2.0 Constance

- Change Exception reporting removing exception details from ``Status 1`` and consolidated in ``Status 12`` if available
- Change HTTP CORS from command ``SetOption73 0/1`` to ``Cors <cors_domain>`` allowing user control of specific CORS domain by Shantur Rathore (#7066)
- Change GUI Shutter button text to Up and Down Arrows based on PR by Xavier Muller (#7166)
- Change amount of supported DHT sensors from 3 to 4 by Xavier Muller (#7167)
- Change some Settings locations freeing up space for future single char allowing variable length text
- Change tasmota-basic.bin and FIRMWARE_BASIC to tasmota-lite.bin and FIRMWARE_LITE
- Fix flashing H801 led at boot by Stefan Hadinger (#7165, #649)
- Fix duplicated ``Backlog`` when using Event inside a Backlog by Adrian Scillato (#7178, #7147)
- Fix Gui Timer when using a negative zero offset of -00:00 by Peter Ooms (#7174)
- Fix DeepSleep in case there is no wifi by Stefan Bode (#7213)
- Fix Fade would ignore ``savedata 0`` and store to flash anyways (#7262)
- Fix Arduino IDE compile error (#7277)
- Fix no AP on initial install (#7282)
- Add command ``SerialConfig 0..23`` or ``SerialConfig 8N1`` to select Serial Config based in PR by Luis Teixeira (#7108)
- Add command ``Sensor34 9 <weight code>`` to set minimum delta to trigger JSON message by @tobox (#7188)
- Add rule var ``%topic%`` by Adrian Scillato (#5522)
- Add rule triggers ``tele-wifi1#xxx`` by Adrian Scillato (#7093)
- Add SML bus decoder syntax support for byte order by Gerhard Mutz (#7112)
- Add experimental support for stepper motor shutter control by Stefan Bode
- Add optional USE_MQTT_TLS to tasmota-minimal.bin by Bohdan Kmit (#7115)
- Add save call stack in RTC memory in case of crash, command ``Status 12`` to dump the stack by Stefan Hadinger
- Add Home Assistant force update by Frederico Leoni (#7140, #7074)
- Add Wifi Signal Strength in dBm in addition to RSSI Wifi Experience by Andreas Schultz (#7145)
- Add Yaw, Pitch and Roll support for MPU6050 by Philip Barclay (#7058)
- Add reporting of raw weight to JSON from HX711 to overcome auto-tare functionality by @tobox (#7171)
- Add Zigbee support for Xiaomi Aqara Vibration Sensor and Presence Sensor by Stefan Hadinger
- Add Shutter functions ramp up/down and MQTT reporting by Stefan Bode
- Add fallback support from version 8.x
- Add restriction if fallback firmware is incompatible with settings resulting in unreachable device
- Add support for DHT12 Temperature and Humidity sensor by Stefan Oskamp
