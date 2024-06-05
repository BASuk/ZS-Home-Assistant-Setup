Welcome to my Home Assistant setup git.

I am using this to save and share various aspects of my journey to build a useful local smart home. My hope is I can help save people time and money!

Please note that all Amazon links are affiliate links. You may be able to find the products cheaper elsewhere (such as aliexpress).

# My Computers (inc pi's)
## My PC
OS: Windows 11 Pro

CPU: AMD Ryzen R5 2700

RAM: 16GB

GPU: MSI Radeon RX 6650 XT 8GB

Mobo: 

## My family's PC (customised to be a server before turning into a PC)
OS: Windows 11 Pro

CPU: Intel Core i5-7600

## <a target="_blank" href="https://www.amazon.co.uk/gp/search?ie=UTF8&tag=basuk036-21&linkCode=ur2&linkId=f79f0e265b3f2fc0fb89815b1592f991&camp=1634&creative=6738&index=computers&keywords=Raspberry Pi 5 (8gb)">Raspberry Pi 5 (8gb)</a>

OS: Home Assistant OS

Accessories: <a target="_blank" href="https://www.amazon.co.uk/gp/search?ie=UTF8&tag=basuk036-21&linkCode=ur2&linkId=57c09ac598653ce026ce5011a4e2da4d&camp=1634&creative=6738&index=computers&keywords=SONOFF Universal Zigbee 3.0 USB Dongle Plus Gateway with Antenna for Home Assistant, IoBroker, Zigbee2MQTT">SONOFF USB Zigbee dongle</a>

## <a target="_blank" href="https://www.amazon.co.uk/gp/search?ie=UTF8&tag=basuk036-21&linkCode=ur2&linkId=bae574f2b1d26e1c4dc864b7b4f18a73&camp=1634&creative=6738&index=computers&keywords=Raspberry Pi 4 (8gb)">Raspberry Pi 4 (8gb)</a>
OS: 
Purpose: Frigate (in docker container)
Accessories: <a target="_blank" href="https://amzn.to/3RcWwe7">Google Coral TPU USB</a>

## Raspberry Pi 3b
### NetAlertX
https://github.com/jokob-sk/NetAlertX

## Raspberry Pi 3b
### Octoprint

## Network
### Current kit
EE(UK) 900mb fibre 

Google Nest WiFi with extender

<a target="_blank" href="https://www.amazon.co.uk/gp/search?ie=UTF8&tag=basuk036-21&linkCode=ur2&linkId=32c43af7de64b551eedd0fd89f65bb12&camp=1634&creative=6738&index=computers&keywords= Goalake PoE+ Switch 5 Port 100Mbps">Goalake PoE+ Switch 5 Port 100Mbps</a>
This is a stop gap measure to power my PoE cameras, it's ugly and inefficient, but cheap! Works fine and with just the cameras performance is less important!



# My smart home setup
My Home Assistant, devices, configs, automation etc

## Home Assistant addons
### Mosquitto broker (mqtt)
https://github.com/home-assistant/addons/blob/master/mosquitto/DOCS.md

### ESPHome
https://esphome.io/

### Music Assistant
https://music-assistant.io/ 

### Ring-MQTT with Video Streaming
https://github.com/tsightler/ring-mqtt

### snapcast-server
https://github.com/Art-Ev/addon-snapserver

### Zigbee2MQTT
https://www.zigbee2mqtt.io/

## Integrations


# Hardware
## Energy Monitoring/Power Management
Glow IHD which connects to my UK "smart" meter
https://shop.glowmarkt.com/

<a target="_blank" href="https://www.amazon.co.uk/gp/search?ie=UTF8&tag=basuk036-21&linkCode=ur2&linkId=d051727f1b05f9783311c94ec41b7a07&camp=1634&creative=6738&index=computers&keywords= tapo p110  smart plug with energy monitoring">Tapo P110 Smart Plug with Energy Monitoring </a>

<a target="_blank" href="https://www.amazon.co.uk/gp/search?ie=UTF8&tag=basuk036-21&linkCode=ur2&linkId=dcf0db99fcd9f8811a2d294fe0b1f09e&camp=1634&creative=6738&index=computers&keywords= tapo p100  smart plug">Tapo P100 Smart Plug </a>

## Climate
Nest thermostat

## Lighting
Lidl gu10 smart bulbs

Phillips Hue bulbs

IKEA TRÅDFRI bulbs
https://www.ikea.com/gb/en/p/tradfri-led-bulb-b22-1055-lumen-smart-wireless-dimmable-white-spectrum-globe-70517641/
Works great with Home Assistant and easy to setup with ZHA. Low cost.

Generic LED strip (using magichome) x2

## Motion Sensors
IKEA TRÅDFRI motion sensor x3

TUYA mmwave sensor 

ZigBee contact Sensors x5

## Safety
TUYA WiFi smoke alarm

Yale Smarthome water sensor x2

## Remotes/Switches
IKEA Styrbar Remote x4

https://www.ikea.com/gb/en/p/styrbar-remote-control-smart-white-60488366/

Great when they work, but can be a pain. About the same as the Hue switches but much cheaper.

Hue switch x2

## Sensors
Custom  <a target="_blank" href="https://www.amazon.co.uk/gp/search?ie=UTF8&tag=basuk036-21&linkCode=ur2&linkId=883958b075c7546a49bb12350f1088a5&camp=1634&creative=6738&index=computers&keywords=Esp8266 nodemcu boards">ESP8266</a>

with BME280


## Security

<a target="_blank" href="https://www.amazon.co.uk/gp/search?ie=UTF8&tag=basuk036-21&linkCode=ur2&linkId=b18d5cb865489258d94c09d54abd64ab&camp=1634&creative=6738&index=computers&keywords=ANNKE C800 4K POE camera">ANNKE C800</a> x2

Yale Smarthome alarm

# Voice Assistants
Wyoming Satellite

<a target="_blank" href="https://amzn.to/3xdgT3G">Raspberry Pi 3b</a>
<a target="_blank" href="https://amzn.to/4cyn1U2">Respeaker 2mic</a>
Generic Speaker

Google Home Mini x6

Google Nest Hub

Lenovo Smart Display 7

# Dashboards
Amazon Fire Tablet 

Dakboard


# Planned

# Previous kit
Avaya 24 port 1gb managed switch
This was an older, no longer supported switch and required extra equipment to get working. Much more hassle than it's worth.

Cisco 24 port 100mb managed switch
This was an older, no longer supported model and worked great with little configuration. However, 100mb was to slow for my server, HA and my 