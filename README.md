def setup(): 
  size(600, 600)
  textSize(70)
def draw():
    clear()
    background(208,252,255)
    
    s = createShape()
    s.beginShape()
    s.fill(0,95,0)
    s.vertex(0, 100)
    s.vertex(-200, 900)
    s.vertex(200, 2800)
    s.vertex(640, 300)
    s.vertex(440, 200)
    s.vertex(300, 300)
    s.vertex(200, 160)
    s.vertex(100, height/4*2)
    s.endShape(CLOSE)
    
    shape(s, 25,25)
    fill(255,215,0)
    
    circle(299,100,100)
    fill(113,183,0)
    
    square(-1,450,600)
    fill(252,200,0)
    
    text("AK",450,550)
    
    if hex(get(mouseX,mouseY)) == ('FFFFE14A'):
         fill(255,0,255)
    else:
        fill(0,0,0)
    
    if keyPressed:
        if key == 'a' or key == 'k' or key == 'A' or key == 'K':
             fill(255,0,255)
