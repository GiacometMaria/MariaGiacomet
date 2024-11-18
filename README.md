
<!DOCTYPE html>
<html lang="en">
  <head>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/1.9.4/p5.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/1.9.4/addons/p5.sound.min.js"></script>
    <link rel="stylesheet" type="text/css" href="style.css">
    <meta charset="utf-8" />

  </head>
  <body>
    <main>
    </main>
    <script src="sketch.js"></script>
  </body>
</html>
let palavra;

function setup() {
  createCanvas(600, 600);//tamanho da tela

  palavra = palavraAleatoria();
  
}

function palavraAleatoria() {
  
  let palavras = ["GuardiõesdaGaláxia", "Vingadores", "HomemAranha"];//filmes sugeridos para assistir
  
  return random(palavras);
}

function inicializaCores() {
  background("lightyellow");//cor do fundo
  fill("#FFB6FA");//cor das palavras
  textSize(50);//tamanho do texto
  textAlign(CENTER, CENTER);
}

function palavraParcial(minimo, maximo) {
  let quantidade = map(mouseX, minimo, maximo, 1, palavra.length);
  let parcial = palavra.substring(0, quantidade);
  return parcial;
}

function draw() {
  
  inicializaCores();

  let texto = palavraParcial(0, width);
    
  text(texto, 300, 200);//local que as palavras ficam
  
}
function
FilmesLegaisParaAssistir(filme, genero)
{

}
