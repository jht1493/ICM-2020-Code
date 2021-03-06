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
  
  * [Code Comments Video Tutorial](https://youtu.be/xJcrPJuem5Q)
    1.6: Code Comments - p5.js Tutorial 76,543 views•Sep 11, 2018
    06:13
    command-slash
    credit

  - The Coding Train videos [Originals](https://github.com/CodingRainbow/Rainbow-Code/tree/master/p5.js) | [2020 Updates](https://editor.p5js.org/jht1493/collections/2R1Sx-_K0n)
  https://github.com/CodingRainbow/Rainbow-Code/tree/master/p5.js
  https://editor.p5js.org/jht1493/collections/2R1Sx-_K0n


  - _Getting Started with p5.js_ [Originals](https://github.com/lmccart/gswp5.js-code) | [2020 Updates](https://editor.p5js.org/jht1493/collections/P5w9v1xsq)
  https://github.com/lmccart/gswp5.js-code
  https://editor.p5js.org/jht1493/collections/P5w9v1xsq

  * `setup()` and `draw()` --remove--
  * [p5.js reference](http://p5js.org/reference)

## Getting Started with p5.js book
  *  Chapter 1-3 of [Getting Started with p5.js book](http://amzn.to/2ckixCW) | [NYU Library Ebook (free, must be on campus to access)](https://ebookcentral.proquest.com/lib/nyulibrary-ebooks/detail.action?docID=4333728) | [Code](https://github.com/lmccart/gswp5.js-code)
  by Lauren McCarthy, Casey Reas, and Ben Fry
  Copyright © 2016 Maker Media. All rights reserved.

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
  triangle(158, 55, 290, 91, 290, 112);

  rect(180, 60, 220, 40);

  ellipse(278, -100, 400, 400);
  ellipse(120, 100, 110, 110);
  ellipse(412, 60, 18, 18);

  arc(90, 60, 80, 80, 0, HALF_PI);
  arc(190, 60, 80, 80, 0, PI+HALF_PI);
  arc(290, 60, 80, 80, PI, TWO_PI+HALF_PI);
  arc(390, 60, 80, 80, QUARTER_PI, PI+QUARTER_PI);

  arc(90, 60, 80, 80, 0, radians(90)); 
  arc(190, 60, 80, 80, 0, radians(270));
  arc(290, 60, 80, 80, radians(180), radians(450));
  arc(390, 60, 80, 80, radians(45), radians(225));

  angleMode(DEGREES);
  arc(90, 60, 80, 80, 0, 90);
  arc(190, 60, 80, 80, 0, 270);
  arc(290, 60, 80, 80, 180, 450);
  arc(390, 60, 80, 80, 45, 225);

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

beginShape(); vertex(180, 82); vertex(207, 36); vertex(214, 63); vertex(407, 11); vertex(412, 30); vertex(219, 82); vertex(226, 109); endShape();

Comments



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


[] only use setup
[] draw only need when state change
