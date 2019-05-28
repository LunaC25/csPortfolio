# Cate Luna's Portfolio

### * [Dog WebPage](https://lunac25.github.io/testWeb/doggos.html)
<br>__About the project__
<br>  This website was a great way to begin the year.  I learned about the use of html and how to format things on a website to make it look nice.
***
### * [Dice](https://lunac25.github.io/dice3/)
<br>__About the project__
<br>In this project, I learned to work with Math.random() in order to make the die appear as I wanted them to. 
***
### * [Chemotaxis](https://lunac25.github.io/chemotaxis4/)
<br>__About the project__
<br>I enjoyed this project.  My code did not redraw the background constantly like many others, so you are able to create images with the old particles.  The particles that show on the screen as blue are the movement, and yellow is the final location.  When you press your mouse, it redraws to remove the blue particles!
***
### * [Starfield](https://lunac25.github.io/starfield5/)
<br>__About the project__
<br>This was probably my favorite project.  For this project, I used interfaces to make my stars.  The most challenging part was using pi to create the circular movement.
***
### * [BU Presentation](https://lunac25.github.io/collegepage/)
<br>__About the project__
<br>For this assignment, we researched the Computer Science program at a particular college. I chose Belmont University in Nashville, and spoke to Dr. Hooper in order to learn more about Comp Sci in college!
***
### * [PixelBud Presentation](https://lunac25.github.io/pixelbuds/)
<br>__About the project__
<br>  For this assignment, we researched an innovation that interested us.  My partner and I researched translating earbuds.
***

### Other Questions
<br>__Sources of Pride__
<br>Starfield and Chemotaxis were my best projects.  The majority of my creativity was shown in those two projects, as I messed around with my code with not redrawing the background, and worked more with Math.random() to create interesting objects.  As shown in my code snippet, I used Math.random to change each aspect of my oddball particle.  Another part of starfield was making the streak that followed the star.  
<br>__A Coding Hurdle__
<br>My biggest hurdle was the creativity.  I am mostly math and science based so when asked to do my own spin on these projects, I struggled.  They began rough but I am proud of the projects I did later on.  I like to follow a template, to ensure I do everything perfectly, but I was able to do my own thing with Chemotaxis and Starfield by experimenting more with my code.  
<br>__The Code Below__
<br>The code shown below is from the Starfield project.  I used Math.random() frequently in this class to ensure that the particles are always drawn in a different location, with different colors, and a different radius for their circular movement.  Something that I worked on collaboratively was using Pi to make the circular movement, because I did not understand how to make that function at first.    



<br>




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
