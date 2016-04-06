### What is p5js and why?
[P5js](https://p5js.org/) is a library created by Lauren McCarthy, and was inspired by the popular Processing language and software. This language was designed specificaly for artists, designers, educators and beginners. The idea behind it was to create a friendly way to introduce programming to these people so they will be able to do programming with a more artistic approach.

## Sketchbook Metaphor
The sketchbook metaphor is a way to break the wall between technology and art. Using concepts that are familiar makes us feel confortable and helps us grasp the concepts more quickly. You'll see that the way to write code in p5js follows the common language used by art makers. And when I say "Art Makers" I refer to all of us, because we have been making art since kindergarden.

### What should you know?
- html (basic)
- javascript (basic)

### Get started
- Download this repo

```
$ git clone this-repo.git
```
Open the repo with your favorite text editor. I recommend you to use the awesome [atom](www.atom.io) or [sublime](www.sublime.com) text editor.

For being able to loading images you need to run a web server, so install a simple node server in your global system.

```
$ npm install -g http-server
$ cd path/to/the/repo
$ http-server
```

### Setup your sketch file
Following the metaphor of the sketchbook, this is the basic setup for every one of the sketches we'll create. A *setup* function will contain the code for setting up our canvas and a *draw* function will contain the piece of art we are going to work on.

```javascript
function setup(){
  // this code runs just once

}

function draw(){
  // this code runs 60 frames per second (by default)

}
```

Now you can start experimenting!

### Code for our "Hello P5 World" sketch
With a few basic shapes we have created a simple heart that will be our entry point to this awesome library. Feel free to copy and paste this code and start experimenting.

```javascript
// this code run just once
function setup(){
  createCanvas(windowWidth, windowHeight);
  // the background method is accepting 3 valued (rgb colors) red green and blue
  background(111, 77, 255);
}

// this code run 60 times per second
function draw(){
  translate(width/2.5, height/2.5);
  noStroke();
  fill(255, 138, 140);

  // left circle of my heart
  ellipse(50, 50, 100, 100);

  // right circle of my heart
  ellipse(120, 50, 100, 100);

  // free style 4 side shape for completing our heart
  quad(20, 90, 85, 50, 150, 90, 85, 130);
}
```
