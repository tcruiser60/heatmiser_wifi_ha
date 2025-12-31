#  Heatmiser WiFi Home Assistant Component


Alternate approach to update the intergration -  [iainbullock/heatmiser_wifi_ha](https://github.com/iainbullock/heatmiser_wifi_ha).
Ian's version replicates the old Heatmiser App. and includes scheduleing and Hot Water Control.



## Overview
A [Heatmiser](http://www.heatmiser.com/) WiFi Thermostat Home Assistant plugin.

Supports:

* Read current air temperature
* Read/set temperature setting (i.e. wanted temperature)
* Read/set on/off of the Thermostat

Supported Heatmiser Thermostats are WiFi versions of DT, DT-E, PRT and PRT-E.

Note that non-WiFi thermostat versions (i.e. using RS-485 serial bus) 
connected through an Heatmiser Ethernet HUB are supported by the
[Home Assistant Heatmiser Core component](https://www.home-assistant.io/integrations/heatmiser/)


Ti install copy the heatmiser_wifi directory and its contents to the 
Home Assistant /config/custom_components directory.

## Configuration
Add following configuration to Home Assistant configuration.yaml

    climate:
    - platform: heatmiser_wifi
        host:          <mandatory - hostname or ip address>
        port:          <optional  - default 8068>
        pin:           <optional  - default 0>
        friendly_name: <optional  - default 'Heatmiser MODELNO'>
  
## See also
* [Heatmiser_Wifi_HA](https://github.com/iainbullock/heatmiser_wifi_ha) alternate approach for intergrating PRT-HW.
* [original version Heatmiser Wifi](https://github.com/midstar/heatmiser_wifi) the library used for communication with Heatmiser WiFi
* [ianbullock/Heatmiser_wifi](https://github.com/iainbullock/heatmiser_wifi) the library used for communication with Heatmiser WiFi
* [Home Assistant Heatmiser Core component](https://www.home-assistant.io/integrations/heatmiser/) for non WiFi versions of Heatmister Thermostats.
 
### Author and license
This component is written by Joel Midstjärna and is licensed under the MIT License.
