# homeassistant-config
This should be my 'mostly' up to date Home Assistant config

I will try to update on a regular basis but as more and more config moves to integrations and are setup/configured
via the GUI I will be relying on backups for recovery rather than GitHub

I have tried to remove sensitive add-on/integrations/config for obvious reasons but please let me know if you find anything ;)

Hope it helps and if you have any questions, drop me an email, message on GitHub or post an issue and will try to reply

Matthew

# HA Hardware
- HASSIO  
  Raspberry Pi 4B+ 8GB + USB SSD (Wired + WiFi) <br />
  https://github.com/home-assistant/operating-system/releases <br />
- RFLink 433 <br />
  Arduino Mega based RFlink PCB with 433 MHz Transceiver <br />
  https://www.nodo-shop.nl/en/ <br />
  f/w http://www.rflink.nl/ <br />
- Zigbee <br />
  Texas Instruments LAUNCHXL-CC1352P-2 <br />
  f/w https://www.zigbee2mqtt.io/information/flashing_via_uniflash.html <br />
- Z-Wave <br />
  Aeotec Z-Stick <br />
  *decommissioned* <br />

# Add-Ons
- Appdaemon - https://github.com/hassio-addons/addon-appdaemon <br />
    hadashboard - https://appdaemon.readthedocs.io/en/latest/DASHBOARD_INSTALL.html <br />
    hassapps-schedy - https://hass-apps.readthedocs.io/en/stable/apps/schedy/index.html <br />
    octoblock - https://github.com/badguy99/octoblock <br />
- ESPHome - https://esphome.io/ <br />
- Grafana <br />
- Home Assistant Google Drive Backup - https://github.com/sabeechen/hassio-google-drive-backup <br />
- InfluxDB <br />
- Mosquitto broker <br />
- SSH & Web Terminal <br />
- zigbee2mqtt - https://www.zigbee2mqtt.io/ <br />

# Integrations
- Apple TV <br />
- BlueIris <br />
- Cloudflare <br />
- ESPHome <br />
- Garbage Collection <br />
- HASS Bridge <br />
- HACS (Home Assistant Community Store) <br />
    see HACS subtopic <br />
- iOS <br />
- Konnected.io <br />
- Life360 <br />
- Mobile App <br />
- Mosquitto broker <br />
- SONOS <br />
- Tasmota <br />
- Tuya <br />
- Waze Travel Time <br />
- WLED <br />

# HACS
- Integrations <br />
    BlueIris NVR <br />
    Config Check  <br />
    Solcast <br />
    Remote Home-Assistant <br />
    AstroWeather <br />
    Octopus Agile <br />
    Camera combined <br />
    Breaking Changes <br />
    Anniversaries <br />
    Garbage Collection <br />
- Frontend <br />
    Garbage Collection Card <br />
    power-distribution-card <br />
    surveillance-card <br />
    Multiple Entity Row <br />
    Canary <br />
    Kiosk Mode <br />
    Fan Control Entity Row <br />
- Automation <br />
    Octoblock <br />
    Auto 'Fan Speed' Controller <br />

# Devices
## WiFi
  - WLED LED
    - QuineLED
  - VIGICA - Two Socket + USB WiFi wall Socket
    f/w https://esphome.io/
## RF
- Light Wave RF
  - Light Switches
  - Wall Sockets
## Zigbee
- IKEA
  - LEPTITER Recessed spot light, dimmable, white spectrum (T1820)
- Lidl
  - Livarno Lux E14 candle CCT (HG06492B)
  - Livarno Lux E14 candle RGB (HG06106B)
  - Livarno Lux GU10 spot RGB (HG06106A)
  - Lidl GU10


# Wall Sockets
- WiFi

# Sensors, Switch & Buttons
- IKEA
  - TRADFRI remote control (E1524/E1810)
  - TRADFRI motion sensor (E1525/E1745)
- Xiaomi
 - Aqara temperature, humidity and pressure sensor (WSDCGQ11LM)
 - Aqara door & window contact sensor (MCCGQ11LM)
 - Aqara wireless switch (WXKG11LM)

# HVAC
- Storage Heaters
  - SonoffTH16
  - f/w https://esphome.io/
- Underfloor Heating
  - BHT-1000 GBW
  - f/w https://github.com/fashberg/WThermostatBeca
- Blinds
  - Generic RF Blinds

# Waterheaters
- SonoffPOWR2

# Solar Installation
## Solax Inverters
- X1-Hybrid SKU-SU5000E 5.Kw
  - Evolution Ultramax Solar Panels (285w)
  - PylonTech US3000
- X1-Hybrid SKU-SU5000E 5Kw
  - LG Chem EM048063P3Sx
- X1-Air-Mini 2.5Kw
  - decommissioned

## Solar Panel Optimization (No HA integration)
- TIGO CCA
- TIGO TS4-R-0

# Energy Monitoring
## Solar
- SolaxPortal - https://www.solax-portal.com/
- TIGO Energy - https://www.tigoenergy.com/
## Whole Home
- IAMMETER - WEM3080 - https://www.iammeter.com
- Light Wave Energy Monitor
  - decommissioned

# Customization and setup
I separate my config into individual yaml files or use packages

## /root
Nothing special in here, stock standard HA files and individual yaml files based on my configuration.yaml

## /packages
This is where most of my custom setup lives
