# Images


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

* use `srcset` and `sizes` attributes. `srcset` is recommended with one alternative, a 2x version.
