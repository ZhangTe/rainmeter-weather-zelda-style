## What's this assets?

This assets shows how 
- To get the information of forecast;
- We use the element in ventusky;

## Get element from webpage

We use [Ventusky](https://www.ventusky.com/) as the forecast database and webpage;

The element in the webpage we need is :


```html
<body>
	<div id="aside">
		<forecast data-forecast="...">
			<div class="forecast_block">
				<ul class="menu clearfix">
					<li id="d_1">
						<a>
							<span class="big_icon big_ico_1">  
							
```


*big_ico_1* is what I want;

## How to use the asset

To see what "big_ico_1" here means, see *ventusky icon map* in asset folder.<br/>

The ventusky use icon number 1-25 as different weather. If you want to change a theme of weather icon, set the different icons' file name as how it is shown in the map. 

Use these: 
- part of the css file from ventusky,  
- ventusky icon map ;
	(The map is simply showed in ventusky_icon_map chart.
	The image file (svg) is pocasi_ikony_v4.)
- ventusky icons folder
- the theme folder
to check how weather icon and the number is corresponded.

file link:
https://cdnstatic.ventusky.com/media/style.css?1670664960




