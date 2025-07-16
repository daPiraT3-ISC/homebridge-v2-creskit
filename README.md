# homebridge-v2-creskit

IT'S A FORK!

CresKit (together with Homebridge) turns Creston controlled devices into HomeKit accessories, enabling you to control many functions using Siri and the iOS Home app. 

As of CresKit 2.0.1 the following HomeKit accessories are supported:

- Lights (dimming available)
- Switches
- Scenese
- Garage Doors
- Alarm
- Thermostat
- Shades

In Homebridge's config.json file you specify the accessories you want to enable, and link the appropiate Crestron signals via the included SIMPL+ Module (only tested on MC4 - July 2025). You can then use the iOS Home app to tie the accessories to rooms and groups.

On the Crestron side, the SIMPL+ Module acts as a basic TCP Server and communicates using three type of commands:

- Set (Controls Crestron from Homebridge)
- Get (Requests Crestron status from Homebridge)
- Event (Pushes Crestron status changes to Homebridge)
