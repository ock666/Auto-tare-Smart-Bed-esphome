# smart-bed
an ESPHome yaml config for a bed presence sensor, with auto taring functionality.

Simply replace the relevant settings for wireless, Home Assistant api password, and pin-out configurations for your set-up; then, upload the yaml to the ESP as you usually would with:

esphome run smart-bed.yaml

The config comes with auto-taring functionality, which avoids having to record super accurate zeroing values and also can prevent false positives when you have laundry or other items on your bed.

Great to set-up any bed presence automations within Home Assistant.

Hardware required:

4x Load cells
1x hx711 board
1x esp8266 board
