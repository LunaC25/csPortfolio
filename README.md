# csPortfolio

* WebPage [here](https://lunac25.github.io/testWeb/doggos.html)
* Lightning [here](https://lunac25.github.io/lightning2/)
* Lighting JS [here]()
* Dice [here](https://lunac25.github.io/dice3/)
* Chemot [here](https://lunac25.github.io/chemotaxis4/)
* Starfield [here](https://lunac25.github.io/starfield5/)
* BU Presentation [here](https://lunac25.github.io/lightning2/college.html)




```Java
class OddballParticle implements Particle
{
  int r,g,b;
  double x,y,speed,angle;
  OddballParticle(){
   x=(int)(Math.random()*300);
    y=(int)(Math.random()*300);
    speed = (Math.random()*10);
    angle = (PI*Math.random()*2);
   r = (int)(Math.random()*256);
   g = (int)(Math.random()*256);
   b = (int)(Math.random()*256);
  }
    void move(){
    x+=speed*cos((float)angle);
    y+=speed*sin((float)angle);
    angle-=.05;
    
  }
  void show(){
    stroke(r,r,b);
    fill(r,r,b);
    ellipse((float)x,(float)y,10,10);
  }
  

}
```
