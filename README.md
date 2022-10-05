# ESPHome Smart Bed

---

This repo contains the necessary code to create the ESPHome Smart Bed. A DIY Project to allow one to create automations based around presence in a bed or couch. 

## Features

- **Auto Tare Functionality** - Automagically tare the bed for any slight adjustments in detected weight, i.e when laundry is placed upon the bed.

- **Manual Tare** - Should you find the bed is incorrectly detecting your presence a manual tare is available to re-tare. This functionality can also be attached to automations which occur when you leave the house. This way you'll always arrive home to a perfectly tared bed.

- **Wifi Signal Strength Detection** - Some metal bedframes can interfere with WiFi signals, This sensor will make sure you set your bed up with sufficient signal strength.


## Hardware

- 1x Wemos D1 Mini or Nodemcuv2
- 1x HX-711 Load cell amplifier board
- 4x Load cells

## Set-up and Installation

1. Replace the settings within the YAML file to fit your configuration. Such as Static IP, Wifi & AP Credentials, OTA & API credentials etc.
2. Connect the Load cells to the hx711, and the hx711 to your chosen ESP board.
![90f2ef0e694b1960b894ac10e2ee480a90cd5a51](https://user-images.githubusercontent.com/73627199/168532855-7570b209-4d54-4761-905e-d9277892f048.png)

**PROTIP:** If you are using a nodemcuv2 you'll have to use 3.3v instead of 5v as shown in the diagram above for the D1 Mini. It **should** work just fine.

3. Connect your d1 mini/nodemcu to your computer and flash the device with your chosen method. I tend to prefer:

`esphome run smart-bed.yaml`

4. Add the device in Home Assistant and start automating!

## Things to know

- **Placement** - Load cells can either be placed under the legs of the bed, or between the slats and the mattress. The latter is easier to set up, but the former tends to be more reliable. I use the slats method for my device and is quite reliable with auto taring enabled.
- **Slats/Mattress Approach** - If you decide this is the path you will take I suggest manually taring the bed upon leaving home. In my personal experience the bed will detect you 99.9% of the time with this approach.

## Donate

If you found this project helpful feel free to send me a donation. If not, Thats cool too! :)

Bitcoin: 3JkyRbkmrF54jEizYgLRkBxMFek32GPhyh

Litecoin: LbqF41gdLjbunGLrvZf3RbPAWyfeQk3LEw

Monero: 45BWhTURjsK1918dnTTZK5DRkLdzEZndPT7p6B9qyRTnGVMhg5zcYwGEiymctGumwGdhySFpCAwSEUSBEXxUGeWyMjvT4TZ

Ethereum: 0x08fB95EbE017A0AeD3430853F5AE924Caa4F8b9a
