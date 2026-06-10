<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Emprende IA Perú</title>

<link rel="stylesheet" href="style.css">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

</head>
<body>

<nav>
<div class="logo">🚀 EMPRENDE IA</div>

<ul>
<li><a href="#inicio">Inicio</a></li>
<li><a href="#nosotros">Nosotros</a></li>
<li><a href="#ideas">Ideas</a></li>
<li><a href="#proyectos">Proyectos</a></li>
<li><a href="#academia">Academia</a></li>
</ul>
</nav>

<header id="inicio">

<h1>Transformando Ideas en Proyectos Reales</h1>

<p>
La plataforma educativa que impulsa la creatividad,
innovación y emprendimiento de los estudiantes del Perú.
</p>

<a href="#ideas" class="btn">
Generar Idea
</a>

</header>

<section id="nosotros">

<h2>¿Qué es Emprende IA?</h2>

<p>
Emprende IA es una plataforma diseñada para ayudar
a estudiantes a desarrollar proyectos innovadores,
resolver problemas de su comunidad y aprender
herramientas de emprendimiento.
</p>

<div class="cards">

<div class="card">
<h3>💡 Creatividad</h3>
<p>Genera soluciones innovadoras.</p>
</div>

<div class="card">
<h3>🚀 Innovación</h3>
<p>Convierte ideas en proyectos.</p>
</div>

<div class="card">
<h3>🌎 Impacto</h3>
<p>Ayuda a tu comunidad.</p>
</div>

</div>

</section>

<section id="ideas">

<h2>🤖 Generador de Ideas</h2>

<select id="categoria">

<option value="">Seleccione una categoría</option>

<option>Tecnología</option>
<option>Educación</option>
<option>Salud</option>
<option>Turismo</option>
<option>Agricultura</option>

</select>

<button onclick="generarIdea()">
Generar Proyecto
</button>

<div id="resultado" class="resultado">
Aquí aparecerá tu idea innovadora.
</div>

</section>

<section id="proyectos">

<h2>🏆 Proyectos Destacados</h2>

<div class="cards">

<div class="card">
<h3>🌱 EcoSmart</h3>
<p>Reciclaje inteligente mediante QR.</p>
</div>

<div class="card">
<h3>📚 Aula IA</h3>
<p>Tutor virtual para estudiantes.</p>
</div>

<div class="card">
<h3>🌄 Turismo Digital</h3>
<p>Promoción de destinos locales.</p>
</div>

</div>

</section>

<section id="academia">

<h2>📚 Academia Emprende IA</h2>

<div class="curso">
<h3>Design Thinking</h3>
<p>Aprende a resolver problemas reales.</p>
</div>

<div class="curso">
<h3>Canvas</h3>
<p>Diseña tu modelo de negocio.</p>
</div>

<div class="curso">
<h3>Marketing Digital</h3>
<p>Promociona tu emprendimiento.</p>
</div>

</section>

<footer>

<h3>EMPRENDE IA 2026</h3>

<p>
Innovación • Creatividad • Emprendimiento
</p>

</footer>

<script src="script.js"></script>

</body>
</html>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
}

body{
background:#f5f8ff;
color:#222;
}

nav{
background:white;
padding:15px 8%;
display:flex;
justify-content:space-between;
align-items:center;
position:sticky;
top:0;
box-shadow:0 2px 10px rgba(0,0,0,.1);
}

.logo{
font-size:1.3rem;
font-weight:700;
color:#003b95;
}

nav ul{
display:flex;
gap:25px;
list-style:none;
}

nav a{
text-decoration:none;
color:#003b95;
font-weight:600;
}

header{
height:90vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;
background:linear-gradient(135deg,#003b95,#00b96b);
color:white;
}

header h1{
font-size:4rem;
margin-bottom:20px;
}

header p{
max-width:700px;
line-height:1.8;
}

.btn{
margin-top:30px;
padding:15px 35px;
background:white;
color:#003b95;
text-decoration:none;
font-weight:bold;
border-radius:30px;
}

section{
padding:80px 10%;
}

section h2{
text-align:center;
margin-bottom:40px;
color:#003b95;
}

.cards{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:25px;
margin-top:30px;
}

.card{
background:white;
padding:25px;
border-radius:20px;
box-shadow:0 5px 15px rgba(0,0,0,.08);
transition:.3s;
}

.card:hover{
transform:translateY(-8px);
}

select,
button{
width:100%;
padding:15px;
margin-top:15px;
border:none;
border-radius:10px;
}

button{
background:#003b95;
color:white;
cursor:pointer;
}

.resultado{
margin-top:20px;
padding:20px;
background:white;
border-radius:15px;
box-shadow:0 5px 15px rgba(0,0,0,.08);
}

.curso{
background:white;
padding:20px;
margin-bottom:20px;
border-radius:15px;
box-shadow:0 5px 15px rgba(0,0,0,.08);
}

footer{
background:#003b95;
color:white;
padding:40px;
text-align:center;
}
function generarIdea(){

const categoria =
document.getElementById("categoria").value;

const resultado =
document.getElementById("resultado");

const ideas={

"Tecnología":
"🤖 APP COMUNIDAD DIGITAL\n\nUna aplicación que conecte estudiantes con oportunidades educativas.",

"Educación":
"📚 AULA IA\n\nTutor virtual para reforzar el aprendizaje escolar.",

"Salud":
"❤️ SALUD CERCA DE TI\n\nAplicación de prevención y bienestar.",

"Turismo":
"🏔️ TURISMO DIGITAL\n\nPlataforma para promocionar destinos turísticos locales.",

"Agricultura":
"🌾 AGROTECH ESCOLAR\n\nSistema inteligente para optimizar el riego."
};

resultado.innerText=
ideas[categoria] ||
"Seleccione una categoría.";
}      
