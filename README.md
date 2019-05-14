# Jekyll Template

This is a barebones template for Jekyll using Filament Group's [LoadJS](https://github.com/filamentgroup/loadJSFilament) and
[LoadCSS](https://github.com/filamentgroup/loadCSS) so you can get fast loading site.

I've built this using recommendations from google page speed insights.

It includes jekyll-livereload for easy development.

[Here is a version that includes Bootsrap 4 CSS and JS](https://github.com/thauvette/jekyll-bootstrap-starter-template)

If you haven't set up Jekyll yet [follow these instructions.](https://jekyllrb.com/docs/installation/)

## Set up
* Run `bundle`
* Run `jekyll serve`

That's it.

## Adding JS and CSS
### CSS
To load additional css files use...

`<link rel='preload' href='/path/to/stylesheet.css' as='style' onload='this.rel="stylesheet"'>`
`<noscript><link rel='stylesheet' href='/path/to/stylesheet.css'></noscript>`

as per [LoadCSS](https://github.com/filamentgroup/loadCSS).

For custom styles, place all sass files in `assets/_sass` and use `@import 'filename'` with no extension in the `assets/css/main.scss`

### JS
For adding JS files see the instructions in `assets/js/loader.js`. It is designed to load files asynchronous and prevent render blocking.

## Recomendations

I like to put any important styles in the `_inludes/prority-css.html` file. This is mostly to prevent flashes of un-styled content.  

Use [Favicon Generator](https://realfavicongenerator.net/) to generate your own favicon. Replace all the files in the root folder with the ones it generates for you. The theme colour can be changed in the `_includes/head.html` file.

## Props and Thanks to...
* Filament Group's [LoadJS](https://github.com/filamentgroup/loadJSFilament) and
[LoadCSS](https://github.com/filamentgroup/loadCSS)
* penibelst's [HTML Compression](https://github.com/penibelst/jekyll-compress-html)
* [jpeg.io](https://www.jpeg.io/) for image compression
* [tiny png](https://tinypng.com/) for png compression
* [Favicon Generator](https://realfavicongenerator.net/)
