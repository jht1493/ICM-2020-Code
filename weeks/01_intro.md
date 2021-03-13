# Introduction

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
      * [p5.js Web Editor Promo Video](https://youtu.be/dtHxDggkBYc)
      * [History of p5.js video](https://www.youtube.com/watch?v=FdsWWjqoPKU)
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
  * [Shapes & Drawing video tutorial](https://youtu.be/c3TeLi6Ns1E)
  * [Color video tutorial](https://youtu.be/riiJTF5-N7c)
  * [Errors and Console Video Tutorial](https://youtu.be/LuGsp5KeJMM)
  * [Code Comments Video Tutorial](https://youtu.be/xJcrPJuem5Q)
  * `setup()` and `draw()`
  * [p5.js reference](http://p5js.org/reference)

## Getting Started with p5.js book
  *  Chapter 1-3 of [Getting Started with p5.js book](http://amzn.to/2ckixCW) | [NYU Library Ebook (free, must be on campus to access)](https://ebookcentral.proquest.com/lib/nyulibrary-ebooks/detail.action?docID=4333728) | [Code](https://github.com/lmccart/gswp5.js-code)

## Additional viewing / reading:
   * [Pick an Eyeo Talk that looks interesting](https://vimeo.com/eyeofestival/)
### More on p5
   * [All introductory p5.js videos](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA)
   * [Comparing Processing and p5.js Part 1 video](https://youtu.be/AmlAiKsiy0o), [Comparing Processing and p5.js Part 2 video](https://youtu.be/AsjPJ5AWkDc), [Comparing Processing and p5.js Part 3 video](https://youtu.be/_y8rEHjqzRA)
   * [Overview of p5.js Web Editor with Cassie](https://youtu.be/x1rJJRVTpAI)
### More on computational drawing
   * [FORM+CODE: Introduction and What is Code?](http://formandcode.com)
   * [Computational Color](http://printingcode.runemadsen.com/lecture-color/) | [Long version: 4 chapters](https://programmingdesignsystems.com/color/a-short-history-of-color-theory/index.html)
   * [More about shapes (specifically "custom shapes" with vertices and bezier curves)](https://programmingdesignsystems.com/shape/custom-shapes/index.html#custom-shapes-pANLh0l)
   * [p5 playground](http://yining1023.github.io/p5PlayGround/)
### More on the Internets
   * [As We May Think](http://www.theatlantic.com/magazine/archive/1945/07/as-we-may-think/303881/), Vannevar Bush
   * [Long Live the Web](http://jblomo.github.io/webarch253/slides/Long_Live_the_Web.pdf), Tim Berners-Lee

# 1. Recap and Explorations

Here is a recap and some exercises to futher explore the concepts introduced in this session.

## Ex 1.1 sketch function draw_head 

So far have used two specially named functions *setup* and *draw*.
The function *setup* is called once when we hit the play button,
and the function *draw* is called repeatedly until we hit the stop button.
Also we haved used functions defined by the p5js library,
like *ellipse* and *rect*, to draw shapes on the canvas.

In this exercise we'll define a few other functions
to explore the p5js canvas coordinate system, shapes, and color.

Open this sketch and play it.
[sketch - function draw_head](https://editor.p5js.org/jht1493/sketches/Tiu0zz1NE)

As you move the mouse around on the canvas you should see 
the mouse location and a color value displayed below the canvas:
For example:
```
[mouseX=200] [mouseY=188] [RGBA=220,220,220,255]
```
The color value is reported as RGBA (Red,Green,Blue and Alpha) numbers between 0 and 255.
This is the color at the mouse location on the canvas.
Move the mouse around and explore these values.

### Ex 1.1.1 Some questions to consider:

- When does the numbers change and when don't they change?

- What is the lowest value you see for the mouseX value?

- What is the largest value for mouseX?

- What value in the code will change the width of the canvas?

- What color value is reported for the background?

Looking at the script you'll see functions *draw_head*, *create_ui*, and *update_ui*.
Don't worry about the mechanics of *create_ui* and *update_ui*, 
we'll get into more detail about them in up comng sessions.

Let's look at the definition of function *draw_head*:

```
function draw_head(xpos, ypos) {
  translate(xpos,ypos)
  // ellipse(x, y, w, [h])
  ellipse(20, 20, 40);     // Face
  ellipse(10, 16, 10);     // Left Eye
  ellipse(30, 16, 10);     // Right Eye
  ellipse(20, 30, 20, 8);  // Mouth
...
```

Unlike the functions we've seen so far, 
*draw_head* is not part of p5js library.
The function *draw_head* and it's definition is written for this exercise.
The name is choosen to be descriptive of what it's supposed to do.
You are encouraged to write functions to break up your code into meaningful units.
In this illustration we are writing our own function to demonstrate creating an image by repeating a smaller image.

Examine the line: *function draw_head(xpos, ypos)* 
This begins the definition of *draw_head*.
The terms xpos and ypos are called parameter variables.
They will be assigned specific values when *draw_head* is called,
in this case from the *draw* function.
The first call to function *draw_head* assigns values 10 for xpos and 80 ypos.
The second call to function *draw_head* assigns values 60 for xpos and 80 ypos.
```
function draw() {
  background(220);
  draw_head(10, 80);
  draw_head(60, 80);
  ...
```
In this case two heads are drawn one starting at x,y location (10, 80)
and another at x,y location (60, 80).

Lookup the function *translate* in p5js reference and 
try to reason for yourself why two heads are drawn at two different locations.

### Ex 1.1.2 Adjustment to the sketch to explore:

- Increase the size of the head by adjusting appropriate values in the calls to *ellipse* in function *draw_head* .

- In function *draw* add additional calls to *draw_head* to draw heads all the way across the canvas.

- Adjust the appearance of the head. For example: add ears to the head, add an entire body, or draw something different. You may call other p5js shape functions (*rect*, *triangle*, etc..) inside function *draw_head*.

## Ex 1.2 sketch function draw_head color

Open this sketch and play it.
[sketch - function draw_head color](https://editor.p5js.org/jht1493/sketches/a7_6dOQ-t)

This sketch draws the heads in different colors.

In p5js a color can be represent in a number of ways.
Here are a few:

- color name, eg: 'white', 'black', 'red', 'green', 'yellow', 'blue'

- gray scale number, eg: 0 (white), 128 (gray), 255 (black)

- red, green, blue, alpha array, eg: [255,0,0,255]

This sketch draws the head in different colors.

function *draw_head* now has had additional parameter variable, *acolor*:
```
function draw_head(xpos, ypos, acolor) {
  translate(xpos,ypos)
  fill(acolor)
...
```

When called from function *draw*, a color name is given:
```
function draw() {
  background(220);
  draw_head(10, 20, 'white');
  draw_head(10, 80, 'yellow');
...
```

When *draw_head* is called the third parameter can be an valid p5js color value.
Lookup the function *fill* and function *color* for some possibilities.


### Ex 1.2.1 Adjustment to the sketch to explore:

- using different types of color values. for example, try the color name 'green', compared to the rgb representation [0,255,0]

- increase the size of the head so they overlap and inspect the color of overlapping shapes

## Ex 1.3 sketch function draw_head alpha

Open this sketch and play it.
[sketch function draw_head alpha](https://editor.p5js.org/jht1493/sketches/3aQA0hvkt)

This sketch uses the [Red,Green,Blue,Alpha] format for colors. The values Red,Greed,Blue and Alpha are numbers between 0 and 255. The alpha value can range from 0 (no alpha, black color), to 255 (full value of the color components). An alpha value in between 0 and 255  will mix some of the background color with the fill color.  An alpha value of 100 is used for the drawings. 

```
function draw() {
  background(220);
  draw_head(10, 20, [255,255,255,100]);
  draw_head(10, 80, [255,255,0,100]);
...
```

### Ex 1.3.1 Adjustment to the sketch to explore:

- increase the size of the head so they overlap and inspect the color of overlapping shapes



