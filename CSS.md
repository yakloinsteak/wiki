# CSS

* [Syntactically Awesome Style Sheets](http://sass-lang.com)

* Test responsive dimensions/parameters as [http://mqtest.io](http://mqtest.io)

* How grids work: [http://css-tricks.com/dont-overthink-it-grids/](http://css-tricks.com/dont-overthink-it-grids/)

* Theory of grid design: [http://grids.subtraction.com/](http://grids.subtraction.com/)

* [CSS Validator](http://jigsaw.w3.org/css-validator)

* Window resizer plugin for Chrome. Native in Firefox.

* Transitions:[CSS Transitions](https://css-tricks.com/almanac/properties/t/transition/)

* Fall-back rule: Convert from pixels to ems by dividing by 16.



## Scratchpad of CSS boilerplate as SASS
    // Let's just avoid margin/padding calculations and call it a day.
    *, *:after, *:before
      box-sizing: border-box

    // Constrain images to parent container
    img
      max-width: 100%

    // Needs <html lang=en>
    body
      font-size: 100%

      -webkit-hyphens: auto
      -moz-hyphens: auto
      -ms-hyphens: auto
      -o-hyphens: auto
      hyphens: auto

      word-wrap: break-word
      overflow-wrap: breakword


## Font Stack no-brainers

    body
      font-family: Baskerville, 'Times New Roman', Times, serif
      font-family: Garamond, 'Hoefler Text', 'Times New Roman', Times, serif
      font-family: Geneva, 'Lucida Sans', 'Lucida Grande', 'Lucida Sans Unicode', Verdana, sans-serif
      font-family: GillSans, Calibri, Trebuchet, sans-serif

    h1,h2,h3,h4,h5
      font-family: Georgia, Times, 'Times New Roman', serif
      font-family: Palatino, 'Palatino Linotype', 'Hoefler Text', Times, 'Times New Roman', serif
      font-family: Tahoma, Verdana, Geneva
      font-family: Trebuchet, Tahoma, Arial, sans-serif

    something
      font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif
      font-family: Cambria, Georgia, Times, 'Times New Roman', serif
      font-family: 'Copperplate Light', 'Copperplate Gothic Light', serif
      font-family: Futura, 'Century Gothic', AppleGothic, sans-serif
