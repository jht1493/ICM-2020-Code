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
  * [Code Comments Video Tutorial](https://youtu.be/xJcrPJuem5Q)

  * `setup()` and `draw()` --remove--
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


[] only use setup
[] draw only need when state change
