# polybar-weather

A simple module for polybar that shows weather.

![alt text](https://github.com/AntonioManceraGamez/polybar-weather/blob/development/screenshots/example.png)

## Usage
Clone this repository and add to your polybar/config.ini (usually in ``.config/polybar/config.ini``)

    [module/weather]
    type = custom/script
    exec = /path/to/polybar-weather/weather
    interval = 30

## Requiremetns
Geopy python library, install using ``pip install geopy``

## Configuration
Edit the ``config.yaml`` file to change some settings, such as location (coords) and units. These are the defaults:

	config:
		coords:
			latitude: 36.73
			longitude: -4.62
		units:
			temperature: celsius
			windspeed: kmh
			precipitation: mm
		timezone: auto

Data is gotten from open-weather.com API

