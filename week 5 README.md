# weekly-lurning
example of mathmatic code 
// y = 5x
// x = 5t
//y = 3t + 3

float t;//command

void setup() {
  background(20);
  size (500,500);
}

void draw() {
  background(20);
  stroke(255);
  strokeWeight(5);

  translate(width/2, height/2);
    // drawing a path
    
  point(x1(t),y1(t));
  point(x2(t),y2(t));
  t++;
}
// statting poit generation

float x1(float t) {
  return sin(t / 10) * 100 + sin(t / 5) * 20;
}

float y1(float t) {
  return cos(t / 10) * 100;
}
float x2 (float t) {
  return sin(t / 10) * 200 + sin(t) * 2;
}

float y2 (float t) {
  return cos(t / 20) * 200 + cos(t / 12) * 20;
}

//point of path movement
