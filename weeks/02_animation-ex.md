# Animation: Variables

https://thecodingtrain.com/beginners/p5js/2.1-mousex-mousey.html
https://thecodingtrain.com/beginners/p5js/2.2-make-your-own.html
https://thecodingtrain.com/beginners/p5js/2.3-objects.html
https://thecodingtrain.com/beginners/p5js/2.4-map.html
https://thecodingtrain.com/beginners/p5js/2.5-random.html
https://thecodingtrain.com/beginners/p5js/2.6-create-graphics.html

https://thecodingtrain.com/beginners/p5js/index.html

-------------------------------------------------------------------------------
https://thecodingtrain.com/beginners/p5js/2.3-objects.html
https://www.youtube.com/watch?v=-e5h4IGKZRY
2.3: JavaScript Objects - p5.js Tutorial
190,360 views•Sep 4, 2015

!!@ In homework but not here

ReferenceError: x is not defined

Ex: use object for vars

-------------------------------------------------------------------------------

>> add translate

>> add translate with parameter variables

- use createSlider to drive variable

>> intro objects as group of variables
>> functions with parameters

*The videos in this section were created ~2 years ago. They use different editors for p5.js. All of the concepts should still apply, however, there are some minor changes. Most notably in JavaScript `let` is now the preferred way to declare a variable over `var`. If you would like to learn more about this you can [watch this video about let vs var](https://youtu.be/q8SHaDQdul0).*

## Tutorials: Basics
* `setup()`, `draw()`, and other events: `mousePressed()`, etc.

-------------------------------------------------------------------------------
* Built-in variables
  * [video 2.1: Variables in p5.js (mouseX, mouseY)](https://www.youtube.com/watch?v=RnS0YNuLfQQ&list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA&index=5)

https://thecodingtrain.com/beginners/p5js/2.1-mousex-mousey.html

https://www.youtube.com/watch?v=7A5tKW9HGoM

Flow of code.
function mousePressed() {
}

https://editor.p5js.org/codingtrain/sketches/IeblvUQrf
p5js Code! - 2.1 - mouseX,mouseY

!!@ Need arith to do suggestions

-------------------------------------------------------------------------------
* User defined variables
  * [video 2.2: Variables in p5.js (Make your own)](https://www.youtube.com/watch?v=Bn_B3T_Vbxs&list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA&index=6)

https://thecodingtrain.com/beginners/p5js/2.2-make-your-own.html
https://www.youtube.com/watch?v=dRhXIIFp-ys
2.2: Variables in p5.js (Define Your Own) - p5.js Tutorial
589 views•Feb 24, 2021

variable:
- declare
- init
- use

global variables
all at the top of script
let circleX = 100;

increment
circleX = circleX + 1;

https://editor.p5js.org/codingtrain/sketches/xPXNdPy17
p5js Code! - 2.2 - make your own variable
https://editor.p5js.org/codingtrain/sketches/ehbMJ-otC
p5js Code! - 2.2 - make your own variable - growing circle exercise



-------------------------------------------------------------------------------
* The [random()](http://p5js.org/reference/#/p5/random) function
  * [video 2.5: random()](https://www.youtube.com/watch?v=nfmV2kuQKwA&list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA&index=9)

https://thecodingtrain.com/beginners/p5js/2.5-random.html
https://www.youtube.com/watch?v=nfmV2kuQKwA
172,294 views•Sep 4, 2015

https://editor.p5js.org/codingtrain/sketches/4gD7Btgi

>> Uses objects
var spot = {
  x: 100,
  y: 50
};

!!@ var point --> spot
>> comment out to isolate problem

!!@ global vars not needed

  * [Rainbow Paintbrush in p5.js](https://medium.com/@kellylougheed/rainbow-paintbrush-in-p5-js-e452d5540b25) by Kelly Lougheed


-------------------------------------------------------------------------------
* The [map()](http://p5js.org/reference/#/p5/map) function
  * [video 2.4: map()](https://www.youtube.com/watch?v=nicMAoW6u1g&list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA&index=8)

https://thecodingtrain.com/beginners/p5js/2.4-map.html
https://www.youtube.com/watch?v=nicMAoW6u1g
2.5: The map() Function - p5.js Tutorial
220,353 views•Sep 4, 2015

https://editor.p5js.org/codingtrain/sketches/yJqbGf71
p5js Code! - map function



-------------------------------------------------------------------------------

* Tutorial: [Recode Catalog by John Whitney](https://github.com/itpresidents/icm-help-sessions-2020/blob/master/session-02/session-02.md)

## Tutorials: Transformations
  * [video 9.1: `translate()`, `rotate()`, `push()`, `pop()`](https://youtu.be/o9sgjuh-CBM)

https://www.youtube.com/watch?v=o9sgjuh-CBM
9.1: Transformations Pt.1 (Translate, Rotate, Push/Pop) - p5.js Tutorial
114,330 views•Sep 18, 2017
22 mins

>> angles
>> radians
>> negative numbers to reverse translate/rotate


  * [video 9.2: `scale()`](https://youtu.be/pkHZTWOoTLM)
  * [video 9.3: More on transformations](https://youtu.be/IVMvq9rd8dA)

## p5.js editor examples
  * [random painting](https://editor.p5js.org/icm/sketches/HJg8jfcT3)
  * [mouse controlled painting](https://editor.p5js.org/icm/sketches/r1JeQqa3)
  * [moving circle](https://editor.p5js.org/icm/sketches/Bymv7ca2)
  * [clock](https://editor.p5js.org/icm/sketches/ryYueiWu7) -- [Clock coding challenge video](https://youtu.be/E4RyStef-gY)

## Getting Started with p5.js book
  * Chapters 4 through Ex.4.5, 8 through Ex. 8.9
  * Going further: Chapters 6 (Transformations) and 8.10-8.15 (More complex motion)
  * [Getting Started with p5.js book](http://amzn.to/2ckixCW) | [Ebook (free with NYU Library login)](https://ebookcentral.proquest.com/lib/nyulibrary-ebooks/detail.action?docID=4333728) | [Code](https://github.com/lmccart/gswp5.js-code)


https://editor.p5js.org/jht1493/sketches/1HRbbpwEK
createButton draw_rect
>> basic buttons. apply to variables

>> buttons to clear and draw
  draw with diferent loc and color

>> intro to DOM from the function point of view
>> minial muse of variables
