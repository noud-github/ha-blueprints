# ha-blueprints

### ikea-somrig

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fnoud-github%2Fha-blueprints%2Fblob%2Fmain%2Fikea-somrig%2Fdeconz-ikea-somrig-switch.yaml)

Here’s a blueprint to support controlling a things with an Ikea Somrig remote. It’s designed to work with the device added via Deconz only.


### ikea-Styrbar

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fnoud-github%2Fha-blueprints%2Fblob%2Fmain%2Fikea-styrbar%2Fdeconz-ikea-styrbar-switch.yaml)

Here’s a blueprint to support controlling a things with an Ikea Styrbar remote. It’s designed to work with the device added via Deconz only.


### RGB disco change

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fnoud-github%2Fha-blueprints%2Fblob%2Fmain%2Frgb-disco%2Fdisco_light.yaml)

Here’s a blueprint to randomly change RGB disco light needs jinja macro function!!!.

./custom_templates/lights.jinja
```
{% macro getColor_data_template_json() %}
{ "data_template":{ "rgb_color":[ "{{(range(0, 255)|random)}}", "{{(range(0, 255)|random)}}", "{{(range(0, 255)|random)}}"]}}
{% endmacro %}
```