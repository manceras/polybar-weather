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
Geopy python library, install using ``pip install geopy``.


## Configuration
Edit the ``config.yaml`` file to change some settings, such as location (coords) and units. These are the defaults:

		config:
			location: Cartama
				# latitude: 36.73
				# longitude: -4.62
			units:
				temperature: celsius
				windspeed: kmh
				precipitation: mm
			timezone: auto

In location, use an adress (such as Cartama, New York, Paris) or use the latitude and longitude parameters to set an exact coordinate. Using a street name will work but introducing the house number won't.

---

Data is gotten from [open-meteo.com](https://open-meteo.com) API

