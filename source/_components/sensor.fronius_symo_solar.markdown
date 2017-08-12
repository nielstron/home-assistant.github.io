---
layout: page
title: "Fronius Symo Solar"
description: "Instructions how to integrate Fronius Symo solar data into Home Assistant."
date: 2017-08-11 23:01
sidebar: true
comments: false
sharing: true
footer: true
logo: 
ha_category: Sensor
ha_release: 0.1
ha_iot_class: "Local Polling"
---


The Fronius Symo Solar sensor polls current data from your Fronius Symo about the power production of installed solar panels.
Most times the Fronius Symo is accessible through the local network. 
It sums up the available data in a group.

To enable this sensor, add the following lines to your `configuration.yaml` file:

```yaml
# Example configuration.yaml entry
sensor:
  - platform: fronius_symo_solar
    resource: http://IP_ADDRESS_OF_YOUR_FRONIUS/
```

The IP address can be accessed by checking the list of devices that are logged in to your local network (for example through your router).
Usually the Symo hosts its own website.