# Laboratorio-4---Implementaci-n-de-Ciclos-con-P5JS
var blueB, pinkB;
var k, l;

function setup() {
createCanvas(700,350);
}

function draw() {
    
//Intensidad del calor en la atmosfera por el cambio climático
  
//Variable del fondo dependiendo el movimiento del mouse   
Bb = map(mouseX,0,width,15,229);
Bg = map(mouseX,0,width,300,280);
background(200,Bg,Bb);
    
// Nebulas
//Variable del color de las estrellas dependiendo el lugar del mouse
alphaE = map(mouseX,0,width,255,0);
    
if(mouseX <= width*3/4){
for(l=0; l<=height; l+=30){
for(k=0; k<=width; k+=30){
fill(255,alphaE);
noStroke();
rect(k,l,3,5);
}}    }
    
// Estrellas
maxRadioStar = map(mouseX,0,width,350,50);
    
var sR=233;
var sG=128
var sB=22;
    
for (var radioStar=maxRadioStar; radioStar>5; radioStar-=random(10, 15)) 
{
fill(sR, sG, sB);
noStroke();  
rect(width/4, height/4, radioStar, radioStar); 

sR+=10;
sG+=10;
sB+=10;}
} 
