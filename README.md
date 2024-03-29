# homeassistant-config
This should be my 'mostly' up to date Home Assistant config

I will try to update on a regular basis but as more and more config moves to integrations and are setup/configured
via the GUI I will be relying on backups for recovery rather than GitHub

I have tried to remove sensitive add-on/integrations/config for obvious reasons but please let me know if you find anything ;)

Hope it helps and if you have any questions, drop me an email, message on GitHub or post an issue and will try to reply

Matthew

# HA Hardware
- HASSIO  
  Raspberry Pi 4B+ 8GB + USB SSD (Wired + WiFi)  
  https://github.com/home-assistant/operating-system/releases
- RFLink 433  
  Arduino Mega based RFlink PCB with 433 MHz Transceiver  
  https://www.nodo-shop.nl/en/  
  f/w http://www.rflink.nl/
- Zigbee  
  Texas Instruments LAUNCHXL-CC1352P-2  
  f/w https://www.zigbee2mqtt.io/information/flashing_via_uniflash.html
- Z-Wave  
  Aeotec Z-Stick - *decommissioned*

# Add-Ons
- Appdaemon - https://github.com/hassio-addons/addon-appdaemon
  - hadashboard - https://appdaemon.readthedocs.io/en/latest/DASHBOARD_INSTALL.html
  - hassapps-schedy - https://hass-apps.readthedocs.io/en/stable/apps/schedy/index.html
  - octoblock - https://github.com/badguy99/octoblock
- ESPHome - https://esphome.io/
- Grafana
- Home Assistant Google Drive Backup - https://github.com/sabeechen/hassio-google-drive-backup
- InfluxDB
- Mosquitto broker
- SSH & Web Terminal
- zigbee2mqtt - https://www.zigbee2mqtt.io/

# Integrations
- Apple TV
- BlueIris
- Cloudflare
- ESPHome
- Garbage Collection
- HASS Bridge
- HACS (Home Assistant Community Store)
  - see HACS subtopic
- iOS
- Konnected.io
- Life360
- Mobile App
- Mosquitto broker
- SONOS
- Tasmota
- Tuya
- Waze Travel Time
- WLED

# HACS
- Integrations
  - Anniversaries
  - AstroWeather
  - BlueIris NVR
  - Breaking Changes
  - Camera combined
  - Config Check
  - Garbage Collection
  - Octopus Agile
  - Remote Home-Assistant
  - Solcast
- Frontend
  - Canary
  - Fan Control Entity Row
  - Garbage Collection Card
  - Kiosk Mode
  - Multiple Entity Row
  - power-distribution-card
  - surveillance-card
- Automation
  - Auto 'Fan Speed' Controller
  - Octoblock

# Devices
## WiFi
- WLED / QuinLED  
  f/w https://github.com/Aircoookie/WLED & https://quinled.info/
- VIGICA - Two Socket + USB WiFi wall Socket  
  f/w https://esphome.io/
- SonoffDUAL  
  f/w https://esphome.io/
- SonoffTH16  
  f/w https://esphome.io/
- SonoffPOW & POWR2  
  f/w https://esphome.io/
- SonoffTH16  
  f/w https://esphome.io/
- SonoffMINI  
  f/w https://esphome.io/
- Sonofd iFan01  
  f/w https://esphome.io/
- Sonofd iFan01  
  f/w https://tasmota.github.io/docs/
- BHT-1000 GBW  
  f/w https://github.com/fashberg/WThermostatBeca  
- Smart Life WIFI Inline Switch  
  f/w Tuya Based
- Smart Plugs *On/Off & Power Monitor*  
  f/w https://esphome.io/
- Konnected Alarm Panel  
  f/w https://konnected.io
- SONOS Audio System
## RF
- Light Wave RF  
  - Light Switches
  - Wall Sockets
- Generic RF Blinds

## Zigbee
- IKEA
  - LEPTITER Recessed spot light, dimmable, white spectrum (T1820)
  - TRADFRI remote control (E1524/E1810)
  - TRADFRI motion sensor (E1525/E1745)
- Lidl
  - Livarno Lux E14 candle CCT (HG06492B)
  - Livarno Lux E14 candle RGB (HG06106B)
  - Livarno Lux GU10 spot RGB (HG06106A)
  - Lidl GU10
- Xiaomi
 - Aqara temperature, humidity and pressure sensor (WSDCGQ11LM)
 - Aqara door & window contact sensor (MCCGQ11LM)
 - Aqara wireless switch (WXKG11LM)

## Other
- Logitech
  - Harmony Elite

# Solar Installation
## Solax Inverters
- X1-Hybrid SKU-SU5000E *(5Kw)*  
  Evolution Ultramax Solar Panels *(285w)*  
  PylonTech - US3000  
- X1-Hybrid SKU-SU5000E *(5Kw)*  
  LG Chem - EM048063P3Sx  
- X1-Air-Mini 2.5Kw - *decommissioned*

## Solar Panel Optimization *(No HA integration)*
- TIGO CCA
- TIGO TS4-R-0

# Energy Monitoring
## Solar
- SolaxPortal - https://www.solax-portal.com/
- TIGO Energy - https://www.tigoenergy.com/
## Whole Home
- IAMMETER  
  WEM3080 - https://www.iammeter.com
- Light Wave Energy Monitor - *decommissioned*

# Customization and setup
I mostly separate my config into individual yaml files or use packages

## /root
Nothing special in here, stock standard HA files and individual yaml files based on my configuration.yaml

## /packages
This is where most of my custom setup lives
