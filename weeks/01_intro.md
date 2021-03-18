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
  *  Chapter 1-3 of [Getting Started with p5.js book](http://amzn.to/2ckixCW) | 
  [NYU Library Ebook (free, must be on campus to access)](https://ebookcentral.proquest.com/lib/nyulibrary-ebooks/detail.action?docID=4333728) | 
  [Code](https://github.com/lmccart/gswp5.js-code)
  * 
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

# 1. Recap, Explore and Experiment

Let's recap, explore, and experiment with the concepts introduced in this session.

- draw a rough schematic what you've learned so far about p5js
- after you finish these exercises redraw with any new insights

So far our sketches defined two specially functions `setup` and `draw`.
The function `setup` is called once when we hit the play button,
and the function `draw` is called repeatedly until we hit the stop button.
Also we haved used functions defined by the p5js library,
like `ellipse` and `rect`, to draw shapes on the canvas.

In this exercises we'll explore 
- how to create buttons to run code
- how to use the print function to debug your code
- the behavior of alpha value for colors
- how to define your own function

For some of these sketches no drawing is done in the function `draw`.
When nothing is drawn the canvas will start out white.

## Ex 1.1 play sketch draw_rect

Open this sketch in a separate window so that you can play it and read this page at the same time.
[sketch - draw_rect](https://editor.p5js.org/jht1493/sketches/WJFtFBmnK)

- if your screen too small to allow viewing sketch and this page at the same time, 
use a print out this page as you explore the sketch.
- buttons will appear below canvas
- play the sketch, click on the buttons and note behavior

## Ex 1.1 explore sketch draw_rect

- did you notice that sometimes the left rect is white and other gray?

- what are possible ways to represent color for function fill ?

- try adjusting the colors specified in calls to function fill

- try adding function print to follow the behavior of the buttons

## Ex 1.1 explore sketch draw_rect_print

- print function added in the sketch

Open this sketch in a separate window so that you can play it and read this page at the same time.
[sketch - draw_rect_print](https://editor.p5js.org/jht1493/sketches/NlCr2UD2P)

In p5js a color can be represent in a number of ways.
Here are a few:

- color name, eg: 'white', 'black', 'red', 'green', 'yellow', 'blue'

- gray scale number, eg: 0 (white), 128 (gray), 255 (black)

- red, green, blue, alpha array, eg: [255,0,0,100] is full red with medium alpha setting.

- try setting different colors for each shape


## Ex 1.1 explore sketch draw_rect_alpha

- alpha colors added to the sketch

Open this sketch in a separate window so that you can play it and read this page at the same time.
[sketch - draw_rect_alpha](https://editor.p5js.org/jht1493/sketches/6mrwOv4RD)

This sketch uses the [Red,Green,Blue,Alpha] format for colors. 
The values Red, Green, Blue and Alpha are numbers between 0 and 255. 
The alpha value can range from 0 (no alpha, white color), to 255 (full value of the color components). 
For example, alpha value 127 will mix an even amount of the background color with the fill color.
Alpha value 20 will give a very light tint of the fill color on the background.

- try clicking each button repeatedly and observe the laying of the colors

- try every low values of alpha, eg. 10 and compare to medium alpha value 100

## Ex 1.1 explore sketch draw_rect_createSpan

In this exercise we'll define a few other functions
to explore the p5js canvas coordinate system, shapes, and color.

Open this sketch in a separate window so that you can play it and read this page at the same time.
[sketch - draw_rect_createSpan](https://editor.p5js.org/jht1493/sketches/C83N_DY9w)

## Ex 1.1 question sketch draw_rect_createSpan 

- When do the numbers change and when don't they change?

- What is the lowest value you see for the mouseX value?

- What is the largest value for mouseX?

- What value in the code will change the width of the canvas?

- What color value is reported for the background?

## Ex 1.2 explore sketch draw_shapes_body 

Open this sketch in a separate window so that you can play it and read this page at the same time.
[sketch - 1.2 draw_shapes_body](https://editor.p5js.org/jht1493/sketches/X5iRxm8HK)

Click on the buttons and observe the actions and the messages that appear in the console.
In the body of the mousePressed function you can call as many other functions as you wish.

- buttons Rect and Circle no color set

- button Shapes draws 3 shapes.
```
  createButton('Shapes').mousePressed(function() {
    print('drawing shapes');
    // fill([red, green, blue, alpha])
    fill([255, 0, 0, 20]); // Red, alpha 20
    rect(0, 100, 200, 200);
    // fill([red, green, blue, alpha])
    fill([255, 255, 0, 20]); // Yellow, alpha 20
    circle(200, 200, 200)
    // fill([red, green, blue, alpha])
    fill([0, 255, 0, 20]); // Green, alpha 20
    rect(200, 100, 200, 200);
  });
```

## Ex 1.2 explore sketch draw_shapes_func

Open this sketch in a separate window so that you can play it and read this page at the same time.
[sketch - 1.2 draw_shapes_func](https://editor.p5js.org/jht1493/sketches/qEgdTdx0K)

Click on the buttons and observe the actions and the messages that appear in the console.

Let's look at the definition of function draw_shapes:

```
function draw_shapes() {
  // fill([red, green, blue, alpha])
  fill([255, 0, 0, 20]); // Red
  rect(0, 100, 200, 200);
  // fill([red, green, blue, alpha])
  fill([255, 255, 0, 20]); // Yellow
  circle(200, 200, 200)
  // fill([red, green, blue, alpha])
  fill([0, 255, 0, 20]);  // Green
  rect(200, 100, 200, 200);
}
```

Unlike the functions we've seen so far, 
function `draw_shapes` is not part of p5js library.
function `draw_shapes` and it's definition is written for this exercise.
The name is choosen to be descriptive of what it's supposed to do.
You are encouraged to write functions to break up your code into meaningful units.

In this sketch function `draw_shapes` is called from the button 'Shapes' defined in the function setup:

```
function setup() {
  ...
  createButton('Shapes').mousePressed(function() {
    print('calling draw_shapes');
    draw_shapes();
  });
  ...
}
```

- Shapes button calls function draw_shapes, defined in script.
- You choose the name for your functions names to describe the intent of the code
- A function name must begin with a letter (upper or lower case), 
followed by any number of letters, numbers or underscore characters.

## Ex 1.2 question sketch draw_shapes_func

- What happens if you repeatedly click on button Shapes? Why?

- What happens if you click on buttons Rect or Circle after button Shapes? Why?

## Ex 1.2 extend sketch draw_shapes_func

- Add/change shapes drawn in function draw_shapes

- Add other buttons to draw other shapes

## Ex 1.2 explore sketch draw_shapes_ui

Open this sketch in a separate window so that you can play it and read this page at the same time.
[sketch - 1.2 draw_shapes_ui](https://editor.p5js.org/jht1493/sketches/DGQoBYV9x)

- added function create_ui and function update_ui 
- uses code from previous sketch to display mouse location and canvas color

## DOM functions createButton, createSpan, select

- for those curious about DOM functions
- ok to skip this section
- DOM functions createButton, createSpan, select
- DOM means Document Object Model, how the browser refers to visual elements on the page.
- function createButton creates a button element on the page
- function createSpan creates span of text, spans are layed out on a line.
- elements may be assigned an id later used to reference them
- function select is used to referred to an element by it's id
- an id is descriptive text you make up

- in future sessions we'll see how to adjust layout of buttons and other DOM elements

- to make a button
- - copy paste code for **createButton**  
- - change title and body

```
function setup() {
  createCanvas(400, 300);
  // createButton('title-for-button-')...
  createButton('backg 240').mousePressed(function() {
    // Code to run when button pressed, the "body"
    background(240);
  }); // End of createButton
...
```

- to display a value
- - copy paste code for **createSpan** and **select**
- - replace id and parameter to html

```
  // setup code
  // first parameter 'mox' is id for span
  // replace with your string
  createSpan().id('mox');

  // draw code
  // replace string mox with id
  // first parameter '#mox' is id for span
  // note: # character needed
  select('#mox').html('[mouseX='+mouseX+'] ')
```
