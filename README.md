# D-J_
Un detalle hecho con amor, pensado para que lo leas  y recuerdes cuánto te amo.

<html lang="es">
<head>
<meta charset="UTF-8">
<title>Para Mi Amor</title>

<style>
body{
    margin:0;
    padding:0;
    background: linear-gradient(135deg,#1e1e2f,#3a3a5f);
    font-family: 'Georgia', serif;
    color:white;
    text-align:center;
    overflow:hidden;
}

.container{
    padding:50px;
    max-width:800px;
    margin:auto;
}

h1{
    font-size:40px;
    margin-bottom:20px;
}

.fancy{
    font-style:italic;
    font-size:28px;
}

p{
    font-size:20px;
    line-height:1.8;
}

button{
    margin-top:30px;
    padding:12px 25px;
    font-size:18px;
    border:none;
    border-radius:25px;
    background:#ff4d88;
    color:white;
    cursor:pointer;
    transition:0.3s;
}

button:hover{
    background:#ff1a66;
    transform:scale(1.05);
}

.hidden{
    display:none;
}

.fade{
    animation:fadeIn 1.5s;
}

@keyframes fadeIn{
    from{opacity:0;}
    to{opacity:1;}
}

.music{
    position:fixed;
    bottom:15px;
    right:15px;
}
</style>
</head>

<body>

<div class="container fade">

<h1>Para mi amor eterno... Jane</h1>

<p>
Lo escribo para que mi amor por ti quede plasmado.<br><br>

A veces omito un cierto detalle que pasa por mi cabeza... y ese detalle eres tú.  
Eres mi parte favorita del día ❤️<br><br>

Me encanta que, a pesar de lo ocupados que estemos, siempre estamos el uno para el otro.  
Basta con una sola notificación tuya para que mi corazón se exalte y mi día cambie totalmente...<br><br>

Sabes... a veces uno se pregunta cómo saber si realmente estás enamorado...  
y yo lo terminé de entender hace unos ayeres.<br><br>

Me di cuenta de que me enamoré de ti cuando mi corazón se emocionaba con tan solo pensar en ti.  
A pesar de la distancia, me haces sentir de todo.  
Con una notificación alegras mi día.<br><br>

Me haces sentir lo que nunca antes había experimentado con alguien,  
y <span class="fancy">𝒯𝑒 𝒶𝓂𝑜 𝒾𝓃𝒻𝒾𝓃𝒾𝓉𝒶𝓂𝑒𝓃𝓉𝑒</span>.<br><br>

Tú me haces sentir cosas tan bonitas e inexplicables que las palabras no pueden describir.  
Mi amor por ti aumenta día tras día.
</p>

<button onclick="mostrarSiguiente()">Continuar 💌</button>

<div id="final1" class="hidden fade">
    <h2>1.</h2>
    <p>Me tienes amando cada pedacito de ti.</p>
</div>

<div id="final2" class="hidden fade">
    <h2>2.</h2>
    <p>Mientras yo exista, a ti no te va a faltar quien ame todo de ti.</p>
</div>

<div id="final3" class="hidden fade">
    <h2>3.</h2>
    <p>Jamás te podré explicar el inmenso amor que tengo hacia ti y el miedo gigantesco que me da perderte.</p>
</div>

<div id="final4" class="hidden fade">
    <h2>4.</h2>
    <p>No eres parte de mi vida...<br>
    <span class="fancy">Eres mi vida</span></p>
</div>

<div id="final5" class="hidden fade">
    <h2>5.</h2>
    <p>我爱你 ❤️</p>
    <p>Tu eterno enamorado,<br>Daniel</p>
</div>

</div>

<div class="music">
    <!-- OPCIÓN BOTÓN YOUTUBE -->
    <button onclick="window.open('https://www.youtube.com/results?search_query=golden+brown+the+stranglers')">
        🎵 Escuchar Golden Brown
    </button>
</div>

<script>
let paso = 1;

function mostrarSiguiente(){
    if(paso <= 5){
        document.getElementById("final"+paso).classList.remove("hidden");
        paso++;
    }
}
</script>

</body>
</html>
