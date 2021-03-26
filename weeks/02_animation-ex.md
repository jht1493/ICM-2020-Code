# Animation: Variables
https://github.com/jht1493/ICM-2020-Code/blob/master/weeks/02_animation.md

[![](../assets/Ex_08_03-Move-0.png) ![](../assets/Ex_08_03-Move-1.png)](https://editor.p5js.org/jht1493/sketches/W_nCg2LI2)
![](../assets/Ex_08_03-Move-1.png) ![](../assets/Ex_08_03-Move-2.png)

https://thecodingtrain.com/beginners/p5js/2.1-mousex-mousey.html
https://thecodingtrain.com/beginners/p5js/2.2-make-your-own.html
https://thecodingtrain.com/beginners/p5js/2.3-objects.html
https://thecodingtrain.com/beginners/p5js/2.4-map.html
https://thecodingtrain.com/beginners/p5js/2.5-random.html
https://thecodingtrain.com/beginners/p5js/2.6-create-graphics.html

https://thecodingtrain.com/Tutorials/9-additional-topics/9.1-transformations-part-1.html
https://thecodingtrain.com/Tutorials/9-additional-topics/9.2-transformations-part-2.html
https://thecodingtrain.com/Tutorials/9-additional-topics/9.3-transformations-art-3.html


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

// https://editor.p5js.org/jht1493/sketches/KaijsTyVc
// 2.1.1 mouseX,mouseY

function mouseDragged() {
  circle(mouseX, mouseY, 24);
}

// https://editor.p5js.org/jht1493/sketches/pmA0d9Uqt
// 2.1.2 mouseX,mouseY arith

>> a value can be an arithmetic expression
function mouseDragged() {
  circle(mouseX-25, mouseY, 24);
  circle(mouseX+25, mouseY, 24);
}

// https://editor.p5js.org/jht1493/sketches/5Q_M3rwpt
// 2.1.3 mouseX,mouseY left

>> intro remainder
function mouseDragged() {
  circle(mouseX % 200, mouseY, 24);
}

// https://editor.p5js.org/jht1493/sketches/I8zejgYIX
// 2.1.4 mouseX,mouseY ui

>> ui added
>> Replace mousePressed with mouseDragged
>> button backg 0
>> button random

>> Try: draw 4 circles around mouse location

>> Try: write functions to draw other shapes call them from mouseDragged
// https://editor.p5js.org/jht1493/sketches/tNEJXRA1V
// 2.1 mouseX,mouseY funcs

>> Try: remainder for x-symmetry
// https://editor.p5js.org/jht1493/sketches/v56Rd_pWx
// 2.1 mouseX,mouseY mirror
function mouseDragged() {
  circle(mouseX % 200, mouseY, 24);
  circle(width - (mouseX % 200), mouseY, 24);
}

>> Try: use raminder to get Y-symmetry

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

>> ?? slider for alpha
  interesting values are low, slide not helpful
>> slider for brush size ??
>> Try: buttons for circle size

// !!@ Expand on expresions
circleX = (circleX + 1) % width;

https://editor.p5js.org/codingtrain/sketches/xPXNdPy17
p5js Code! - 2.2 - make your own variable

  circle(circleX, 150, 64);
  circleX = circleX + 1;

>> mouse presssed out side of canvas will reset

// https://editor.p5js.org/jht1493/sketches/v9zsQFPqN
// 2.2 variable circleX

  createCanvas(400, 300).mousePressed(function() {
    circleX = 0;
  });

>> mouse presssed on canvas only to reset circleX

function mousePressed() {

// https://editor.p5js.org/jht1493/sketches/CwYDz_4N2
// 2.2.2 variable circleX % width

>> variable restricted to 0 ... width
  circleX = (circleX + 1) % width;

// https://editor.p5js.org/jht1493/sketches/UhNMB6GQO
// 2.2.3 variable circleX % width ui

>> ui added. add buttons to change circleX and/or circleY

>> Try: no background

>> Try: buttons to change color of shape

// https://editor.p5js.org/jht1493/sketches/mDleb9mKk
// 2.2.4 variable circleX rgb


-------------------------------------------------------------------------------
* The [random()](http://p5js.org/reference/#/p5/random) function
  * [video 2.5: random()](https://www.youtube.com/watch?v=nfmV2kuQKwA&list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA&index=9)

https://thecodingtrain.com/beginners/p5js/2.5-random.html
https://www.youtube.com/watch?v=nfmV2kuQKwA
172,294 views•Sep 4, 2015
https://editor.p5js.org/codingtrain/sketches/4gD7Btg

// https://editor.p5js.org/jht1493/sketches/UTMOVgcsv
// 2.5.1 random function 

// https://editor.p5js.org/jht1493/sketches/XzrXlqxMN
// 2.5.1 random function scan x

  spot.x = (spot.x + 1) % width;
  spot.y = random(0, height);

// https://editor.p5js.org/jht1493/sketches/ny4aSEPTp
// 2.5.1 random function scan x ran y

  spot.x = (spot.x + 1) % width;
  let h = height/8;
  spot.y = random([h, h*3, h*5, h*7]);

// https://editor.p5js.org/jht1493/sketches/vpcHXx_E1
// 2.5.2 random function spot.count

  spot.count = spot.count + spot.d;
  spot.x = spot.count % width;
  spot.y = (int(spot.count / width) * spot.d) % height;

>> Try: have scan bottom to top, right to left

// https://editor.p5js.org/jht1493/sketches/A1NHTo3cg
// 2.5.2 random function spot.count ui bottom

  spot.count = spot.count + spot.d;
  spot.x = width - (spot.count % width);
  spot.y = height - ((int(spot.count / width) * spot.d) % height);

>> Try: limit to fix set of colors

Use: array of values in 
https://p5js.org/reference/#/p5/random
  random(choices)
  choices Array: the array to choose from
https://p5js.org/reference/#/p5/fill
  fill(values)
  values Number[]: an array containing the red,green,blue & and alpha components of the color

// https://editor.p5js.org/jht1493/sketches/jZtF7e5E5
// 2.5.2 random spot.count ui col set

let col_set = [
  [255, 0, 0, a_alpha],
  [0, 255, 0, a_alpha],
  [255, 255, 0, a_alpha],
  [0, 0, 0, a_alpha],
  // [255, 255, 255, a_alpha]
];

  let col = random(col_set);
  col[3] = a_alpha;

    frameRate(0);

    frameRate(10);

-------------------------------------------------------------------------------
  * [Rainbow Paintbrush in p5.js](https://medium.com/@kellylougheed/rainbow-paintbrush-in-p5-js-e452d5540b25) by Kelly Lougheed

>> Added sketch
// https://editor.p5js.org/jht1493/sketches/9aYZcF6DM
// 2.5 Rainbow Paintbrush
  a_hue = (a_hue + 10) % 360;

// https://editor.p5js.org/jht1493/sketches/dojCKsdwQ
// 2.5 Rainbow Paintbrush ui

// https://editor.p5js.org/jht1493/sketches/TAnGTwIJ1
// 2.5.3 Rainbow Paintbrush a_step


-------------------------------------------------------------------------------
* The [map()](http://p5js.org/reference/#/p5/map) function
  * [video 2.4: map()](https://www.youtube.com/watch?v=nicMAoW6u1g&list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA&index=8)

https://thecodingtrain.com/beginners/p5js/2.4-map.html
https://www.youtube.com/watch?v=nicMAoW6u1g
2.5: The map() Function - p5.js Tutorial
220,353 views•Sep 4, 2015

https://editor.p5js.org/codingtrain/sketches/yJqbGf71
p5js Code! - map function

!!@----------------------------------------------------
02.5 animation 
  function and objects for multiple motino
  functions with tranlates to draw complex shapes
  variables can store color
  variables can store functions


-------------------------------------------------------------------------------
* Tutorial: [Recode Catalog by John Whitney](https://github.com/itpresidents/icm-help-sessions-2020/blob/master/session-02/session-02.md)

-------------------------------------------------------------------------------
## Tutorials: Transformations
  * [video 9.1: `translate()`, `rotate()`, `push()`, `pop()`](https://youtu.be/o9sgjuh-CBM)

https://thecodingtrain.com/Tutorials/9-additional-topics/9.1-transformations-part-1.html

https://www.youtube.com/watch?v=o9sgjuh-CBM
9.1: Transformations Pt.1 (Translate, Rotate, Push/Pop) - p5.js Tutorial
114,330 views•Sep 18, 2017
22 mins

>> angles
>> radians
>> negative numbers to reverse translate/rotate

let angle = 0;
angle = angle + 1;

>> push / pop

-------------------------------------------------------------------------------

  * [video 9.2: `scale()`](https://youtu.be/pkHZTWOoTLM)

https://thecodingtrain.com/Tutorials/9-additional-topics/9.2-transformations-part-2.html

https://www.youtube.com/watch?v=pkHZTWOoTLM&t=19s
9.2: Transformations Pt.2 (Scale) - p5.js Tutorial
27,812 views•Sep 19, 2017
8 mins
!!@ -- no sketch

>> scale(-1,-1) -- flips coord. to flip image left-right
>> scale affect stroke

>> intro arithmatic
  mouseX/4

>> matrix
2 0 0 
0 2 0

-------------------------------------------------------------------------------
  * [video 9.3: More on transformations](https://youtu.be/IVMvq9rd8dA)

https://thecodingtrain.com/Tutorials/9-additional-topics/9.3-transformations-art-3.html

!!@ push pop already discussed

>> push / pop -- save style

https://www.youtube.com/watch?v=IVMvq9rd8dA
9.3: Transformations Pt.3 - p5.js Tutorial
18,490 views•Sep 19, 2017
11 mins

-- STACK -- push / pop -- LIFO
-- QUEUE


-------------------------------------------------------------------------------

## p5.js editor examples
  * [random painting](
https://editor.p5js.org/icm/sketches/HJg8jfcT3

https://editor.p5js.org/jht1493/sketches/sUEajcpKC
2. Random Painting noStroke
>> !!@ try: cycle circle size
>> !!@ try: lower alpha
>> !!@ try: cycle alpha
>> !!@ try: othe shapes

  * [mouse controlled painting](
https://editor.p5js.org/icm/sketches/r1JeQqa3

  * [moving circle](
https://editor.p5js.org/icm/sketches/Bymv7ca2
>> Try: use mousePressed function to set new color and x, y to mouseX, mouseY
// https://editor.p5js.org/jht1493/sketches/QfgP2VgJt
// 2.9 moving circle random set

// https://editor.p5js.org/jht1493/sketches/IiHPr9gcV
// 2.9 moving circle

  * [clock](https://editor.p5js.org/icm/sketches/ryYueiWu7) -- [Clock coding challenge video](https://youtu.be/E4RyStef-gY)

-------------------------------------------------------------------------------
## Getting Started with p5.js book
  * Chapters 4 through Ex.4.5, 8 through Ex. 8.9

Example 4-4: Basic Arithmetic
// https://editor.p5js.org/jht1493/sketches/Eg01Z5WpY
// Ex_04_04 Basic Arithmetic


// https://editor.p5js.org/jht1493/sketches/DJ99paBR7
// Ex_08_03 Move a Shape
https://github.com/lmccart/gswp5.js-code/blob/master/08_Motion/Ex_08_03.js
#- Example 8-3: Move a Shape
var radius = 40;
var x = -radius;
var speed = 0.5;
function draw() {
  background(0);
  x += speed;  // Increase the value of x
  arc(x, 60, radius, radius, 0.52, 5.76);
}

// https://editor.p5js.org/jht1493/sketches/W_nCg2LI2
// Ex_08_04 Wrap Around
#- Example 8-4: Wrap Around
  x += speed;  // Increase the value of x
  if (x > width+radius) {  // If the shape is off screen
    x = -radius;  // move to the left edge
  }
  arc(x, 60, radius, radius, 0.52, 5.76);

#- Example 8-9: Move Shapes Randomly
function draw() {
  x += random(-speed, speed);
  y += random(-speed, speed);
  x = constrain(x, 0, width);
  y = constrain(y, 0, height); 
  ellipse(x, y, diameter, diameter);
}

https://p5js.org/reference/#/p5/constrain
constrain(n, low, high)


  * Going further: Chapters 6 (Transformations) and 8.10-8.15 (More complex motion)
  * [Getting Started with p5.js book](http://amzn.to/2ckixCW) | [Ebook (free with NYU Library login)](https://ebookcentral.proquest.com/lib/nyulibrary-ebooks/detail.action?docID=4333728) | [Code](
    https://github.com/lmccart/gswp5.js-code
    )

!!@----------------------------------------------------

https://editor.p5js.org/jht1493/sketches/1HRbbpwEK
createButton draw_rect
>> basic buttons. apply to variables

>> buttons to clear and draw
  draw with diferent loc and color

>> intro to DOM from the function point of view
>> minial muse of variables

!!@----------------------------------------------------
!!@ no-no, circleX goes negative
>> Try: add variable to use for step
>> add button to set a_step to 1, and -1 (negative 1)
let a_step = 1;
  circleX = (circleX + a_step) % width;
// https://editor.p5js.org/jht1493/sketches/HtESWWNTa
// 2.2 variable circleX remainder
>> use remainder operator % to restrict value to 0 ... n
>> introduce a_diam user variable
let circleX = 0;
let circleY = 80;
let a_diam = 100;
  circle(circleX, circleY, a_diam);
  circleX = (circleX + 1) % width;
>> add ui to show circleX
>> add button to grow 0, grow 1

!!@----------------------------------------------------
!!@ use objects and function args for multiple shapes
!!@ composition
!!@ frameRate(1) to slowdown
!!@ propose pulse - tease conditions
!!@ intro sliders

https://editor.p5js.org/codingtrain/sketches/ehbMJ-otC
p5js Code! - 2.2 - make your own variable - growing circle exercise

// https://editor.p5js.org/jht1493/sketches/P9xSA4D7d
// 2.2 - make your own variable - growing circle remainder

// https://editor.p5js.org/jht1493/sketches/T8BbkINop
// 2.2 button slider ui remainder
>> related to:
https://editor.p5js.org/jht1493/sketches/tuC5MB4nm
3.1 button slider checkbox ui if

// https://editor.p5js.org/jht1493/sketches/vig9Wkf9V
// 2.2 variable remainder erase
>> lots of buttons
