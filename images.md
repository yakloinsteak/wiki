# Images


## New picture element

To allow specification of multiple images depending on capabilities, use the picture element:

http://responsiveimages.org/#implementation

and since it's not fully supported, you'll need this polyfill:

http://scottjehl.github.io/picturefill/

* use `srcset` and `sizes` attributes. `srcset` is recommended with one alternative, a 2x version.
