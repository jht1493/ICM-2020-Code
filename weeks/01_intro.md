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

# 1. Recap, Extensions, and Explorations

Let's recap, look at some extentions, do some exercises to futher explore the concepts introduced in this session.

## Ex 1.1 sketch draw_shapes 

So far our sketches defined two specially named functions *setup* and *draw*.
The function *setup* is called once when we hit the play button,
and the function *draw* is called repeatedly until we hit the stop button.
Also we haved used functions defined by the p5js library,
like *ellipse* and *rect*, to draw shapes on the canvas.

In this exercise well explore 
- how to create buttons to trigger our own events in a sketch
- how to define our own function
- the behavior of alpha settings for colors.

Open this sketch and play it.
[sketch - draw_shapes](https://editor.p5js.org/jht1493/sketches/qEgdTdx0K)

In this sketch in the function *draw* the call to the p5js function *background* is commented out.
Since the background color is not explicitly set it will start out as white.

Let's look at the definition of function *draw_shapes*:

```
function draw_shapes() {
  // fill(red, green, blue, alpha)
  fill(255, 0, 0, 20)
  rect(0, 100, 200, 200);
  // fill([red, green, blue, alpha])
  fill([255, 0, 255, 20])
  circle(200, 200, 200)
  // Green
  fill([0, 255, 0, 20])
  rect(200, 100, 200, 200);
}
```

Unlike the functions we've seen so far, 
*draw_shapes* is not part of p5js library.
The function *draw_shapes* and it's definition is written for this exercise.
The name is choosen to be descriptive of what it's supposed to do.
You are encouraged to write functions to break up your code into meaningful units.

This sketch uses the [Red,Green,Blue,Alpha] format for colors. 
The values Red,Greed,Blue and Alpha are numbers between 0 and 255. 
The alpha value can range from 0 (no alpha, black color), to 255 (full value of the color components). 
An alpha value in between 0 and 255  will mix some of the background color with the fill color.  

- messages in console panel
- print vs. console.log (p5js vs. javascript)
- nameing rules for functions (and javascript variables)

## Ex 1.1 sketch draw_shapes questions

- What happens if you repeatedly click on button Shapes? Why?

- What happens if you click on buttons Rect or Circle after button Shapes? Why?

- What happens if you enable the call to p5js function background in function *draw*?

## Ex 1.1 explore sketch draw_shapes

- Add/change shapes drawn in draw_shapes

- Add other button to draw other shapes

## Ex 2.1 sketch draw_mon 

In this exercise we'll define a few other functions
to explore the p5js canvas coordinate system, shapes, and color.

Open this sketch and play it.
[sketch - draw_mon](https://editor.p5js.org/jht1493/sketches/Tiu0zz1NE)

As you move the mouse around on the canvas you should see 
the mouse location and a color value displayed below the canvas:
For example:
```
[mouseX=200] [mouseY=188] [RGBA=220,220,220,255]
```
The color value is reported as RGBA (Red,Green,Blue and Alpha) numbers between 0 and 255.
This is the color at the mouse location on the canvas.
Move the mouse around and explore these values.

Looking at the script you'll see functions *draw_mon*, *create_ui*, and *update_ui*.
Don't worry about the mechanics of *create_ui* and *update_ui*, 
we'll get into more detail about them in up comming sessions.

- function name draw_mon chosen to be generic

Let's look at the definition of function *draw_mon*:

```
function draw_mon(xpos, ypos) {
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
*draw_mon* is not part of p5js library.
The function *draw_mon* and it's definition is written for this exercise.
The name is choosen to be descriptive of what it's supposed to do.
You are encouraged to write functions to break up your code into meaningful units.
In this illustration we are writing our own function to demonstrate creating an image by repeating a smaller image.

Examine the line: *function draw_mon(xpos, ypos)* 
This begins the definition of *draw_mon*.
The terms xpos and ypos are called parameter variables.
They will be assigned specific values when *draw_mon* is called,
in this case from the *draw* function.
The first call to function *draw_mon* assigns values 5 for xpos and 60 ypos.
The second call to function *draw_mon* assigns values 70 for xpos and 60 ypos.
```
function draw() {
  background(220);
  draw_mon(5, 60);
  draw_mon(70, 60);
  ...
```
In this case two shapes are drawn one starting at x,y location (10, 80)
and another at x,y location (60, 80).

Lookup the function *translate* in p5js reference and 
try to reason for yourself why two shapes are drawn at two different locations.

### Ex 2.1.1 sketch draw_mon questions

- When does the numbers change and when don't they change?

- What is the lowest value you see for the mouseX value?

- What is the largest value for mouseX?

- What value in the code will change the width of the canvas?

- What color value is reported for the background?

### Ex 2.1.2 explore sketch draw_mon

- Increase the size of the shape by adjusting appropriate values in the calls to *rect* in function *draw_mon* .

- In function *draw* add additional calls to *draw_mon* to draw shapes all the way across the canvas.

- Adjust the appearance of the shape. For example: add other shapes, or draw something different. 
You may call other p5js shape functions (*rect*, *triangle*, etc..) inside function *draw_mon*.

## Ex 2.2 sketch draw_mon color

Open this sketch and play it.
[sketch - draw_mon color](https://editor.p5js.org/jht1493/sketches/a3VD0HYqD)

This sketch draws the shapes in different colors.

In p5js a color can be represent in a number of ways.
Here are a few:

- color name, eg: 'white', 'black', 'red', 'green', 'yellow', 'blue'

- gray scale number, eg: 0 (white), 128 (gray), 255 (black)

- red, green, blue, alpha array, eg: [255,0,0,255]

function *draw_mon* now has an additional parameter variable, *acolor*:
```
function draw_mon(xpos, ypos, acolor) {
  // fill(color)
  // fill([r,g,b,a])
  fill(acolor);
...
```

When called from function *draw*, a color name is given:
```
function draw() {
  background(220);
  draw_mon(5, 60, 'white');
  draw_mon(70, 60, 'gray');
...
```

When *draw_mon* is called the third parameter can be an valid p5js color value.
The first call to *draw_mon* gives a value of 'white' to parameter acolor for *draw_mon*.
The second call gives a value of 'yellow' to *draw_mon*.

Lookup the function *fill* and function *color* for other color possibilities.

### Ex 2.2.1 explore draw_mon color

- using different types of color values. 
for example, try the color name 'green', compared it to the rgb representation [0,255,0]

- increase the size of the shape so they overlap and inspect the color of overlapping shapes

## Ex 2.3 sketch draw_mon alpha

Open this sketch and play it.
[sketch draw_mon alpha](https://editor.p5js.org/jht1493/sketches/3aQA0hvkt)

This sketch uses the format [Red,Green,Blue,Alpha] for colors. 

```
function draw() {
  background(220);
  draw_mon(5, 60, [255,255,255,100]);
  draw_mon(70, 60, [255,255,0,100]);
...
```

### Ex 2.3.1 explore draw_mon alpha

- increase the size of the shape so they overlap and inspect the color of overlapping shapes

- try different values of alpha for colors

## Ex 2.4 Free range draw_mon

Here are some variations on the function draw_mon.
Go forth and explore!

[sketch draw_fem rotate](https://editor.p5js.org/jht1493/sketches/R2Rdoodqo)

[sketch draw_fem mon](https://editor.p5js.org/jht1493/sketches/I7OFtFR8K)

[sketch draw_fem mon row](https://editor.p5js.org/jht1493/sketches/9Cy8EX8iO)

[sketch draw_fem matrix](https://editor.p5js.org/jht1493/sketches/BPBunRg2H)
