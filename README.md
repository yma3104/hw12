# https://editor.p5js.org/yma/sketches/zQFIu8o5E
//sounds
var soundA;
var soundB;
var soundC;
var soundD;
var soundE;
var soundF;
var soundG;
var soundH;
var soundI;
var soundJ;
var soundK;
var soundL;
var soundM;
var soundN;
var soundO;
var soundP;
var soundQ;
var soundR;
var soundS;
var soundT;
var soundU;
var soundV;
var soundW;
var soundX;
var soundY;
var soundZ;

// keep track of what the user typed
var word = "";

function preload() {
  soundFormats('mp3');
  soundA = loadSound('sounds/A.mp3');
  // soundB = loadSound('sounds/B.mp3');
}

function setup() {
  createCanvas(400, 400);
  fill(255);
  
  var score = 0;
  score++;
  textSize(24);
  text("Score: " + score, 10, 25);
}


//timer

let timer = 50

function draw() {
  background(100, 30);
  textAlign(CENTER, CENTER);
  textSize(40);
  text(timer, width / 8, height / 8);

  if (frameCount % 60 == 0 && timer > 0) {
    timer--;
  }

  if (timer == 0) {
    text("GAME OVER", width / 2, height * 0.7);
  }
  

  text("/ˈhænd/", 200, 130);
   if (word == "hand") {
   text("✔", 200, 200);
   word = word + "✔";
 }
  
   text("/ˌek.spekˈteɪ.ʃən/", 200, 130);
   if (word == "expectation") {
   text("✔", 200, 200);
   word = word + "✔";
 }
}


//type
function keyPressed() {
  textSize(150);
  noStroke();
  if (timer == 0){
     textSize = 0;
  }
    if (key == 'a') {
    print("Hit 'a'");
    soundA.play();
    text('A', 200, 230);
    word = word + "a";
  }
  if (key == 'b') {
    text('B', 200, 230);
    soundB.play();
    word = word + "b"
  }
  if (key == 'c') {
    text('C', 200, 230);
    soundC.play();
    word = word + "c"
  }
  if (key == 'd') {
    text('D', 200, 230);
    soundD.play();
    word = word + "d"
  }
    if (key == 'e') {
    text('E', 200, 230);
    soundD.play();
    word = word + "e"
  }
    if (key == 'f') {
    text('D', 200, 230);
    soundD.play();
    word = word + "f"
  }
    if (key == 'g') {
    text('G', 200, 230);
    soundG.play();
    word = word + "g"
  }  
    if (key == 'h') {
    text('H', 200, 230);
    soundH.play();
    word = word + "h"
  }
    if (key == 'i') {
    text('I', 200, 230);
    soundI.play();
    word = word + "i"
  }
    if (key == 'j') {
    text('J', 200, 230);
    soundJ.play();
    word = word + "j"
  }
    if (key == 'k') {
    text('K', 200, 230);
    soundK.play();
    word = word + "k"
  }
    if (key == 'l') {
    text('L', 200, 230);
    soundL.play();
    word = word + "l"
  }
    if (key == 'm') {
    text('M', 200, 230);
    soundM.play();
    word = word + "m"
  }
    if (key == 'n') {
    text('N', 200, 230);
    soundN.play();
    word = word + "n"
  }
    if (key == 'o') {
    text('O', 200, 230);
    soundO.play();
    word = word + "o"
  }
    if (key == 'p') {
    text('P', 200, 230);
    soundP.play();
    word = word + "p"
  }
    if (key == 'q') {
    text('Q', 200, 230);
    soundQ.play();
    word = word + "q"
  }
    if (key == 'r') {
    text('R', 200, 230);
    soundR.play();
    word = word + "r"
  }
    if (key == 's') {
    text('S', 200, 230);
    soundS.play();
    word = word + "s"
  }
  if (key == 't') {
    text('T', 200, 230);
    soundt.Pplay();
    word = word + "t"
  }
    if (key == 'u') {
    text('U', 200, 230);
    soundU.play();
    word = word + "u"
  }
    if (key == 'v') {
    text('V', 200, 230);
    soundV.play();
    word = word + "v"
  }
    if (key == 'w') {
    text('W', 200, 230);
    soundW.play();
    word = word + "w"
  }
    if (key == 'x') {
    text('X', 200, 230);
    soundX.play();
    word = word + "x"
  }
    if (key == 'y') {
    text('Y', 200, 230);
    soundY.play();
    word = word + "y"
  }
    if (key == '  z') {
    text('Z', 200, 230);
    soundZ.play();
    word = word + "z"
  }
}
