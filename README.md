# typeface-minecraft

The CSS and web font files for the Minecraft typeface and colors

## Install

`npm install --save @south-paw/typeface-minecraft`

or

`yarn add @south-paw/typeface-minecraft`

## Use

This project assumes that you're using webpack to process CSS and files.

The package includes the necessary font files (woff2, woff) and a CSS file with font-face declarations pointing at these files.

You will need to have webpack setup to load css and font files.

Many tools built with Webpack will work out of the box with this package such as [Gatsby](https://github.com/gatsbyjs/gatsby) and [Create React App](https://github.com/facebook/create-react-app).

To use, simply require the package in your project's entry file:

```js
// Load Minecraft typeface
require("@south-paw/typeface-minecraft");
```

and then apply the font family via CSS:

```css
body {
  font-family: "Minecraft";
}
```

The package also adds some global CSS classes for matching Minecraft colors:

```css
.minecraft-black
.minecraft-dark-blue
.minecraft-dark-green
.minecraft-dark-aqua
.minecraft-dark-red
.minecraft-dark-purple
.minecraft-gold
.minecraft-gray
.minecraft-dark-gray
.minecraft-blue
.minecraft-green
.minecraft-aqua
.minecraft-red
.minecraft-light-purple
.minecraft-yellow
.minecraft-white
```

Any of these can be applied to an element e.g.

```html
<div class="minecraft-blue">Minecraft</div>
```

## Source

Colors are from the [Minecraft wiki](https://minecraft.gamepedia.com/Formatting_codes).

Package is inspired by the [typefaces project](https://github.com/KyleAMathews/typefaces).
