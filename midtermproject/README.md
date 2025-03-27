# Midterm Project Documentation

click below for project:
[midtermproject](https://editor.p5js.org/sarnaqvi/sketches/5D4qUEOmn)

I started by using the code in lines 54 to 86 in the codealong.js file in the [05Functions](https://github.com/rdwrome/261sp25/blob/main/05Functions/codealong.js) subfolder in the 261sp25 repository. I started by uploading 11 mp3 files to p5.js, and then changed the code I had taken from the repository slightly. Here is the code from the repository...

`
let myFirstSound;

function preload() {
  soundFormats('wav', 'mp3');  
  myFirstSound = loadSound('00_ann.wav', soundLoaded);
}

function setup() {
  createCanvas(400, 200);
  textSize(20);
  textAlign(CENTER, CENTER);
  text("Move your cursor to the 'Preview' section\nPress 'P' to play sound", width / 2, height / 2);
}

function soundLoaded() {
  console.log("Sound successfully loaded!");
}

function keyPressed() {
  console.log("Key pressed:", key);
  if (key.toLowerCase() === 'p') {
    playCustomSound();
  }
}

function playCustomSound() {
  if (myFirstSound.isLoaded()) {
    myFirstSound.play();
    console.log("Sound played.");
  } else {
    console.log("Sound not loaded yet.");
  }
}
`

Instead of keeping the variable, myFirstSound, I used eleven new variables for each of the mp3 files I uploaded to [p5.js](https://editor.p5js.org/). My new variables were soundB, soundY, soundC, soundE, soundP, soundF, soundH, soundX, soundT, soundR, and soundV. I put these new variables in the let statement and then for the preload function, setup function, and keyPressed function. In the preload function, I copied the format of the code..

`
myFirstSound = loadSound('00_ann.wav', soundLoaded);
`

and copied this eleven times before replacing with my eleven new variables and the corresponding mp3 files. 

For the setup function, I changed the text to include my new variables which caused some of the text to be cut off since there were so many more variables used, resulting in more text that didn't fit on the canvas properly. To combat this, I increased the canvas size slightly so it would be 500x200 pixels. I used the [p5 reference](https://p5js.org/reference/p5/createCanvas/) to help me understand this.  

Next, I made some changes to the keyPressed function. Since there are multiple keys that need to be pressed that means that there are multiple conditions, and so, I refered to lines 30 to 37 in the [04ControlFlow](https://github.com/rdwrome/261sp25/blob/main/04ControlFlow/codealong.js) subfolder in the 261sp25 repository. Here is the code I referred to...

`
let thirdNote = 64;
if (thirdNote < 64) {
  console.log("MIDI note is smaller than 64.");
} else if (thirdNote > 64) {
  console.log("MIDI note is greater than 64.");
} else {
  console.log("MIDI note is exactly 64.");
}
`
First, I changed the original code for the key pressed function by typing the lowercase letters that corresponded with my new variables. I also made sure to write the new variables in the parentheses following playCustomSound since I'm using multiple sounds and need to specify which sound I am calling on my pressing the respective keys. Then, I just tested my code with the first three variables to see if modeling the if, else if, then else statement would work. Since, I just wanted to test these three sounds I deleted the other variables temporarily so I would only have soundB, soundY, and soundC. My code for the keyPressed function looked like the following...

`
function keyPressed() {
  console.log("Key pressed:", key);
  if (key.toLowerCase() === 'b') {
    playCustomSound(soundB);
  }else if (key.toLowerCase() === 'y') {
    playCustomSound(soundY);
  }else (key.toLowerCase() === 'c') {
    playCustomSound(soundC);
}
`
The code didn't run and then I realized I missed one last bracket at the end. After adding this, there was still a problem. The code wouldn't run because there was an issue with the playCustomSound function at the end. This was the code I originally had...

`
function playCustomSound() {
  if (myFirstSound.isLoaded()) {
    myFirstSound.play();
    console.log("Sound played.");
  } else {
    console.log("Sound not loaded yet.");
  }
}
`
I knew I had to change the variable myFirstSound, but I wasn't sure what I would need to change it to in order to account for all eleven of my sounds. After consulting a tutor, I learned that I needed one variable for all the sounds I wanted to use and use that to replace myFirstSound, but also I needed to define this new variable in the function by putting it in the paranthesis following playCustomSound. I changed my code to the following...

`
function playCustomSound(sound) {
  if (sound.isLoaded()) {
    sound.play();
    console.log("Sound played.");
  } else {
    console.log("Sound not loaded yet.");
  }
}
`
Then I went back to working on the keyPressed function. When I pressed b for soundB, the mp3 file was not being played independently- another audio file was playing too. I then thought to try omitting the last else statement so that everything besides the first if statement, was an else if statement. I thought this may work because I will have multiple conditions and I don't want to default to any key by using the else statement. After changing to only else if statement and the if statement, I tested the keys and they played each audio file independtly. Then, I re-added the other variables since I had finished testing with the first three variables. My function looked like the following...

`
function keyPressed() {
  console.log("Key pressed:", key);
  if (key.toLowerCase() === 'b') {
    playCustomSound(soundB);
  }else if (key.toLowerCase() === 'y') {
    playCustomSound(soundY);
  }else if (key.toLowerCase() === 'c') {
    playCustomSound(soundC);
  }else if (key.toLowerCase() === 'e') { 
    playCustomSound(soundE);
  }else if (key.toLowerCase() === 'p') { 
    playCustomSound(soundP);
  }else if (key.toLowerCase() === 'f') {
    playCustomSound(soundF);
  }else if (key.toLowerCase() === 'h') {
    playCustomSound(soundH);
  }else if (key.toLowerCase() === 'x') {
    playCustomSound(soundX);
  }else if (key.toLowerCase() === 't') {
    playCustomSound(soundT);
  }else if (key.toLowerCase() === 'r') {
    playCustomSound(soundR);
  }else if (key.toLowerCase() === 'v') {
    playCustomSound(soundV);
}
}
`

After these changes, my code worked and looked like the following...

`
let soundB, soundY, soundC, soundE, soundP, soundF, soundH, soundX, soundT, soundR, soundV;

function preload() {
  soundFormats('wav', 'mp3');  
  soundB = loadSound('Bag.mp3', soundLoaded);
  soundY = loadSound('BendFlute.mp3', soundLoaded);
  soundC = loadSound('Chords.mp3', soundLoaded);
  soundE = loadSound('EchoFlute.mp3', soundLoaded);
  soundP = loadSound('EndPro.mp3', soundLoaded);
  soundF = loadSound('FilterPro.mp3', soundLoaded);
  soundH = loadSound('HA.mp3', soundLoaded);
  soundX = loadSound('Playbox.mp3', soundLoaded);
  soundT = loadSound('PrettyPro.mp3', soundLoaded);
  soundR = loadSound('ReverbFlute.mp3', soundLoaded);
  soundV = loadSound('VitalInt.mp3', soundLoaded);
}

function setup() {
  createCanvas(500, 200);
  textSize(20);
  textAlign(CENTER, CENTER);
  text("Move your cursor to the 'Preview' section\nPress 'B, Y, C, E, P, F, H, X, T, R, or V' to play sounds", width / 2, height / 2);
}

function soundLoaded() {
  console.log("Sound successfully loaded!");
}

function keyPressed() {
  console.log("Key pressed:", key);
  if (key.toLowerCase() === 'b') {
    playCustomSound(soundB);
  }else if (key.toLowerCase() === 'y') {
    playCustomSound(soundY);
  }else if (key.toLowerCase() === 'c') {
    playCustomSound(soundC);
  }else if (key.toLowerCase() === 'e') { 
    playCustomSound(soundE);
  }else if (key.toLowerCase() === 'p') { 
    playCustomSound(soundP);
  }else if (key.toLowerCase() === 'f') {
    playCustomSound(soundF);
  }else if (key.toLowerCase() === 'h') {
    playCustomSound(soundH);
  }else if (key.toLowerCase() === 'x') {
    playCustomSound(soundX);
  }else if (key.toLowerCase() === 't') {
    playCustomSound(soundT);
  }else if (key.toLowerCase() === 'r') {
    playCustomSound(soundR);
  }else if (key.toLowerCase() === 'v') {
    playCustomSound(soundV);
}
}

function playCustomSound(sound) {
  if (sound.isLoaded()) {
    sound.play();
    console.log("Sound played.");
  } else {
    console.log("Sound not loaded yet.");
  }
}
`

## Experimentation and Failure with Playback Rate Changes
After meeting the requirements for the midterm project, I decided to try adding playback rate changes for at least one of the audio files. I used lines of code 43 to 50 from the [05Functions](https://github.com/rdwrome/261sp25/blob/main/05Functions/codealong.js) subfolder but replaced the variable myFirstSound with soundC in order to change the playback rate changes of the audio files with the chords playing. Here is what the code looked like...
`
function draw(){
  background(0);
  let mouseXNormalized = map (mouseX, 0, width, 0.5, 2.0);
  soundC.rate(mouseXNormalized);
  
  fill(255);
  text('rate: ' + mouseXNormalized.toFixed(2), 20,20);
}
`
Though the playback rate changed did work, the canvas for this blocked the text that had previously taken up the canvas. I also wanted to add more canvases for more playback rate changes for more audio files; however I struggled to make multiple apropriately sized canvases even after referring to the [p5 reference on multiple canvases](https://p5js.org/examples/advanced-canvas-rendering-multiple-canvases/). I was able to get two canvases so the text was no longer blocked by the playback rate changes canvas; however, now the issue was that the playback rate changes were no longer working and did not show the playback rate change in the upper left corner of the canvas. 


Here is the code from the p5 reference...

`
// Function for first canvas
function sketch1(p) {
  p.setup = function () {
    p.createCanvas(720, 200);
    p.background(0);
  };
  p.draw = function () {
    p.circle(p.mouseX, p.mouseY, 50);
  };
}

// Run first p5 instance
new p5(sketch1);

// Function for second canvas
function sketch2(p) {
  p.setup = function () {
    p.createCanvas(720, 200);
    p.background(255);
    p.fill(0);
    p.stroke(255);
  };
  p.draw = function () {
    p.square(p.mouseX, p.mouseY, 50);
  };
}

// Run second p5 instance
new p5(sketch2);
`

And here is how I tried to change it for two canvases, one with writing and one with playback rate change control. I just tried to keep one canvas  the same as the setup function lines of code for the text and then made the second canvas with the playback rate changes code from the 05 subfolder as previously shown..

`
function sketch1(p) {
  
  p.setup=function draw(){
  p.background(0);
  let mouseXNormalized = map (mouseX, 0, width, 0.5, 2.0);
  soundC.rate(mouseXNormalized);
  
  fill(255);
  text('rate: ' + mouseXNormalized.toFixed(2), 20,20);
};
  p.setup = function () {
    p.createCanvas(200, 200);
    p.background(0);
  };
 
}

// Run first p5 instance
new p5(sketch1);

// Function for second canvas
function sketch2(p) {
  p.setup = function () {
  {
  createCanvas(500, 200);
  textSize(20);
  textAlign(CENTER, CENTER);
  text("Move your cursor to the 'Preview' section\nPress 'B, Y, C, E, P, F, H, X, T, R, or V' to play sounds", width / 2, height / 2);
}
    
  };
 
}
new p5(sketch2);
`

Since the playback rate changes were not a requirement, I decided to omit this in my submission. 