kanjivg2svg
===========

This Ruby 1.9 script takes stroke order data from the [KanjiVG](http://kanjivg.tagaini.net/) project and outputs SVG files with special formatting.

Usage
-----

    $ ruby kanjivg2svg.rb path/to/kanji [frames|animated|numbers]

You can change the output type by setting the second argument. If not set it will default to 'frames'. The animated and numbers are less perfected compared to the frames output.

For the animation to work, the generated svg cannot be loaded as an image.

source html needs to contains the following css:
```
.draw2 {
  stroke-dasharray: 100;
  stroke-dashoffset: 100;
  animation: dash2 1s linear forwards;
}
@keyframes dash2 {
  to { stroke-dashoffset: 0;}
}  
```

License
-------

By Kim Ahlström <kim.ahlstrom@gmail.com>

[Creative Commons Attribution-Share Alike 3.0](http://creativecommons.org/licenses/by-sa/3.0/)

KanjiVG
-------

KanjiVG is copyright (c) 2009/2010 Ulrich Apel and released under the Creative Commons Attribution-Share Alike 3.0
