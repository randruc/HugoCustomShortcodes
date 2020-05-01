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

This custom shortcode is a wrapper for the Hugo "highlight" shortcode. It allows highlighting of source code
read from a file.

Usage example:

    {{<  sourcecode file="demo.c" language="c" from="3" to="15" >}}

Parameters are:
    file      (mandatory) : The file to read content from. The path is relative to the calling page.
    language  (mandatory) : The source language.
    from      (optional)  : The first line to read.
    to        (optional)  : The last line to read.
    highlight (optional)  : The set of lines to highlight.
    linum     (optional)  : The setting of this option to any value will switch on line numbers printing.
    style     (optional)  : The style to use. This option has the priority. If this option is not set, then the style is taken
                            from the site param named "highlightTheme". If this site param is not set, then the default style is
                            applied.