# Rera
Jogo educacional em conjunto com o ColabEduc

var page = 0
var xmenu = 70;
var largura = 250;
var altura = 60;
var yplay = 90;
var yinstru = 190;
var ycred = 290;
var segundos, seg = 0;
var a = 3, b = 2, c = 6, d = 5;
var tempo;

var x = 50;
var y = 370;

let img;

function preload() {
  img = loadImage('eu.jpg');
}

function setup() {
  createCanvas(400, 500);
  frameRate(30);
}

function draw() {
  textStyle(NORMAL);
  
  if(page == 0 ){
  background(240, 50, 50);
        
  textSize(20);
  text("ReRa: Resolvendo Racionais", 50, 20, 300, 40);
  
  rect(xmenu, yplay, largura, altura, 24);
    
  textAlign(CENTER);
  textSize(30);
    

  
  text("Play!", 190, 130);
    
  if(mouseX > xmenu && mouseX < xmenu+largura && mouseY>yplay && mouseY < yplay+altura){
    if(mouseIsPressed){
      page = 1;
    }
  }
  
  
  rect(xmenu, yinstru, largura, altura, 24);
  
  textAlign(CENTER);
  textSize(30);
  text("Instruções", 190, 230);
    
  if(mouseX > xmenu && mouseX < xmenu+largura && mouseY>yinstru && mouseY < yinstru+altura){
    if(mouseIsPressed){
      page = 2;
    }
  }

  rect(xmenu, ycred, largura, altura, 24);
    
  textAlign(CENTER);
  textSize(30);
  text("Créditos", 190, 330);
    
  if(mouseX > xmenu && mouseX < xmenu+largura && mouseY>ycred && mouseY < ycred+altura){
    if(mouseIsPressed){
      page = 3;
    }
  }
    
  }  
  
  if(page == 1 ){
    
    background(240, 50, 50);

    line(5, 400, 400, 400);
    
    rect(19, 19, 80, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("<= Voltar", 52, 44);
    

    textSize(50);
    text(a+ "X" +b+ " + " +c+ "X" +d, 200, 290);
    
    
    seg = seg + 1;
    segundos = parseInt(seg/30);
    textSize(20);
    text(segundos, 375, 480)
    
    
    if(mouseX > 19 && mouseX < 99 && mouseY>19 && mouseY < 69){      
      if(mouseIsPressed){
        page = 0;
      }
    }
     
    textSize(18);
    text("Escolha sua resposta: ", 100, 390);
    
    rect(200,360, 40, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("28", 220, 385);
    
    rect(260, 360, 40, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("36", 280, 385);
    
    rect(320, 360, 40, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("42", 340, 385);
    
     if(mouseX > 260 && mouseX < 300 && mouseY>360 && mouseY < 400){      
       if(mouseIsPressed){
        page = 4;
      }
    }

    
    
    
  }
  
  if(page == 4 ){
    
    background(240, 50, 50);

    line(5, 400, 400, 400);
    
    rect(19, 19, 80, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("<= Voltar", 52, 44);
    

    textSize(50);
    text(a+ " - " +b+ "X" +c+ " + " +d, 200, 290);
    
    
    seg = seg + 1;
    segundos = parseInt(seg/30);
    textSize(20);
    text(segundos, 375, 480)
    
    
    if(mouseX > 19 && mouseX < 99 && mouseY>19 && mouseY < 69){      
      if(mouseIsPressed){
        page = 0;
      }
    }
     
    textSize(18);
    text("Escolha sua resposta: ", 100, 390);
    
    rect(200,360, 40, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("7", 220, 385);
    
    rect(260, 360, 40, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("11", 280, 385);
    
    rect(320, 360, 40, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("14", 340, 385);
    
    if(mouseX > 320 && mouseX < 360 && mouseY>360 && mouseY < 400){      
      if(mouseIsPressed){
        page = 5;
      }
    
    }

    
    
    
  }
  
  if(page == 5 ){
    
    background(240, 50, 50);

    line(5, 400, 400, 400);
    
    rect(19, 19, 80, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("<= Voltar", 52, 44);
    

    textSize(50);
    text(a+ " + " +b+ "+" +c+ " X " +d, 200, 290);
    
    
    seg = seg + 1;
    segundos = parseInt(seg/30);
    textSize(20);
    text(segundos, 375, 480)
    
    
    if(mouseX > 19 && mouseX < 99 && mouseY>19 && mouseY < 69){      
      if(mouseIsPressed){
        page = 0;
      }
    }
     
    textSize(18);
    text("Escolha sua resposta: ", 100, 390);
    
    rect(200,360, 40, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("35", 220, 385);
    
    rect(260, 360, 40, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("42", 280, 385);
    
    rect(320, 360, 40, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("60", 340, 385);
    
    if(mouseX > 200 && mouseX < 240 && mouseY>360 && mouseY < 400){      
      if(mouseIsPressed){
        page = 6;
      }
    
    }

    
    
    
  }
  
  if(page == 6 ){
    
    background(240, 50, 50);

    line(5, 400, 400, 400);
    
    rect(19, 19, 80, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("<= Voltar", 52, 44);
    

    textSize(50);
    text(a+ "/" +b+ " + " +c+ "/" +d, 200, 290);
    
    
    seg = seg + 1;
    segundos = parseInt(seg/30);
    textSize(20);
    text(segundos, 375, 480)
    
    
    if(mouseX > 19 && mouseX < 99 && mouseY>19 && mouseY < 69){      
      if(mouseIsPressed){
        page = 0;
      }
    }
     
    textSize(18);
    text("Escolha sua resposta: ", 100, 390);
    
    rect(200,360, 40, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("2,3", 220, 385);
    
    rect(260, 360, 40, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("2,5", 280, 385);
    
    rect(320, 360, 40, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("2,7", 340, 385);
    
    if(mouseX > 320 && mouseX < 360 && mouseY>360 && mouseY < 400){      
      if(mouseIsPressed){
        page = 7;
      }
    
    }

    
    
    
  }
  
  if(page == 7 ){
    
    background(240, 50, 50);

    line(5, 400, 400, 400);
    
    rect(19, 19, 80, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("<= Voltar", 52, 44);
    

    textSize(50);
    text(a+ "X" +b+ " /" +c+ " +" +d, 200, 290);
    
    
    seg = seg + 1;
    segundos = parseInt(seg/30);
    textSize(20);
    text(segundos, 375, 480)
    
    
    if(mouseX > 19 && mouseX < 99 && mouseY>19 && mouseY < 69){      
      if(mouseIsPressed){
        page = 0;
      }
    }
     
    textSize(18);
    text("Escolha sua resposta: ", 100, 390);
    
    rect(200,360, 40, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("4", 220, 385);
    
    rect(260, 360, 40, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("6", 280, 385);
    
    rect(320, 360, 40, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("10", 340, 385);
    
    if(mouseX > 260 && mouseX < 300 && mouseY>360 && mouseY < 400){      
      if(mouseIsPressed){
        page = 8;
      }
    
    }

    
    
    
  }
  
  if(page == 8 ){
    tempo = segundos;
    
    background(240, 50, 50);
    
    rect(19, 19, 80, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("<= Voltar", 52, 44);
    
    if(mouseX > 19 && mouseX < 99 && mouseY>19 && mouseY < 69){      
      if(mouseIsPressed){
        page = 0;
      }
    }
    
    textSize(20);
    text("Parábens! Vocêc concluiu todos os desafios propostos no decorrer do game. Continue se dedicando assim no estudos e até mais!", 90, 60, 250, 200)
    
    text("Você concluiu o jogo em: "+tempo+" segundos. Muito bem !", 90, 240, 250, 300);
  }
  
  if(page == 2) {
    background(240, 50, 50);
    
    rect(19, 19, 80, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("<= Voltar", 52, 44);
    
    if(mouseX > 19 && mouseX < 99 && mouseY>19 && mouseY < 69){      
      if(mouseIsPressed){
        page = 0;
      }
    }
    
    
    textAlign(CENTER);
    textSize(20); 
    text("(EF07MA12) Resolver e elaborar problemas que envolvam as operações com números racionais. ", 50, 85, 320, 240);
    
    textAlign(CENTER);
    textSize(20); 
    text("Instruções: Você deverá resolver os problemas que serão apresentados e escolher a resposta quando solicitado. Durante o jogo, só existirá uma resposta correta, então você só irá passar de fase quando clicar na alternativa correta. ", 50, 250, 320, 350);
  
  }
   
  if(page == 3) {
    background(240, 50, 50);
    
    
    rect(19, 19, 80, 40, 24);
    textAlign(CENTER);
    textSize(15);
    text("<= Voltar", 52, 44);
    
    if(mouseX > 19 && mouseX < 99 && mouseY>19 && mouseY < 69){      
      if(mouseIsPressed){
        page = 0;
      }
    }
    
    textAlign(CENTER);
    textSize(20); 
    text("João Luiz Miranda de Melo : Programador.", 15, 95, 350, 200);
    image(img, 100, 180, 200, 200)
  }
}
