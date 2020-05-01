# Hugo CustomShort codes

A collection of custom shortcodes for the Hugo static site generator.


# Usage

Add this repository as a submodule of your Hugo website.

To do that run this command from the root directory of your Hugo website:

    git submodule add https://github.com/randruc/HugoCustomShortcodes layouts/shortcodes/custom

Then you can use the custom shortcodes like so:

    {{<  custom/sourcecode file="demo.c" language="c" from="6" to="12" >}}


# List of custom shortcodes in this repository

## sourcecode

This custom shortcode is a wrapper for the Hugo "highlight" shortcode.
It allows highlighting of source code read from a file.
