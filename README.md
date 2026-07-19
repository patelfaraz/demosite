  <!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>I'm Sorry ❤️</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&family=Dancing+Script:wght@700&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Poppins,sans-serif;
}

body{

background:linear-gradient(-45deg,#ff9aa2,#fad0c4,#ffd1ff,#ffc3a0);
background-size:400% 400%;
animation:bg 12s ease infinite;
height:100vh;
overflow:hidden;
display:flex;
justify-content:center;
align-items:center;
color:white;

}

@keyframes bg{

0%{background-position:0 50%;}
50%{background-position:100% 50%;}
100%{background-position:0 50%;}

}

.container{

width:90%;
max-width:700px;
padding:40px;
border-radius:25px;
background:rgba(255,255,255,.12);
backdrop-filter:blur(18px);
text-align:center;
box-shadow:0 20px 40px rgba(0,0,0,.25);

}

img{

width:180px;
height:180px;
border-radius:50%;
object-fit:cover;
border:5px solid white;
margin-bottom:25px;

}

h1{

font-family:"Dancing Script";
font-size:62px;
margin-bottom:10px;

}

p{

font-size:18px;
line-height:1.8;

}

.letter{

margin-top:25px;
font-size:18px;

}

.timer{

margin-top:20px;
font-size:16px;
opacity:.9;

}

button{

padding:15px 35px;
border:none;
border-radius:50px;
margin:15px;
font-size:18px;
cursor:pointer;
transition:.3s;

}

#yes{

background:#ff3d7f;
color:white;

}

#no{

background:white;
color:#ff3d7f;
position:relative;

}

button:hover{

transform:scale(1.08);

}

.heart{

position:absolute;
color:white;
font-size:20px;
animation:float 6s linear infinite;
pointer-events:none;

}

@keyframes float{

0%{

transform:translateY(100vh);
opacity:0;

}

50%{

opacity:1;

}

100%{

transform:translateY(-120vh);
opacity:0;

}

}

.success{

display:none;
margin-top:25px;
font-size:26px;
font-family:"Dancing Script";

}

</style>
</head>

<body>

<div class="container">

<img src="your-photo.jpg">

<h1>I'm Sorry, Beba ❤️</h1>

<p>
I know I hurt you.<br>
Maybe my words weren't enough... maybe my actions weren't either.<br><br>

But if love means trying every single day to become a better person for you,
then I promise I'll never stop trying.
</p>

<div class="letter">

Every smile of yours is my favorite memory.

Every laugh of yours is my favorite song.

Every moment with you has become my definition of happiness.

If I could go back and change what hurt you,
I would do it without thinking twice.

I know I cannot change the past...

But I can promise to love you better tomorrow than I did yesterday.

I miss us.

I miss your smile.

I miss hearing you call me.

Most importantly...

I miss making you happy.

❤️

</div>

<div class="timer">

Waiting for your forgiveness for...

<div id="time"></div>

</div>

<button id="yes">I Forgive You ❤️</button>

<button id="no">Still Angry 😒</button>

<div class="success" id="success">

Thank you... ❤️

You have no idea how much this means to me.

I promise I'll keep choosing you,
every single day.

I love you endlessly. ❤️

</div>

</div>

<script>

const start=new Date("2026-07-15");

function update(){

const now=new Date();

let diff=now-start;

let days=Math.floor(diff/86400000);

let hrs=Math.floor(diff%86400000/3600000);

let mins=Math.floor(diff%3600000/60000);

let secs=Math.floor(diff%60000/1000);

document.getElementById("time").innerHTML=

`${days} Days ${hrs} Hours ${mins} Minutes ${secs} Seconds`;

}

setInterval(update,1000);

update();

const no=document.getElementById("no");

no.addEventListener("mouseover",()=>{

const x=Math.random()*window.innerWidth-150;

const y=Math.random()*window.innerHeight-100;

no.style.position="absolute";

no.style.left=x+"px";

no.style.top=y+"px";

});

document.getElementById("yes").onclick=function(){

document.getElementById("success").style.display="block";

for(let i=0;i<120;i++){

let h=document.createElement("div");

h.className="heart";

h.innerHTML="❤️";

h.style.left=Math.random()*100+"vw";

h.style.animationDuration=(Math.random()*4+3)+"s";

document.body.appendChild(h);

setTimeout(()=>h.remove(),7000);

}

};

setInterval(()=>{

const h=document.createElement("div");

h.className="heart";

h.innerHTML="❤";

h.style.left=Math.random()*100+"vw";

h.style.fontSize=(Math.random()*20+15)+"px";

h.style.animationDuration=(Math.random()*3+4)+"s";

document.body.appendChild(h);

setTimeout(()=>h.remove(),7000);

},350);

</script>

</body>
</html>  }

    .card {
      background: #fff;
      max-width: 500px;
      width: 100%;
      padding: 30px;
      border-radius: 20px;
      box-shadow: 0 20px 40px rgba(0,0,0,0.1);
      text-align: center;
      animation: fadeIn 1.2s ease;
    }

    h1 {
      font-family: 'Playfair Display', serif;
      font-size: 2.2rem;
      margin-bottom: 15px;
      color: #d6336c;
    }

    p {
      font-size: 1rem;
      color: #444;
      line-height: 1.7;
      margin-bottom: 20px;
    }

    .heart {
      font-size: 2.5rem;
      animation: pulse 1.5s infinite;
      margin-bottom: 15px;
    }

    button {
      padding: 12px 25px;
      border: none;
      border-radius: 25px;
      background: #d6336c;
      color: white;
      font-size: 1rem;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    button:hover {
      background: #b92d5b;
      transform: scale(1.05);
    }

    .hidden {
      display: none;
      margin-top: 20px;
      font-size: 1rem;
      color: #333;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.2); }
      100% { transform: scale(1); }
    }
  </style>
</head>
<body>

  <div class="card">
    <div class="heart">🥺</div>
    <h1>Beba, I'm Sorry</h1>

    <p>
      I know I hurt you, and I hate that I did.  
      There isn’t a single excuse that can undo it,  
      but there’s a heart here that truly regrets it.
    </p>

    <p>
      You mean more to me than my ego, my anger, or my mistakes.  
      I’m learning, I’m trying, and I promise to do better —  
      not just in words, but in actions.
    </p>

    <button onclick="showMessage()">Tap if you can forgive me 🥺</button>

    <div id="message" class="hidden">
      <p>
        Thank you for even reading this.  
        I love you, and I’ll keep choosing you — every single day. 💖
      </p>
    </div>
  </div>

  <script>
    function showMessage() {
      document.getElementById("message").classList.remove("hidden");
    }
  </script>

</body>
</html>
