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

https://frigate.video/

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

Honestly, I picked this as it was noob friendly, but it has never once let me down, even with my dodgy python bombarding it with stats and as such stayed.

### ESPHome
https://esphome.io/

This add on from the HA team makes building DIY Sensors a doddle.

### Music Assistant
https://music-assistant.io/ 

This add on is fantastic and brings my music into Home Assistant. Whilst I am currently playing with Wyoming and snapcast and don't have a finished and reliable speaker at the moment, this will form an important part of reducing my dependence on the cloud.

### Ring-MQTT with Video Streaming
https://github.com/tsightler/ring-mqtt

This add on makes my ring doorbell play nice with Home Assistant and makes all of my front door related automation possible. The camera is just an expensive piece of plastic without it.

### snapcast-server
https://github.com/Art-Ev/addon-snapserver

Similar to Music Assistant, this will form the backbone of my wyoming smart speakers once I have a reliable and affordable working model that can replace all of the Google minis.

### Zigbee2MQTT
https://www.zigbee2mqtt.io/

I previously used ZHA for managing my zigbee network, and it was fantastic and reliable. However, I find my zigbee devices don't always have all of the options/Sensors that should exist and decided to try this. So far it is definitely an upgrade given I love data and pressing random buttons for the lolz. I'd say ZHA for ease of use and getting the basics working and Z2MQTT for better compatibility, more features with less fuss, but not as easy to use (although, after the initial deluge of data and options is quite intuitive).

## Integrations

Alarmo

https://github.com/nielsfaber/alarmo

This addon supercharges the security of my Home and massively simplifies monitoring.

Android TV remote

Electricity Maps

https://app.electricitymaps.com/map

This shows the current CO2 intensity of my local power (gCO2eq/kWh) and the % of fossil fuel in the grid. I'm not currently using this in automation but plan to curb my energy usage when the grid is dirtiest. Saving the planet watt by watt.

Frigate

Fully Kiosk Browser

https://www.home-assistant.io/integrations/fully_kiosk

This integration works with my old Fire device to create a control panel for my Home. The integration allows some control of the dashboard and provides some useful data (such as battery level) allowing for automated charging when the tablet needs some juice.

GDACS

Google Calendar

Google Cast

Google Nest

Allows control of my Nest thermostat, need I say more? Whilst the thermostat does a fine job using its ai smarts, its even better when using all of the additional sensor data provided by HA. I currently have improved automation based on location and temperature. Including using relevant sensors based on occupancy and time of day. (for example, if upstairs is warm at night, shutdown even if the temperature target has not been met). I am also able to factor in other devices, such as if the electric blankets have been on, don't use the heating. (with the smart plugs controlling the blankets used as a proxy measure).

Google Photos

https://github.com/Daanoz/ha-google-photos

A great little integration which pulls my albums from Google Photos into Home Assistant for use in Dashboards.

Hildebrand Glow IHD MQTT

https://github.com/megakid/ha_hildebrand_glow_ihd_mqtt

This makes pulling the data from my electricity and gas meter a lot easier with much less faff!

HomeKit Bridge

Islamic Prayer Times

Magic Home

Met Office

My local weather, free :)

Music Assistant 

Notifications for Android TV / Fire TV

https://www.home-assistant.io/integrations/nfandroidtv

Love this integration, it allows me to send pictures from my cameras and ring doorbell to my GoogleTV stick as a little coloured box!

Onvif

This is used to reduce the strain on my Frigate server by pulling the stream direct from the camera.

OpenAI Conversation 

Presence Simulation 

https://github.com/slashback100/presence_simulation

This makes my house act like my family are home, even if we are not. What's not to like?

Rhasspy

SmartThings

Snapcast

PS4

SpeedTest.net

Monitor my Internet speed and automations to warn me if the speed is below 200 mbps or has been below 400mbps for more than one hour.

Tile

TP Link Smart Home

Tuya

Wyoming Protocol

Xbox

Yale Smart Living



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

Important Tutorials/software: 
https://github.com/rhasspy/wyoming-satellite
https://github.com/badaix/snapcast


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