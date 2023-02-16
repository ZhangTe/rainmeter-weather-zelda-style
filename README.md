# Weather Widget
This weather widget with zelda BotW style is a set of [Rainmeter](https://docs.rainmeter.net/) skin. <br/>

![Thumbnail](https://github.com/ZhangTe/rainmeter-weather-zelda-style/blob/main/Asset/screenshot1.png)
<br/>

The weather icons show the current weather and forecast for next 3 days.<br/>

The data is from [Ventusky](https://www.ventusky.com/)

## Usage

### Load Skin
Put `Ventusky_with_baiduIcon` in the your themes folder. <br/>

Refresh the Rainmeter themes. Use `Ventusky_with_baiduIcon\webweather_ventusky_4_day.ini` to load the skin.

### Change the location

Open `webweather_ventusky_4_day.ini` file, find the part
```ini
[MeasureSite]
Measure=WebParser
UpdateRate=3600;
;{location} change to your location
Url=https://www.ventusky.com/zh/{location}
RegExp=#Reg_Exp#
```
Change the `{location}` part to your city, like `new-york`:

```ini
Url=https://www.ventusky.com/zh/new-york
```

Visit [Ventusky](https://www.ventusky.com/) and find your city on map then click it, you can check the web-url if you don't know exactly how your city name is restored on the website.