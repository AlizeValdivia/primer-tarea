# primer-tarea
código de geometría 
void setup() //llamar funciones
{
size(640,640);
background(255,60,60,30); //fondo de color
//noFill(); 

//triangle(350,250,400,350,290,350); 
fill(0,255,150);
rect(455,455,100,100);
fill(0,150,150);
rect(440,500,15,30);
rect(480,500,10,20);
ellipse(507,597,80,80);

//triangle(350,250,400,350,290,350);
fill(80,56,70);
triangle(490,350,600,490,400,490);
fill(60,0,0);
ellipse(460,500,15,30);
fill(160,0,0);

triangle(160,180,200,130,400,160);

int tag=0;
for(int y=0; y<340; y+=30)
{
  for(int x=0; x<640; x+=30)
{
  if(tag%2==0)
  ellipse(x+(30/2),y+(30/2),30,10);
  fill(random(255),random(255),random(255));
  //el incremento de tam
  //para separar los circulos uno de otro, es decir uno si y uno no.
  tag++;
    }
    tag++;
}

strokeWeight(10);
strokeCap(ROUND);
fill(0,255,255);
line(500,500,500,600);

noStroke();
fill(0,0,47,90);
arc(200,480,200,200,QUARTER_PI,TWO_PI-QUARTER_PI);


//arc(360,360,100,100,QUARTER_PI,PI+QUARTER_PI);
//for(int y=0; y<=height; y+=10) //(alto de la ventana, comienza en 20, terina -20)hace un barrido, punto inicial a punto final en x.
//    for(int x=0; x<=width; x+=10) //wisth toma el valor de 500,
//    {
//        fill(random(0,255),random(0,255),random(0,255)); //si quiero que el fill afecte individualmente lo bajo 
//        //al replicar los tres random tenemos colores.
//        stroke(random(0,255),random(0,255),random(0,255)); //también puede aplicarse.
//        line(width,height,x,y); 
//    }


}
void draw() //dibujar
{
  
  strokeWeight(random(2,10)); //cambia el tamaño de la Rb
  stroke(random(0),random(250),250); //escoge colores al azar
  float rainbow_size =random(100,200);
  ellipse(150,170, rainbow_size,rainbow_size); //tamaño del la elipse
  fill(0,20);
  
   
}
