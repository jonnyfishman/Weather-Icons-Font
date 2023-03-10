![Icon Banner Image](docs/images/banner.png)

## Custom CSS Weather Icons Font with Multicolour Capabilities

This project provides a custom font that includes a set of weather icons with Multicolour capabilities, meaning that each icon can be displayed in different colours. The icons can be easily customised and incorporated into any web project through simple CSS classes.

Demo the fonts and the colour functions at [https://jonnyfishman.github.io/](https://jonnyfishman.github.io/)!

## Installation

To use the weather icons font in your project, you will need to include the following files in your project:

   + `css/weather-icons.min.css` This file contains the styles for the weather icons, including the classes for specifying the colours of the icons.

   + The folder `fonts/`. These re the actual font files for the weather icons and should be placed in the parent folder `../` from the CSS files.

## Usage

To use a weather icon in your project, simply include the appropriate class in an `i` element. For example:

`<i class="wi-few-clouds-day"></i>`

This will display the few clouds day icon ![wi-few-clouds-day](docs/images/few_clouds.png).

To specify the colours of the icon, you must include the class `wi-multiline` along with one or more colour class, like so:

`<i class="wi-few-clouds-day wi-multitone wi-yellow"></i>`

This will display the few clouds day icon using the default primary colour (black) for the first part of the icon and yellow for the second part ![wi-few-clouds-day-multitone](docs/images/few_clouds_yellow.png).

## Available Icons

Included in the font are 12 weather icons (view them here [https://jonnyfishman.github.io/](https://jonnyfishman.github.io/)):

+ `wi-clear-day`: Sunny day icon
+ `wi-few-clouds-day`: A sun and cloud icon
+ `wi-scattered-clouds-day`: A sun and multiple clouds
+ `wi-shower-rain-day`: Rain with a day icon
+ `wi-broken-clouds`: Two clouds icon
+ `wi-rain`: Rain icon
+ `wi-thunderstorm`: Thunderstorm icon
+ `wi-snow`: A snow icon

*All instances of `day` can be replaced with `night` for a moon icon*

8 wind direction icons:

+ `wi-wind` plus direction i.e. `-n` or `-se`

and 24 time of day icons:

+ `wi-tod-0` to `wi-tod-23`

## Customization

The colours of the icons can be easily customised by modifying `:root` code block in the CSS file. Simply specify your desired colours as the value of the colour property:

    :root {
      --primary-color: black;
      --secondary-color: white;
      --second-color: #ffff00;
      --third-color: #c2c2c2;
      --fourth-color: #f24236;
      --fifth-color: #3498db;
    }

For simplicity these colours are matched with the following CSS tags:

    wi-yellow = #ffff00
    wi-grey = #c2c2c2
    wi-red = #f24236
    wi-blue = #3498db

The order of the colours is important with `wi-yellow` being highest and `wi-blue` being the lowest. When combining multiple colours the first colour to be applied will always be the highest in the list.

Fonts can be rotated using the `wi-rotate-*` where `*` is a whole number in degrees.

## Acknowledgments
+ I created this project after using [Erik Flower's](https://github.com/erikflowers/weather-icons) superb weather icons for a different project and wanted to add some extra colour options. His work was a great help in putting together this project.
+ After making the SVGs for each icon they were turned into fonts using [Icoomoon](https://icomoon.io/app/#/select) which is a really helpful website for making custom fonts.

## Licensing

* Weather Icons licensed under [SIL OFL 1.1](http://scripts.sil.org/OFL)
* Code licensed under [MIT License](http://opensource.org/licenses/mit-license.html)
* Documentation licensed under [CC BY 3.0](http://creativecommons.org/licenses/by/3.0)
