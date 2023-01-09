# Weather Icons Font

## Custom CSS Weather Icons Font with Dualtone Capabilities

This project provides a custom font that includes a set of weather icons with dualtone capabilities, meaning that each icon can be displayed in two different colours. The icons can be easily customised and incorporated into any web project through simple CSS classes.

Demo the fonts and the colour functions at [https://jonnyfishman.github.io/](https://jonnyfishman.github.io/)!

## Installation

To use the weather icons font in your project, you will need to include the following files in your project:

   + `css/weather-icons.min.css` This file contains the styles for the weather icons, including the classes for specifying the colours of the icons.

   + The folder `fonts/` This is the actual font file for the weather icons and should be placed in the parent folder `../` from the CSS files.

## Usage

To use a weather icon in your project, simply include the appropriate class in an `i` element. For example:

`<i class="wi-few-clouds-day"></i>`

This will display the few clouds day icon.

To specify the colours of the icon, you must include the class `wi-multiline` along with one or more colour class, like so:

`<i class="wi-few-clouds-day wi-multitone wi-yellow"></i>`

This will display the few clouds day icon using the default primary colour (black) for the first part of the icon and yellow for the second part.

## Available Icons

Included in the font are 12 weather icons:

   + `wi-clear-day`: Sunny day icon
   + `wi-few-clouds-day`: A sun and cloud icon
   + `wi-scattered-clouds-day`: A sun and multiple clouds
   + `wi-shower-rain-day`: Rain with a day icon
   + `wi-broken-clouds`: Two clouds icon
   + `wi-rain`: Rain icon
   + `wi-thunderstorm`: Thunderstorm icon
   + `wi-snow`: A snow icon

**All instances of `day` can be replaced with `night` for a moon icon**

8 wind direction icons:

    + `wi-wind` plus direction i.e. `-n` or `-se`

and 24 time of day icons:

    + `wi-tod-0` to `wi-tod-23`

## Customization

The colours of the icons can be easily customised by modifying `:root` code block in the CSS file. Simply specify your desired colours as the value of the colour property:

    `:root {
      --primary-color: black;
      --secondary-color: white;
      --second-color: yellow;
      --third-color: #c2c2c2;
      --fourth-color: #f24236;
      --fifth-color: #3498db;
    }`

For simplicity these colours are matched with the following CSS tags:

    `wi-yellow = #ffff00
    wi-grey = #c2c2c2
    wi-red = #f24236
    wi-blue = #3498db`

The order of the colours is important with `wi-yellow` being highest and `wi-blue` being the lowest. When combining multiple colours the first colour to be applied will always be the highest in the list.

Fonts can be rotated using the `wi-rotate-*` where `*` is a whole number in degrees.

## Acknowledgments

## License

This project is licensed under the MIT License. See the LICENSE file for details.
