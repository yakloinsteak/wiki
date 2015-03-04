# Responsive Images

* [http://blog.cloudfour.com/sensible-jumps-in-responsive-image-file-sizes/](http://blog.cloudfour.com/sensible-jumps-in-responsive-image-file-sizes/)

* Aim for about 20KB between successive images when creating duplicates.

* [Which responsive solution should you use?](https://css-tricks.com/which-responsive-images-solution-should-you-use/)

## `<picture>` element

To allow specification of multiple images depending on capabilities, use the picture element:

http://responsiveimages.org/#implementation


    <picture>
      <source media="(min-width: 40em)"
        srcset="big.jpg 1x, big-hd.jpg 2x">
      <source
        srcset="small.jpg 1x, small-hd.jpg 2x">
      <img src="fallback.jpg" alt="">
    </picture>

and since it's not fully supported, you'll need this polyfill:

http://scottjehl.github.io/picturefill/

## `srcset` on image tags

use `srcset` and `sizes` attributes. `srcset` is recommended with one alternative, a 2x version.

## Responsive Image JavaScript

* HiSRC: [https://github.com/teleject/hisrc](https://github.com/teleject/hisrc)
* Foresight: [https://github.com/adambradley/foresight.js](https://github.com/adambradley/foresight.js)

## Image Resizing Services

* [www.resrc.it](http://www.resrc.it)
* [www.thumbr.io](http://www.thumbr.io)
* [responsive.io](http://responsive.io)
