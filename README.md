# ledpijp

71 APA-102 LEDs mounted in a hornbach fixture, driven by an esp-8266

## interacting

- visit the IP of the ESP-8266 in a browser
- select the animation you want
- inspect the page source, reverse engineer the API routes

## specs

- tries to approximate 144 Hz refresh rate

## todo

_patches welcome_

- [X] API route to get currently chosen animation
- [X] increase and decrease brightness at runtime
- [X] strobe light
- [X] API route to get brightness
- [X] API route to get speed
- [X] show the correct speed slider depending on animation
- [ ] reset button
- [ ] save brightness in nvram
- [ ] API route to allow arbitrary solid-color switching (use cycle, slow it down, then slow it to zero when it's where you want)
- [ ] more animations
- [ ] use the onboard (H)SPI functionality of the ESP-8266
- [ ] use NTP syncing to switch animations depending on time of day
- [ ] [redshift](https://github.com/jonls/redshift)-style animation that darkens in the evening and brightens in the morning
- [ ] API route to allow fully custom animations using a simple intrepreted language or expression
- [ ] use a more serious template for HTTP responses
- [ ] minimal css styling for `GET /`
