<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Para Jane 💌</title>

<style>
body{
    margin:0;
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    background: linear-gradient(135deg,#2b2b4b,#1a1a2e);
    font-family: 'Georgia', serif;
    overflow:hidden;
}

/* SOBRE */
.sobre{
    position:relative;
    width:320px;
    height:220px;
    background:#ff4d88;
    cursor:pointer;
    transition:0.5s;
}

.sobre:before{
    content:"";
    position:absolute;
    top:0;
    left:0;
    width:0;
    height:0;
    border-left:160px solid transparent;
    border-right:160px solid transparent;
    border-top:110px solid #ff80aa;
    transform-origin:top;
    transition:1s;
}

/* CARTA */
.carta{
    position:absolute;
    width:300px;
    height:400px;
    background:white;
    color:#333;
    top:-200px;
    left:10px;
    padding:20px;
    box-sizing:border-box;
    transform:translateY(200px);
    transition:1s;
    opacity:0;
    overflow:auto;
    border-radius:10px;
}

/* ABIERTO */
.sobre.abierto:before{
    transform:rotateX(180deg);
}

.sobre.abierto .carta{
    transform:translateY(-20px);
    opacity:1;
}

/* TEXTO */
h1{
    text-align:center;
    font-size:22px;
}

.fancy{
    font-style:italic;
    font-size:20px;
}

/* BOTÓN MÚSICA */
.boton-musica{
    position:fixed;
    bottom:20px;
    right:20px;
    padding:10px 20px;
    border:none;
    border-radius:20px;
    background:#ff4d88;
    color:white;
    cursor:pointer;
}
</style>
</head>

<body>

<div class="sobre" onclick="abrirCarta()" id="sobre">
    <div class="carta">
        <h1>Para mi amor eterno... Jane</h1>

        <p>
        Lo escribo para que mi amor por ti quede plasmado.<br><br>

        A veces omito un cierto detalle que pasa por mi cabeza... y ese detalle eres tú.  
        Eres mi parte favorita del día ❤️<br><br>

        Me encanta que, a pesar de lo ocupados que estemos, siempre estamos el uno para el otro.  
        Basta con una sola notificación tuya para que mi corazón se exalte y mi día cambie totalmente...<br><br>

        Me di cuenta de que me enamoré de ti cuando mi corazón se emocionaba con tan solo pensar en ti.  
        A pesar de la distancia, me haces sentir de todo.<br><br>

        Me haces sentir lo que nunca antes había experimentado con alguien,  
        y <span class="fancy">𝒯𝑒 𝒶𝓂𝑜 𝒾𝓃𝒻𝒾𝓃𝒾𝓉𝒶𝓂𝑒𝓃𝓉𝑒</span>.<br><br>

        Tú me haces sentir cosas tan bonitas e inexplicables que las palabras no pueden describir.  
        Mi amor por ti aumenta día tras día.<br><br>

        我爱你 ❤️<br><br>

        Tu eterno enamorado,<br>
        Daniel
        </p>
    </div>
</div>

<audio id="musica" loop>
    <source src="golden-brown.mp3" type="audio/mpeg">
</audio>

<button class="boton-musica" onclick="reproducirMusica()">🎵 Reproducir Golden Brown</button>

<script>
function abrirCarta(){
    document.getElementById("sobre").classList.toggle("abierto");
}

function reproducirMusica(){
    document.getElementById("musica").play();
}
</script>

</body>
</html>
