# Introduction
https://github.com/jht1493/ICM-2020-Code/blob/master/weeks/01_intro.md
https://github.com/jht1493/ICM-2020-Code/blob/master/weeks/01_intro-aa.md

-- overview
https://thecodingtrain.com/beginners/p5js/

## Getting Started with p5.js book

// https://editor.p5js.org/jht1493/sketches/Cc8MICNun
// Ex_02_02 Make Circles


[] move wiki/inspiration to here
https://github.com/ITPNYU/ICM-2020-Code/wiki/Inspiration

  - [Allison Parrish'](https://creative-coding.decontextualize.com/) tutorial
https://creative-coding.decontextualize.com

https://thecodingtrain.com/beginners/git-and-github/

https://thecodingtrain.com/beginners/p5js/0.1-trailer.html
https://thecodingtrain.com/beginners/p5js/1.1-introduction.html
https://thecodingtrain.com/beginners/p5js/1.2-p5js-web-editor.html
https://thecodingtrain.com/beginners/p5js/1.3-shapes-and-drawing.html
https://thecodingtrain.com/beginners/p5js/1.4-color.html
https://thecodingtrain.com/beginners/p5js/1.5-errors-and-console.html
https://thecodingtrain.com/beginners/p5js/1.6-code-comments.html

--------------------------------------------

++ scratch.mit.edu

!!@ https://github.com/CodingRainbow/Rainbow-Code
--> https://github.com/CodingTrain/website.git

/Volumes/GSPOT/jht-g/projects/repo/ICM-2020-Code-forked/weeks/07_dom.md
  6,27: * [Code for videos below](https://github.com/CodingTrain/website/tree/master/Tutorials/P5JS/p5.js/08)

https://github.com/CodingTrain/website/tree/main/beginners/p5js/
https://github.com/CodingTrain/website/tree/main/beginners/p5js/1.3-shapes-and-drawing/P5
https://github.com/CodingTrain/website/tree/main/beginners/p5js/1.4-color/P5

##  What is computational media?
  * What is programming?
  * How can I apply programming to _____________?
  * As a ____________, why would I want or need to write software?
  * [Example projects for Inspiration](https://github.com/ITPNYU/ICM-2020-Code/wiki/Inspiration)
  * Can programming be an expressive medium?
  * Why are we introducing programming through drawing?

## Programming language discussion
  * General discussion of programming languages
  * History of creative coding frameworks
      * [Processing](https://processing.org/) and [p5.js](https://p5js.org/) (and what's [processing.js](http://processingjs.org/)?)

      * [Introduction to Code with p5.js Video](https://youtu.be/yPWkPOfnGsw)
      1.1: Code! Programming for Beginners with p5.js 373,027 views•Sep 5, 2018
      13:10
      What is means to program?
      Algorithm
      Syntax
      HTML / CSS
      !!@ Community Statement -- BLM ++

      * [p5.js Web Editor Promo Video](https://youtu.be/dtHxDggkBYc)
      Announcing the p5.js Web Editor! 11,975 views•Aug 31, 2018
      02:49
      Diversity - Inclusion

      * [History of p5.js video](https://www.youtube.com/watch?v=FdsWWjqoPKU)
      Q&A #5: The History of p5.js and Processing 3,434 views•Sep 2, 2016
      24:59
      "Design by Numbers"
      Logo \ Hypercard \ Seymour Papert
      ?? API
      2013 "What if processing started over" -- Lauren McCathy
        -- sharability / simplicity
        -- port: openness - friently-ness - design - visual - art
      ++ DOM -- !!@ Lets use it!!
      ++ little p -- the issue: P5 with a capital P #1572
      --> community statement
      --> github code of conduct
      +++ diversity and inclusion

## Programming language discussion

    !!@ Drop to end
      * [openFrameworks](https://openframeworks.cc/), [Cinder](https://libcinder.org/)
      * [Max/MSP](https://cycling74.com/) [dataflow programming](https://en.wikipedia.org/wiki/Dataflow_programming)
      * How does [Arduino](https://www.arduino.cc/) fit in?

## p5.js in the context of the browser
  * Landscape of HTML, CSS, and JavaScript
  * Other JS frameworks
  * Server-side vs. client-side
  * What is the difference between p5 and JavaScript?

## Participating in an open-source community
  * What is git and github?
  * When should you post to a forum vs. file a github issue?
  * Who makes these things?

# Drawing
## Getting started, your first program

  * [p5.js Web Editor Tutorial](https://youtu.be/MXs1cOlidWs) 
    1.2: p5.js Web Editor - p5.js Tutorial 207,393 views•Sep 6, 2018 
    07:41
    https://editor.p5js.org/
    sharing
    auto named (cool)

  * [Shapes & Drawing video tutorial](https://youtu.be/c3TeLi6Ns1E).
    1.3: Shapes & Drawing - p5.js Tutorial 245,913 views•Sep 7, 2018 
    25:46

https://www.youtube.com/watch?v=c3TeLi6Ns1E
1.3: Shapes & Drawing - p5.js Tutorial
https://editor.p5js.org/codingtrain/sketches/HJ1WjEPwQ
p5js Code! - Shapes & Drawing

    calling functions syntax
    function_name(____, _____, ____);
    -- parameters / arguments (Dan S. calls in video)
    try and error editing numbers
    auto-refresh
    dots ==> pixels 
    JavaScript vs. p5 Library
    2D Primitives: 
      arc - 
      ellipse - line - point - quad - 
      rect - 
      triangle
    draw canvas --> you should do it too.
    cartesian coordinate system
    ** 0-based. coordinates are edges not pixels **
    >> make your own drawing
    DOC: optional args
    layering - order of lines of code
    attributes: rectMode, ellipseMode 
    ** disagree: intro translate and take more about functions **

  * [Color video tutorial](https://youtu.be/riiJTF5-N7c)
    1.4: Color - p5.js Tutorial 143,970 views•Sep 10, 2018
    17:25

https://www.youtube.com/watch?v=riiJTF5-N7c
1.4: Color - p5.js Tutorial
https://editor.p5js.org/codingtrain/sketches/rJ9MQSwvm
p5js Code! - Color

  fill(255, 0, 0, 175); // alpha = 175

    [ ] link error Oscillation Nature of Code Sketch
        https://editor.p5js.org/codingtrain/sketches/SJPtYPPOl
        -- correction:
          https://editor.p5js.org/natureofcode/sketches/SJPtYPPOl
    https://editor.p5js.org/codingtrain/sketches/rJ9MQSwvm
      -- demo of alpha
    p5js Code! - Color
    Red-Green-Blue
    background(200) -- gray
    background(___, ___, ___)
    HW: in reference Color/Settings
      + background()
      + stroke()
      + fill()
      + noFill()
      + noStroke()
      clear()
      colorMode()
      ++ erase() !!@
      ++ noErase() !!@
    Shape / Attributes
      ++ strokeWeight
      ++ alpha -- transparency

  * [Errors and Console Video Tutorial](https://youtu.be/LuGsp5KeJMM)
    1.5: Errors & Console - p5.js Tutorial  89,861 views•Sep 10, 2018
    06:36
    print("hello")
    error message
    >> use console.log() to show stuff pre-startup

  * [Code Comments Video Tutorial](https://youtu.be/xJcrPJuem5Q)
    1.6: Code Comments - p5.js Tutorial 76,543 views•Sep 11, 2018
    06:13
    command-slash
    credit

https://www.youtube.com/watch?v=xJcrPJuem5Q
1.6: Code Comments - p5.js Tutorial
https://editor.p5js.org/codingtrain/sketches/H1mj3SwD7
p5js Code! - Code Comments

  - The Coding Train videos [Originals](https://github.com/CodingRainbow/Rainbow-Code/tree/master/p5.js) 
  | [2020 Updates](https://editor.p5js.org/jht1493/collections/2R1Sx-_K0n)
  https://github.com/CodingRainbow/Rainbow-Code/tree/master/p5.js
  https://editor.p5js.org/jht1493/collections/2R1Sx-_K0n

>> Ref. from weeks/03_interaction.md
* Video Examples: [3.1-3.4](https://github.com/CodingRainbow/Rainbow-Code/tree/master/p5.js)

  !!@ See below

  - _Getting Started with p5.js_ [Originals](https://github.com/lmccart/gswp5.js-code) 
  | [2020 Updates](https://editor.p5js.org/jht1493/collections/P5w9v1xsq)
  https://github.com/lmccart/gswp5.js-code
  https://editor.p5js.org/jht1493/collections/P5w9v1xsq

  !!@ See below

## Getting Started with p5.js book
  *  Chapter 1-3 of [Getting Started with p5.js book](http://amzn.to/2ckixCW) | [NYU Library Ebook (free, must be on campus to access)](https://ebookcentral.proquest.com/lib/nyulibrary-ebooks/detail.action?docID=4333728) | [Code](https://github.com/lmccart/gswp5.js-code)
  by Lauren McCarthy, Casey Reas, and Ben Fry
  Copyright © 2016 Maker Media. All rights reserved.

https://github.com/lmccart/gswp5.js-code

https://github.com/lmccart/gswp5.js-code/tree/master/03_Draw
>> copy and paste into p5js editor

// https://editor.p5js.org/jht1493/sketches/Cc8MICNun
// Ex_02_02 Make Circles

1/Hello: Learn about p5.js.

2/Starting to Code: Create your first p5.js program.

function draw() {
  if (mouseIsPressed) {
    fill(0); 
  } else {
    fill(255); 
  }
  ellipse(mouseX, mouseY, 80, 80);

3/Draw: Define and draw simple shapes.

  line(20, 50, 420, 110);
  quad(158, 55, 199, 14, 392, 66, 351, 107);
  triangle(347, 54, 392, 9, 392, 66); 
  rect(180, 60, 220, 40);
  ellipse(278, -100, 400, 400);

Drawing Order

Shape Properties

strokeWeight(8); // Stroke weight to 8 pixels

Example 3-13: Set Stroke Attributes

strokeJoin(ROUND);  // Round the stroke corners
rect(40, 25, 70, 70); 
strokeJoin(BEVEL); 
rect(140, 25, 70, 70); 
strokeCap(SQUARE); 
line(270, 25, 340, 95); 
strokeCap(ROUND); 
line(350, 25, 420, 95);

Color

Example 3-15: Control Fill and Stroke

noFill(); // Turn off fill
noStroke(); // Turn off stroke

Example 3-16: Draw with Color

Example 3-17: Set Transparency

Custom Shapes

beginShape(); vertex(180, 82); vertex(207, 36); vertex(214, 63); vertex(407, 11); 
vertex(412, 30); vertex(219, 82); vertex(226, 109); 
endShape();

Comments

https://docs.google.com/document/d/1Qu7qf-E6PblFg8U3MvfP_xVeca9yT8Bt6mIsSYAxf0s/edit
JHT - Week 1 Worksheet


## p5.js
  * `setup()` and `draw()` --remove--
  * [p5.js reference](http://p5js.org/reference)

## Additional viewing / reading:
   * [Pick an Eyeo Talk that looks interesting](https://vimeo.com/eyeofestival/)
### More on p5
   * [All introductory p5.js videos](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA)
   * [Comparing Processing and p5.js Part 1 video](https://youtu.be/AmlAiKsiy0o), 
    [Comparing Processing and p5.js Part 2 video](https://youtu.be/AsjPJ5AWkDc), 
    [Comparing Processing and p5.js Part 3 video](https://youtu.be/_y8rEHjqzRA)
   * [Overview of p5.js Web Editor with Cassie](https://youtu.be/x1rJJRVTpAI)
### More on computational drawing
   * [FORM+CODE: Introduction and What is Code?](http://formandcode.com)
   * [Computational Color](http://printingcode.runemadsen.com/lecture-color/) | 
   [Long version: 4 chapters](https://programmingdesignsystems.com/color/a-short-history-of-color-theory/index.html)
   * [More about shapes (specifically "custom shapes" with vertices and bezier curves)](https://programmingdesignsystems.com/shape/custom-shapes/index.html#custom-shapes-pANLh0l)
   * [p5 playground](http://yining1023.github.io/p5PlayGround/)
### More on the Internets
   * [As We May Think](http://www.theatlantic.com/magazine/archive/1945/07/as-we-may-think/303881/), Vannevar Bush
   * [Long Live the Web](http://jblomo.github.io/webarch253/slides/Long_Live_the_Web.pdf), Tim Berners-Lee

[] ?? Use  Allison Parrish text 
  https://creative-coding.decontextualize.com/

[] ?? only use setup for static drawing

[] draw only need when state change

[] ?? go back to this model with example code in repo:
  https://github.com/ITPNYU/ICM-2015

[] inventory code examples
  - The Coding Train videos [Originals](https://github.com/CodingRainbow/Rainbow-Code/tree/master/p5.js) 
  | [2020 Updates](https://editor.p5js.org/jht1493/collections/2R1Sx-_K0n)
  https://github.com/CodingRainbow/Rainbow-Code/tree/master/p5.js
https://editor.p5js.org/jht1493/collections/2R1Sx-_K0n
https://editor.p5js.org/jht1493/sketches/p4WOzDrgQ
1.1_p5.js basics_of_drawing
  createCanvas(400, 300);
  background(220, 0, 200);
  rect(10, 20, 100, 80);
https://editor.p5js.org/jht1493/sketches/K_1xNuX78
1.2 p5.js_Color
  ellipseMode(CENTER);
  rectMode(CENTER);
  ellipse(240, 115, 60, 60);
  fill(255, 0, 0); // Body
  fill(0, 0, 255);
  fill(0, 255, 0);
  line(230, 195, 220, 205);

  - _Getting Started with p5.js_ [Originals](https://github.com/lmccart/gswp5.js-code) 
  | [2020 Updates](https://editor.p5js.org/jht1493/collections/P5w9v1xsq)
  https://github.com/lmccart/gswp5.js-code
https://editor.p5js.org/jht1493/collections/P5w9v1xsq
https://editor.p5js.org/jht1493/sketches/1jYHAXZRF
gswp5 Ex_02_01.js

https://editor.p5js.org/jht1493/sketches/un2SAKRVm
gswp5 Ex_02_02.js
  if (mouseIsPressed) {
    fill(0);
  } else {
    fill(255);
  }

https://editor.p5js.org/jht1493/sketches/4ru5A30iE
gswp5 Ex_03_04 quad tri

https://editor.p5js.org/jht1493/sketches/R0o3EvVOC
gswp5 Ex_03_06 circles touch

https://editor.p5js.org/jht1493/sketches/lj5UimD1G
gswp5 Ex_03_09 arcs

https://editor.p5js.org/jht1493/sketches/sxI2SjRrh
gswp5 Ex_03_17 alpha circles

https://editor.p5js.org/jht1493/sketches/xFElx4UBj
gswp5 Ex_03_19 beginShape

https://editor.p5js.org/jht1493/sketches/mPX1b9278
gswp5 Ex_03_20 Two Creatures

https://editor.p5js.org/jht1493/sketches/0EzMYSpky
gswp5 Ex_03 Robot 1: Draw


https://github.com/lmccart/gswp5.js-code/tree/master/03_Draw
>> copy and paste into p5js editor

>> x,y coordinates

>> p5 functions and parameters

>> example functions
  create_ui
  update_ui
  draw_head



https://editor.p5js.org/jht1493/sketches/a7_6dOQ-t
head color growth start
>> mouseX as parameter
>> num+mouseX

>> color rep.
  'white',
  255
  [255,255,255]

>> r,g,b,alpha
  [255,255,255,100]

>> Layering of drawing

>> flow of control

>> starting fresh with background() vs. building up 

https://editor.p5js.org/jht1493/sketches/sNH4P8QEp
head circle 100
  translate(100,0);
  draw_head();
>> flow of execution inside a function
>> translate affects next drawing
>> need to understand number line for translate(-100)
>> fill affects next drawing

https://editor.p5js.org/jht1493/sketches/HC9y3joDz
head circle
>> add scale and translate to draw many heads

https://editor.p5js.org/jht1493/sketches/K_1xNuX78
1.2 p5.js_Color
>> group draw calls into function and create a row of robots

>> recommend using graphing paper
>> copy and paste refs from doc

>> first hw already using other constructs
  extraCanvas = createGraphics(600, 400);
  extraCanvas.clear();
  extraCanvas.ellipse(mouseX, mouseY, 50, 50)
  image(extraCanvas, 0, 0)

>> color as array [], can be before setup

https://bmoren.github.io/p5js-cheat-sheet/


-------------------------------------------------------------------------------

## Ex 1.3 sketch draw_bars 

In this exercise we'll define a few other functions
to explore the p5js canvas coordinate system, shapes, and color.

Open this sketch in a separate window so that you can play it and read this page at the same time.
[sketch - draw_bars](https://editor.p5js.org/jht1493/sketches/Tiu0zz1NE)

As you move the mouse around on the canvas you should see 
the mouse location and a color value displayed below the canvas:
For example:
```
[mouseX=200] [mouseY=188] [RGBA=220,220,220,255]
```
The color value is reported as RGBA (Red,Green,Blue and Alpha) numbers between 0 and 255.
This is the color at the mouse location on the canvas.
Move the mouse around and explore these values.

Looking at the script you'll see functions *draw_bars*, *create_ui*, and *update_ui*.
Don't worry about the mechanics of *create_ui* and *update_ui*, 
we'll get into more detail about them in up comming sessions.
!!@ Explain later on this page

- function name draw_bars chosen to be generic

Let's look at the definition of function *draw_bars*:

!!@ print('in function draw_bars xpos=', xpos, 'ypos', ypos);
!!@ Use tranlate out side func to avoid args until later

```
function draw_bars(xpos, ypos) {
  // translate(x, y)
  translate(xpos,ypos)
  // rect(x, y, w, h)
  rect(20, 0, 20, 20);     
  rect(0, 20, 60, 20);     
  rect(20, 40, 20, 20);     
  translate(-xpos,-ypos)
}
...
```

Unlike the functions we've seen so far, 
*draw_bars* is not part of p5js library.
The function *draw_bars* and it's definition is written for this exercise.
The name is choosen to be descriptive of what it's supposed to do.
You are encouraged to write functions to break up your code into meaningful units.
In this illustration we are writing our own function to demonstrate creating an image by repeating a smaller image.

Examine the line: *function draw_bars(xpos, ypos)* 
This begins the definition of *draw_bars*.
The terms xpos and ypos are called parameter variables.
They will be assigned specific values when *draw_bars* is called,
in this case from the *draw* function.
The first call to function *draw_bars* assigns values 5 for xpos and 60 ypos.
The second call to function *draw_bars* assigns values 70 for xpos and 60 ypos.
```
function draw() {
  background(220);
  draw_bars(5, 60);
  draw_bars(70, 60);
  ...
```
In this case two shapes are drawn one starting at x,y location (5, 60)
and another at x,y location (70, 60).

Lookup the function *translate* in p5js reference and 
try to reason for yourself why two shapes are drawn at two different locations.


### Ex 1.3 explore sketch draw_bars

- Increase the size of the shape by adjusting appropriate values in the calls to *rect* in function *draw_bars* .

- In function *draw* add additional calls to *draw_bars* to draw shapes all the way across the canvas.

- Adjust the appearance of the shape. For example: add other shapes, or draw something different. 
You may call other p5js shape functions (*rect*, *triangle*, etc..) inside function *draw_bars*.

## Ex 1.4 sketch draw_bars color

Open this sketch in a separate window so that you can play it and read this page at the same time.
[sketch - draw_bars color](https://editor.p5js.org/jht1493/sketches/a3VD0HYqD)

This sketch draws the shapes in different colors.

In p5js a color can be represent in a number of ways.
Here are a few:

- color name, eg: 'white', 'black', 'red', 'green', 'yellow', 'blue'

- gray scale number, eg: 0 (white), 128 (gray), 255 (black)

- red, green, blue, alpha array, eg: [255,0,0,100] is full red with medium alpha setting.

function *draw_bars* now has an additional parameter variable, *acolor*:
```
function draw_bars(xpos, ypos, acolor) {
  // fill(color)
  // fill([r,g,b,a])
  fill(acolor);
...
```

When called from function *draw*, a color name is given:
```
function draw() {
  background(220);
  draw_bars(5, 60, 'white');
  draw_bars(70, 60, 'gray');
...
```

When *draw_bars* is called the third parameter can be an valid p5js color value.
The first call to *draw_bars* gives a value of 'white' to parameter acolor for *draw_bars*.
The second call gives a value of 'yellow' to *draw_bars*.

Lookup the function *fill* and function *color* for other color possibilities.

### Ex 1.4 explore draw_bars color

- using different types of color values. 
for example, try the color name 'green', compared it to the rgb representation [0,255,0]

- increase the size of the shape so they overlap and inspect the color of overlapping shapes

## Ex 1.5 sketch draw_bars alpha

Open this sketch in a separate window so that you can play it and read this page at the same time.
[sketch draw_bars alpha](https://editor.p5js.org/jht1493/sketches/3aQA0hvkt)

This sketch uses the format [Red,Green,Blue,Alpha] for colors. 

```
function draw() {
  background(220);
  draw_bars(5, 60, [255,255,255,100]);
  draw_bars(70, 60, [255,255,0,100]);
...
```

### Ex 1.5 explore draw_bars alpha

- increase the size of the shape so they overlap and inspect the color of overlapping shapes

- try different values of alpha for colors

## Ex 1.6 Free range draw_bars

Here are some variations on the sketch draw_bars.
Go forth and explore!

[sketch draw_fem rotate](https://editor.p5js.org/jht1493/sketches/R2Rdoodqo)

[sketch draw_fem mon](https://editor.p5js.org/jht1493/sketches/I7OFtFR8K)

[sketch draw_fem mon row](https://editor.p5js.org/jht1493/sketches/9Cy8EX8iO)

[sketch draw_fem matrix](https://editor.p5js.org/jht1493/sketches/BPBunRg2H)
