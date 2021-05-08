# homeassistant-config
This is my hopefully current Home Assistant config

I will try to update on a regular basis but as more and more config moves to integrations and are setup/configured
via the GUI I will be relying on backups for recovery rather than GitHub

I have tried to remove sensitive add-on/integrations/config for obvious reasons but please let me know if you find anything ;)

Hope it helps and if you have any questions, drop me an email, message on GitHub or post an issue and will try to reply

Matthew

# HA Hardware
    HASSIO:
    Raspberry Pi 4B+ 8GB + USB SSD (Wired + WiFi)
      https://github.com/home-assistant/operating-system/releases

    RF 433:
    RFLink
      https://www.nodo-shop.nl/en/
      f/w http://www.rflink.nl/

    Zigbee:
    Texas Instruments LAUNCHXL-CC1352P-2
      https://www.zigbee2mqtt.io/information/flashing_via_uniflash.html

# Add-Ons:
    Appdaemon - https://github.com/hassio-addons/addon-appdaemon
      - hadashboard - https://appdaemon.readthedocs.io/en/latest/DASHBOARD_INSTALL.html
      - hassapps-schedy - https://hass-apps.readthedocs.io/en/stable/apps/schedy/index.html
      - octoblock - https://github.com/badguy99/octoblock
    ESPHome - https://esphome.io/
    Grafana
    Home Assistant Google Drive Backup - https://github.com/sabeechen/hassio-google-drive-backup
    InfluxDB
    Mosquitto broker
    SSH & Web Terminal
    zigbee2mqtt - https://www.zigbee2mqtt.io/

# Integrations
    Apple TV
    BlueIris
    Cloudflare
    ESPHome
    Garbage Collection
    HASS Bridge
    HACS (Home Assistant Community Store)
    iOS
    Konnected.io
    Life360
    Mobile App
    Mosquitto broker
    SONOS
    Tasmota
    Tuya
    Waze Travel Time
    WLED

# HACS (Home Assistant Community Store)
    Integrations
    - BlueIris NVR
    - Config Check
    - Solcast
    - Remote Home-Assistant
    - AstroWeather
    - Octopus Agile
    - Camera combined
    - Breaking Changes
    - Anniversaries
    - Garbage Collection
    Frontend
    - Garbage Collection Card
    - power-distribution-card
    - surveillance-card
    - Multiple Entity Row
    - Canary
    - Kiosk Mode
    - Fan Control Entity Row
    Automation
    - Octoblock
    - Auto 'Fan Speed' Controller

# Lights
    Light Wave RF
    Zigbee
      - Lidl GU10
      -
    WLED
      - QuineLED

# Wall Sockets:
    Light Wave RF

# HVAC
    Thermostats:
      - Xiaomi Aqara Zigbee
    Storage Heaters:
      - SonoffTH16
        f/w https://esphome.io/
    Underfloor Heating:
      - BHT-1000 GBW
        f/w https://github.com/fashberg/WThermostatBeca
    Blinds:
      - Generic RF Blinds

# Waterheaters
    SonoffPOWR2

# Solar
    Solax X1-Hybrid SKU-SU5000E Inverter
      - Evolution Ultramax Solar Panels (285w)
      - PylonTech US3000
    Solax X1-Hybrid SKU-SU5000E Inverter
      - LG Chem
    Solar Panel Optimization (No HA integration)
      - TIGO CCA
      - TIGO TS4-R-0

# Energy Monitoring
    Solar:
      - SolaxPortal - https://www.solax-portal.com/
      - TIGO Energy - https://www.tigoenergy.com/
    Whole Home:
      - IAMMETER - WEM3080 - https://www.iammeter.com

Now for my customization and setup. I separate my config into individual yaml files or use packages
# /root
Nothing special in here, stock standard HA files and individual yaml files based on my configuration.yaml
 
