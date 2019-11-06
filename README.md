## : : s p a c e 0 0 6

![space](https://github.com/nicolasbaez/space006/blob/master/space006.gif)

```processing
void setup() {
  size(512, 256);
  background(0);
}
int i=0;
float por;
int maxR=8;
int complete=0;
;
void draw() {
  noStroke();
  fill(0, 0, 0, 8);
  rect(0, 0, width, height);
  fill(0, 255, 0);
  por=map(i, 0, width, 0, 100);
  if (por>=0&&por<10) {
    ellipse(i, height/2, maxR, maxR);
  }
  if (por>=10&&por<20) {
    ellipse(i, map(sin(radians(map(por, 10, 20, 0, 180))), 0, 1, height*0.5, height*0.4), maxR, maxR);
  }
  if (por>=20&&por<30) {
    ellipse(i, height/2, maxR, maxR);
  }
  if (por>=30&&por<40) {
    ellipse(i, map(sin(radians(map(por, 30, 40, 0, 180))), 0, 1, height*0.5, height*0.55), maxR, maxR);
  }
  if (por>=40&&por<50) {
    ellipse(i, map(sin(radians(map(por, 40, 50, 0, 180))), 0, 1, height*0.5, height*0.1), maxR, maxR);
  }
  if (por>=50&&por<60) {
    ellipse(i, map(sin(radians(map(por, 50, 60, 0, 180))), 0, 1, height*0.5, height*0.6), maxR, maxR);
  }
  if (por>=60&&por<70) {
    ellipse(i, height/2, maxR, maxR);
  }
  if (por>=70&&por<80) {
    ellipse(i, map(sin(radians(map(por, 50, 60, 0, 180))), 0, 1, height*0.5, height*0.3), maxR, maxR);
  }
  if (por>=80&&por<100) {
    ellipse(i, height/2, maxR, maxR);
  }
  if (i<=width {
    i+=8;
  } else {
    complete++;
    i=0;
  }
  if (complete==2) {
    saveFrame("gif/space006-######.png");
  }
}
```
