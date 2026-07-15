# Pour-meganee
I want to propose marriage 
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<title>Pour Mégane ❤️</title>

<style>
body{
margin:0;
background:#000;
color:white;
font-family:Arial;
display:flex;
justify-content:center;
align-items:center;
height:100vh;
overflow:hidden;
text-align:center;
}

#box{
padding:30px;
}

button{
padding:15px 35px;
font-size:20px;
border:none;
border-radius:40px;
background:#ff2d75;
color:white;
cursor:pointer;
transition:.3s;
}

button:hover{
transform:scale(1.08);
}

.heart{
position:absolute;
font-size:25px;
animation:fall 5s linear infinite;
}

@keyframes fall{
0%{
transform:translateY(-100vh);
opacity:1;
}
100%{
transform:translateY(100vh);
opacity:0;
}
}
</style>

</head>

<body>

<div id="box">
<h1 id="text">❤️ Un petit message pour toi...</h1>
<br>
<button onclick="next()">Continuer</button>
</div>

<script>

let step=0;

function next(){

step++;

if(step==1){
document.getElementById("text").innerHTML=
"Tu es prête ? 🥹";
}

else if(step==2){
document.getElementById("text").innerHTML=
"Promets-moi de ne pas fermer cette page... ❤️";
}

else if(step==3){
document.getElementById("text").innerHTML=
"J'ai quelque chose d'important à te dire...";
}

else if(step==4){
document.getElementById("text").innerHTML=
"Depuis que tu es entrée dans ma vie...<br><br>Tout est devenu plus beau ❤️";
}

else if(step==5){
document.getElementById("text").innerHTML=
"Chaque sourire de toi est devenu mon bonheur...";
}

else if(step==6){
document.getElementById("text").innerHTML=
"Je veux passer toute ma vie avec toi...";
}

else if(step==7){
document.getElementById("text").innerHTML=
"Ferme les yeux 3 secondes...✨";
}

else if(step==8){

document.body.style.background="#240012";

setInterval(createHeart,200);

document.getElementById("text").innerHTML=
"<h1 style='color:#ff5fa2;font-size:50px;'>💍 Mégane...</h1><br><h2>Veux-tu m'épouser ? ❤️</h2><br><button onclick='yes()'>OUI ❤️</button> <button id='no' onmouseover='moveNo()'>NON 😅</button>";

}

}

function yes(){

document.body.innerHTML=
"<div style='display:flex;justify-content:center;align-items:center;height:100vh;width:100%;font-size:45px;color:white;text-align:center;'>🎉❤️ OUIIIII !!!<br><br>Tu viens de faire de moi le garçon le plus heureux du monde 💍❤️</div>";

}

function moveNo(){

let b=document.getElementById("no");

b.style.position="absolute";

b.style.left=Math.random()*80+"%";

b.style.top=Math.random()*80+"%";

}

function createHeart(){

let h=document.createElement("div");

h.className="heart";

h.innerHTML="❤️";

h.style.left=Math.random()*100+"vw";

h.style.animationDuration=(3+Math.random()*4)+"s";

document.body.appendChild(h);

setTimeout(()=>{

h.remove();

},7000);

}

</script>

</body>
</html>
