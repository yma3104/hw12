# https://editor.p5js.org/yma/sketches/zQFIu8o5E

function setup() { 
  createCanvas(400, 400);
  fill(255);
} 

let timer = 60

function draw() { 
  background(100);
  textAlign(CENTER, CENTER);
  textSize(40);
  text(timer, width/8, height/8);  
  
  if (frameCount % 60 == 0 && timer > 0) { 
    timer --;
  }
  
  if (timer == 0) {
    text("GAME OVER", width/2, height*0.7);
  }
}

function keytyped() {  
  textSize(150);
  noStroke();
  
  if (key == 'a') {
  text("A", 150, 230);
 }
  if (key == 'b') {
  text("B", 150, 230);
 }
  if (key == 'c') {
  text("C", 150, 230);
 }
  if (key == 'd') {
  text("D", 150, 230);
 }
}
