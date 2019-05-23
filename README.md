# Projetolop6
etapa6
var x=50
var y=200
var xi=385
var yi=200
var raioP=15
var raioO=20
function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(150);
  ellipse(x,y,2*raioP,2*raioP)
    if ( keyIsDown(RIGHT_ARROW) )
  {
    x=x+4
  }
   if ( keyIsDown(LEFT_ARROW) )
  {
    x=x-4
  }
  if ( keyIsDown(UP_ARROW) )
  {
    y=y-4
  }
    if ( keyIsDown(DOWN_ARROW) )
  {
    y=y+4
  }
  ellipse(xi,yi,2*raioO,2*raioO)
  if(x>50)
  {
    xi=xi-2
  }
  if(dist(x, y, xi, yi)< raioO + raioP) 
  {
    x=50
    y=200
  }
}
