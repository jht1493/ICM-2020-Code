# ICM-Code-2020

# Javascript Objects

-------------------------------------------------------------------------------
https://thecodingtrain.com/beginners/p5js/2.3-objects.html
!!@ Dead link

https://www.youtube.com/watch?v=-e5h4IGKZRY   
2.3: JavaScript Objects - p5.js Tutorial
190,360 views•Sep 4, 2015
!!@ In homework but not here

https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics   

>> dropped !!@
https://github.com/Codingrainbow/Rainbow-Code/blob/master/p5.js/2.3_1_p5.js_JavaScript_with_objects%20/sketch.js

// https://editor.p5js.org/jht1493/sketches/h-rLRPdqn   
// 2.2_p5.js user_defined

// https://editor.p5js.org/jht1493/sketches/qsfTfkb_5   
// 2.3_1_p5 with_objects

// https://editor.p5js.org/jht1493/sketches/gv8PmJE2u   
// 2.3_0_p5 without_objects


```
/Volumes/GSPOT/jht-g/projects/repo/ICM-2020-Code-forked/weeks/03_interaction.md
  9,18: * [3.2: Bouncing Ball - video tutorial](https://www.youtube.com/watch?v=LO3Awjn_gyU&list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA&index=11)
  10,15:   * [bouncing ball editor example](https://editor.p5js.org/icm/sketches/BJKWv5Tn)

/Volumes/GSPOT/jht-g/projects/repo/ICM-2020-Code-forked/weeks/05_functions.md
  8,15:   - [Bouncing ball with functions code example](https://editor.p5js.org/icm/sketches/H1Oq4qta)
!!@ With objects

/Volumes/GSPOT/jht-g/projects/repo/ICM-2020-Code-forked/weeks/06_objects.md
  9,16: * [Two Gravity Ball Objects code](https://editor.p5js.org/icm4.0/sketches/vshTFC6kU)

```

  * [video 2.4: random()](https://thecodingtrain.com/beginners/p5js/2.4-random.html) (~11 min)
  * [sketch - Random Square Design](https://editor.p5js.org/codingtrain/sketches/Sl8ml_Lz8)

// https://editor.p5js.org/jht1493/sketches/UTMOVgcsv   
// 2.5.1 obj object scan 

```
let a_scan = {
  x: 0,
  r: 0,
  alpha: 100,
  diam: 20
};

function draw() {
  // variables are set on the object a_scan
  a_scan.x = (a_scan.x + 1) % width;
  a_scan.y = random(0, height / 2);
  a_scan.r = (a_scan.r + 1) % 255;
  a_scan.g = random(100, 255);
  a_scan.b = random(100, 190);
  fill(a_scan.r, a_scan.g, a_scan.b, a_scan.alpha);
  ellipse(a_scan.x, a_scan.y, a_scan.diam);
}
```

// https://editor.p5js.org/jht1493/sketches/XzrXlqxMN   
// 2.5.1 obj random function scan x
```
  spot.x = (spot.x + 1) % width;
  spot.y = random(0, height);
```

// https://editor.p5js.org/jht1493/sketches/ny4aSEPTp   
// 2.5.1 random function scan x ran y
```
  spot.x = (spot.x + 1) % width;
  let h = height/8;
  spot.y = random([h, h*3, h*5, h*7]);
```

// https://editor.p5js.org/jht1493/sketches/vpcHXx_E1   
// 2.5.2 random function spot.count
```
  spot.count = spot.count + spot.d;
  spot.x = spot.count % width;
  spot.y = (int(spot.count / width) * spot.d) % height;
```

>> Try: have scan bottom to top, right to left

// https://editor.p5js.org/jht1493/sketches/A1NHTo3cg   
// 2.5.2 random function spot.count ui bottom
```
  spot.count = spot.count + spot.d;
  spot.x = width - (spot.count % width);
  spot.y = height - ((int(spot.count / width) * spot.d) % height);
```

