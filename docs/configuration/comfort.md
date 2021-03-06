

| Device                                                       | Quantity | Connection        | Integration                                                  | Notes                                                        |
| ------------------------------------------------------------ | :------: | ----------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Ecobee 4](https://www.ecobee.com/en-us/smart-thermostats/smart-wifi-thermostat-with-voice-control/) |    1     | Wi-Fi             | [ecobee](https://www.home-assistant.io/integrations/ecobee/) | Whole home thermostat, with built-in Amazon Alexa.           |
| [Ecobee Room Sensor](https://www.ecobee.com/en-us/accessories/smart-temperature-occupancy-sensor/) |    2     | Ecobee 4          | [ecobee](https://www.home-assistant.io/integrations/ecobee/) | Temperature and Occupancy sensor.  Wonder why they did not include humidity sensing. |
| [Airthings Wave Plus](https://www.airthings.com/wave-plus)   |    1     | Bluetooth         | [ESPHome](https://www.home-assistant.io/integrations/esphome/) | Indoor  CO<sub>2</sub>, Radon, and temperature sensor. (*) See below |
| [Aqara sensors](https://www.gearbest.com/access-control/pp_626702.html?wid=1433363) |    4     | HUSBZB-1 (Zigbee) | [Zigbee](https://www.home-assistant.io/integrations/zigbee/) | Temperature, humidity, and occupancy sensors.                |
| Xiaomi Mijia Bluetooth Thermometer 2                         |    3     | Bluetooth         | [ESPHome](https://www.home-assistant.io/integrations/esphome/) | See note below (§)                                           |
| DIY                                                          |    3     | Wi-Fi             |                                                              | DHT 22 temperature sensor and humidity sensors on ESP8266 microcontrollers, [configured and controlled](https://esphome.io/components/sensor/dht.html) via  ESPHome. |
| [Netatmo](https://www.netatmo.com/en-us/weather/weatherstation) |    1     | Wi-Fi             | [Netatmo](https://www.home-assistant.io/integrations/netatmo/) | Indoor  CO<sub>2</sub>, Air Quality, temperature, and Sound sensors. The outdoor module is not working. |
| [Environment Canada](https://weather.gc.ca/index_e.html)     |    1     | Cloud             | [Environment Canada](https://www.home-assistant.io/integrations/environment_canada/) | Official weather service by Goverrnment of Canada            |
| [Dark Sky](https://darksky.net/)                             |    1     | Cloud             | [Dark Sky](https://www.home-assistant.io/integrations/darksky/) | See below (soon to be deprecated)                            |
| [AirVisual](https://www.home-assistant.io/integrations/airvisual/) |    1     | Ethernet          | [Airvisual](https://www.home-assistant.io/integrations/airvisual/) | Custom Shell script for managing Integration                 |
| [OpenUV](https://www.openuv.io/)                             |    1     | Cloud             | [Openuv](https://www.home-assistant.io/integrations/openuv/) | UV and Ozone data                                            |

(*) Airthings has a native integration.  But this polls their cloud using login credentials. I prefer local integration which is fast, and well, local. 

(§) Model: LYWSD03MMC. At $15 for a pack of three, these are very good value, considering that they display the temperature and humidity.  I use them in my terrarium and near the cluster of plants.  They run a custom firmware (so no longer connect to Xiaomi), [Telink Flasher for Mi Thermostat](https://atc1441.github.io/TelinkFlasher.html) and are scanned using Esp32 BLE scanner (described in the plants section). 
