# Weather Widget
This weather widget with zelda BotW style is a set of [Rainmeter](https://docs.rainmeter.net/) skin. <br/>

![Thumbnail](https://github.com/ZhangTe/rainmeter-weather-zelda-style/blob/main/Asset/screenshot1.png)
<br/>

The weather icons show the current weather and forecast for next 3 days.<br/>

The data is from [Ventusky](https://www.ventusky.com/)

## Usage

### Load Skin
Put `Ventusky_with_baiduIcon` in your themes folder. <br/>

Refresh the Rainmeter themes. Use `Ventusky_with_baiduIcon\webweather_ventusky_4_day.ini` to load the skin.

### Change the location

Open `webweather_ventusky_4_day.ini` file, find the part
```ini
[Variables]
;{location} change to your location
Url_weather=https://www.ventusky.com/{location}
```
Change the `{location}` part to your city, like `new-york`:

```ini
Url_weather=https://www.ventusky.com/new-york
```

Some city name may need longtitude and latitude (or other arguments) because of the Duplicate name like Peterborough in England and Canada:

```ini
; Peterborough in Canada
https://www.ventusky.com/peterborough;44.3;-78.33
; Peterborough in England
https://www.ventusky.com/peterborough
```
Use coordinates(longtitude and latitude) directly:

```ini
; somewhere in Alaska
Url_weather=https://www.ventusky.com/62.283;-155.028
```

Visit [Ventusky](https://www.ventusky.com/) and find your city on map then click it, you can check the web-url if you don't know exactly how your city name or data is stored on the website.

## The Termometer

### Thermometer scale



<br/>

![thermoscale](https://github.com/ZhangTe/rainmeter-weather-zelda-style/blob/main/Asset/Thermometer_scale.png)

<br/>

### Thermometer not moving

If the Thermometer always lays on 0, try to change the other regular expression here:

```ini
[Variables]

 ....
 
;Thermometer not moving?
;If the temperature information cannot loaded, try the other regular expression
Reg_Exp_tmp=(?s)<td\s+class="temperature">\s+((\-)?\d+(\.\d+)?)
;Reg_Exp_tmp=(?s)<b\s+class="teplota">\s*((\-)?\d+(\.\d+)?)

```

This is because some of the cities don't have actual information panel.
The second regular expression can also be used when you want to use coordinates(longtitude and latitude) directly.


