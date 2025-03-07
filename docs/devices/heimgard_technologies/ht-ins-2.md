---
title: "Heimgard Technologies HT-INS-2 Homebridge/HomeKit integration"
description: "Add HomeKit support to your Heimgard Technologies HT-INS-2, using Homebridge, Zigbee2MQTT and homebridge-z2m."
---
<!---
This file has been GENERATED using src/docgen/docgen.ts
DO NOT EDIT THIS FILE MANUALLY!
-->
# Heimgard Technologies HT-INS-2
> Indoor siren


# Services and characteristics
The following HomeKit Services and Characteristics are exposed by
the Heimgard Technologies HT-INS-2

* [Battery](../../battery.md)
  * Battery Level
  * Charging State
  * Status Low Battery



## Exposes

This is the information provided by Zigbee2MQTT for this device:

```json
[
  {
    "name": "warning",
    "label": "Warning",
    "access": 2,
    "type": "composite",
    "property": "warning",
    "features": [
      {
        "name": "mode",
        "label": "Mode",
        "access": 2,
        "type": "enum",
        "property": "mode",
        "description": "Mode of the warning (sound effect)",
        "values": [
          "stop",
          "burglar",
          "fire",
          "emergency",
          "police_panic",
          "fire_panic",
          "emergency_panic"
        ]
      },
      {
        "name": "level",
        "label": "Level",
        "access": 2,
        "type": "enum",
        "property": "level",
        "description": "Sound level",
        "values": [
          "low",
          "medium",
          "high",
          "very_high"
        ]
      },
      {
        "name": "strobe_level",
        "label": "Strobe level",
        "access": 2,
        "type": "enum",
        "property": "strobe_level",
        "description": "Intensity of the strobe",
        "values": [
          "low",
          "medium",
          "high",
          "very_high"
        ]
      },
      {
        "name": "strobe",
        "label": "Strobe",
        "access": 2,
        "type": "binary",
        "property": "strobe",
        "description": "Turn on/off the strobe (light) during warning",
        "value_on": true,
        "value_off": false
      },
      {
        "name": "strobe_duty_cycle",
        "label": "Strobe duty cycle",
        "access": 2,
        "type": "numeric",
        "property": "strobe_duty_cycle",
        "description": "Length of the flash cycle",
        "value_max": 10,
        "value_min": 0
      },
      {
        "name": "duration",
        "label": "Duration",
        "access": 2,
        "type": "numeric",
        "property": "duration",
        "description": "Duration in seconds of the alarm",
        "unit": "s"
      }
    ]
  },
  {
    "name": "battery",
    "label": "Battery",
    "access": 5,
    "type": "numeric",
    "property": "battery",
    "description": "Remaining battery in %",
    "category": "diagnostic",
    "unit": "%",
    "value_max": 100,
    "value_min": 0
  }
]
```

# Related
* [Other devices from Heimgard Technologies](../index.md#heimgard_technologies)
* [Zigbee2MQTT documentation for this device](https://www.zigbee2mqtt.io/devices/HT-INS-2.html)