# pagina-da-web
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Pelé - O Rei do Futebol</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <h1>⚽ Pelé - O Rei do Futebol</h1>
    <p>Conheça a história do maior jogador da história.</p>
</header>

<section class="hero">
    <img src="https://images.unsplash.com/photo-1508098682722-e99c643e7485?auto=format&fit=crop&w=1400&q=80" alt="Campo de futebol">
</section>

<section class="conteudo">

<div class="foto">
    <!-- Troque o src pela foto do Pelé enviada ao CodePen -->
    <img src="https://upload.wikimedia.org/wikipedia/commons/5/5e/Pele_con_brasil_%28cropped%29.jpg" alt="Pelé">
</div>

<div class="texto">

<h2>Quem foi Pelé?</h2>

<p>
Edson Arantes do Nascimento, conhecido como Pelé, nasceu em 23 de outubro de 1940, em Três Corações, Minas Gerais.
</p>

<p>
Começou sua carreira no Santos Futebol Clube aos 15 anos e rapidamente encantou o mundo com seu talento, velocidade e capacidade de fazer gols.
</p>

<p>
Pelé conquistou três Copas do Mundo com a Seleção Brasileira (1958, 1962 e 1970), sendo o único jogador da história a alcançar esse feito.
</p>

<p>
Durante sua carreira marcou mais de mil gols e ajudou a transformar o futebol em um esporte ainda mais popular em todo o planeta.
</p>

<p>
Seu legado permanece vivo até hoje, sendo reconhecido como "O Rei do Futebol".
</p>

</div>

</section>

<section class="cards">

<div class="card">
<h3>🏆 3 Copas do Mundo</h3>
<p>1958 • 1962 • 1970</p>
</div>

<div class="card">
<h3>⚽ Mais de 1.000 gols</h3>
<p>Um dos maiores artilheiros da história.</p>
</div>

<div class="card">
<h3>👑 Rei do Futebol</h3>
<p>Ícone mundial do esporte.</p>
</div>

</section>

<section class="curiosidade">

<h2>Curiosidade</h2>

<p id="mensagem">
Clique no botão para descobrir uma curiosidade sobre Pelé.
</p>

<button onclick="mostrar()">Mostrar Curiosidade</button>

</section>

<footer>

Projeto desenvolvido em HTML • CSS • JavaScript

</footer>

<script src="script.js"></script>

</body>
</html>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Poppins,sans-serif;
}

body{
background:#101010;
color:#fff;
}

header{
background:linear-gradient(90deg,#0c7a2d,#17b857);
text-align:center;
padding:35px;
}

header h1{
font-size:42px;
}

.hero img{
width:100%;
height:350px;
object-fit:cover;
}

.conteudo{
max-width:1100px;
margin:50px auto;
display:flex;
gap:40px;
align-items:center;
padding:20px;
flex-wrap:wrap;
}

.foto{
flex:1;
text-align:center;
}

.foto img{
width:280px;
height:350px;
object-fit:cover;
border-radius:15px;
border:5px solid #17b857;
}

.texto{
flex:2;
}

.texto h2{
color:#00ff88;
margin-bottom:20px;
font-size:35px;
}

.texto p{
margin-bottom:18px;
font-size:18px;
line-height:1.8;
}

.cards{
display:flex;
justify-content:center;
gap:30px;
flex-wrap:wrap;
padding:40px;
}

.card{
background:#1b1b1b;
padding:30px;
width:300px;
border-radius:15px;
text-align:center;
transition:.4s;
}

.card:hover{
transform:translateY(-10px);
background:#239d52;
}

.card h3{
margin-bottom:15px;
}

.curiosidade{
text-align:center;
padding:50px;
}

button{
padding:15px 35px;
border:none;
border-radius:10px;
background:#17b857;
color:white;
font-size:18px;
cursor:pointer;
margin-top:20px;
}

button:hover{
background:#00d96c;
}

#mensagem{
margin-top:20px;
font-size:22px;
color:#ffe600;
}

footer{
background:#000;
text-align:center;
padding:25px;
margin-top:40px;
}
const curiosidades = [

"Pelé é o único jogador tricampeão mundial.",

"Marcou mais de 1.000 gols durante sua carreira.",

"Foi eleito Atleta do Século.",

"Estreou no Santos com apenas 15 anos.",

"É conhecido mundialmente como O Rei do Futebol."

];

function mostrar(){

const numero = Math.floor(Math.random()*curiosidades.length);

document.getElementById("mensagem").innerHTML = curiosidades[numero];

}
