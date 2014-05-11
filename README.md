# niu-x2 lazy load helper

This pelican plugin is inspired by the plugin [better figures and images](https://github.com/getpelican/pelican-plugins/tree/master/better_figures_and_images) and is intended to be used with the theme [niu-x2-sidebar](https://github.com/mawenbao/niu-x2-sidebar).

To all the img tags in the html document, this plugin do these things:

* add attributes:
    * width: real width of the image file, in px.
* if `NIUX2_LAZY_LOAD` is set as True in your pelican configuration:
    * add the following attributes:
        * data-height: real height of the image file, in px.
        * data-width: real width of the image file, in px.
    * add class `lazy`.
    * move attribute `src` to attribute `data-original`.

## Requirements

    pip install pillow beautifulsoup4

