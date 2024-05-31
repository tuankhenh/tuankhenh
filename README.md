<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Love</title>
    <link rel="stylesheet" href="main.css">
    <link rel="shortcut icon" href="./icon.png" type="image/x-icon">
</head>
<body>
    <div class="grid"></div>

    <div class="warning"></div>

    <div class="base">
        <button id="activate">
            <span></span>
        </button>
    </div>

    <div class="box opened" id="cover">
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <span></span><span></span>
    </div>

    <div class="hinges"></div>

    <div class="text">
        SELF-&thinsp;DESTRUCT
    </div>
    
    <div id="panel2">
        <div id="msg">YOUR ANSWER IS FALSE</div>
        <span id="again">AGAIN PLEASE</span>
    </div>


    <div id="panel">
        <div id="msg">ANSWER NOW</div>
        <div id="time">9</div>
        <span id="abort"><a href="index2.html">YES</a></span>
        <span id="no">NO</span>
        <span id="detonate">Oc Cho</span>
    </div>

    <div id="turn-off"></div>
    <div id="closing"></div>

    <div id="restart"><button id="reload"></button></div>

    <div id="mute"></div>

    <audio id="alarm">
        <source src="https://josetxu.com/demos/sounds/self-destruct-alarm-count.mp3" type="audio/mpeg">
    </audio>
    
    <script src="main.js"></script>

</body>
</html>
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Love</title>
    <link rel="stylesheet" href="main2.css">
    <link rel="shortcut icon" href="./icon.png" type="image/x-icon">
</head>
<body>
    <canvas></canvas>
    
    <h1 aria-label="Sarah Fossheim">
      <span aria-hidden="true">
        <span style="--index: 1s">I</span>
      </span>  
        <span aria-hidden="true" class="spacing"  style="--index: 1.1"></span>
      <span aria-hidden="true">
        <span style="--index: 1.2s">L</span>
        <span style="--index: 1.3s">O</span>
        <span style="--index: 1.4s">V</span>
        <span style="--index: 1.5s">E</span>
      </span>  
        <span aria-hidden="true" class="spacing"  style="--index: 1.6"></span>
      <span aria-hidden="true">
        <span style="--index: 1.7s">Y</span>
        <span style="--index: 1.8s">O</span>
        <span style="--index: 1.9s">U</span>
      </span>  
        <span aria-hidden="true" class="spacing"  style="--index: 2"> </span>
      <span aria-hidden="true">
        <span style="--index: 2.1s">T</span>
        <span style="--index: 2.2s">O</span>
        <span style="--index: 2.3s">O</span>
      </span>
    
      <audio src="music.mp3" autoplay controls hidden>
      </audio>
    
    
    <script src="main2.js"></script>
</body>
</html>
body {
	margin: 0;
	padding: 0;
	width: 100vw;
	height: 100vh;
	display: flex;
	justify-content: center;
	align-items: center;
	overflow: hidden;
	background-color: #151515;
}

.base {
	background: #cacaca;
	width: 20vmin;
	border-radius: 27vmin;
	box-shadow: 0 6vmin 0.15vmin 0vmin #777, 0 4vmin 0.15vmin 0vmin #777, 0 2vmin 0.15vmin 0vmin #777;
	padding: 0vmin 2vmin 2vmin 2vmin;
	z-index: 1;
	transform: rotateX(60deg) rotateZ(0deg);
	margin-top: -4.5vmin;
	height: 22vmin;
}

button#activate {
	background: #d60505;
	border: 0;
	width: 20vmin;
	height: 19vmin;
	border-radius: 100%;
	position: relative;
	cursor: pointer;
	outline: none;
	z-index: 2;
	box-shadow: 0 4vmin 0.15vmin 0vmin #af0000, 0 2vmin 0.15vmin 0vmin #af0000;
	top: -2.5vmin;
	border: 0.5vmin solid #af0000a1;
	transition: all 0.25s ease 0s;
}

button#activate:hover {
	box-shadow: 0 3vmin 0.15vmin 0vmin #af0000, 0 1vmin 0.15vmin 0vmin #af0000;
	top: -1.5vmin;
	transition: all 0.5s ease 0s;
}
button#activate:active, button#activate.pushed {
	box-shadow: 0 1vmin 0.15vmin 0vmin #af0000, 0 1vmin 0.15vmin 0vmin #af0000;
	top: 0.5vmin;
	transition: all 0.25s ease 0s;
}
button#activate.pushed {
	box-shadow: 0 0 20px 10px #ff3c3c, 0 0 100px 50px #ff2828;
	background: #ff0000;
	border-bottom: 3px solid #00000020;
}


.box {
	transform: rotateX(-35deg) rotateY(45deg) rotateZ(0deg) rotate3d(1, 0, 0, 90deg);
	transform-origin: center top;
	transform-style: preserve-3d;
	width: 45vmin;
	position: absolute;
	z-index: 5;
	margin-top: 27vmin;
	transition: transform 1s ease 0s;
	cursor: pointer;
	height: 45vmin;
	margin-left: -32vmin;
}

.box.opened {
  transform: rotateX(-35deg) rotateY(45deg) rotateZ(0deg) rotate3d(1, 0, 0, 180deg);
}

.box div {
	position: absolute;
	width: 45vmin;
	height: 45vmin;
	background: #00bcd47d;
	opacity: 0.5;
	border: 3px solid #00a4b9;
	border-radius: 3px;
	box-sizing: border-box;
	box-shadow: 0 0 3px 0 #00bcd48a;
}

.box > div:nth-child(1) {
	opacity: 0;
}
.box > div:nth-child(2) {
	transform: rotateX(90deg) translate3d(0px, 5vmin, 5vmin);
	height: 10vmin;
}
.box > div:nth-child(3) {
	transform: rotateX(0deg) translate3d(0, 0, 10vmin);
}
.box > div:nth-child(4) {
	transform: rotateX(270deg) translate3d(0px, -5vmin, 40vmin);
	height: 10vmin;
}
.box > div:nth-child(5) {
	transform: rotateY(90deg) translate3d(-5vmin, 0, 40vmin);
	width: 10vmin;
}
.box > div:nth-child(6) {
	transform: rotateY(-90deg) translate3d(5vmin, 0vmin, 5vmin);
	width: 10vmin;
}




.grid {
	background:repeating-linear-gradient(150deg, rgba(255,255,255,0) 0, rgba(255,255,255,0) 49px, rgb(255 255 255 / 10%) 50px ,rgb(0 0 0 / 30%) 51px , rgba(255,255,255,0) 55px ), repeating-linear-gradient(30deg, rgba(255,255,255,0) 0, rgba(255,255,255,0) 49px, rgb(255 255 255 / 10%) 50px ,rgb(0 0 0 / 30%) 51px , rgba(255,255,255,0) 55px );
	position: fixed;
	width: 200vw;
	height: 150vh;
}


.warning {
	position: absolute;
	z-index: 0;
	width: 45vmin;
	height: 45vmin;
	background: repeating-linear-gradient(-45deg, black, black 3vmin, yellow 3vmin, yellow 6vmin);
	transform: rotateX(-35deg) rotateY(45deg) rotateZ(0deg) rotate3d(1, 0, 0, 90deg);
	box-shadow: 0 0 0 3vmin #af0000;
}

.warning:before {
	content: "";
	width: 80%;
	height: 80%;
	background: linear-gradient(45deg, #000000 0%, #414141 74%);
	float: left;
	margin-top: 10%;
	margin-left: 10%;
	border: 1vmin solid yellow;
	border-radius: 1vmin;
	box-sizing: border-box;
}

.warning:after {
	content: "WARNING:\2009 DANGER";
	color: white;
	transform: rotate(90deg);
	float: left;
	background: #af0000;
	position: absolute;
	bottom: 18.5vmin;
	left: -35vmin;
	font-size: 5vmin;
	font-family: Arial, Helvetica, serif;
	width: 49vmin;
	text-align: center;
	padding: 1vmin;
	text-shadow: 0 0 1px #000, 0 0 1px #000, 0 0 1px #000;
}





.hinges {
  position: absolute;
	z-index: 3;
	transform: rotateX(-35deg) rotateY(45deg) rotateZ(0deg) rotate3d(1, 0, 0, 90deg);
}


.hinges:before, .hinges:after {
	content: "";
	background: #2b2b2b;
	width: 5vmin;
	height: 1.5vmin;
	position: absolute;
	margin-top: -24.5vmin;
	z-index: 5;
	border: 2px solid #00000010;
	border-radius: 5px 5px 0 0;
	box-sizing: border-box;
	margin-left: -16.25vmin;
}
.hinges:after {
  margin-left: 13.75vmin;
  margin-top: -24.5vmin;
}


.box > span:before, .box > span:after {
	content: "";
	width: 5vmin;
	height: 1.5vmin;
	background: #103e4480;
	position: absolute;
	margin-left: 6vmin;
	border-radius: 0 0 5px 5px;
}
.box > span:after  {
  margin-left: 36vmin;
}

.box > span {
  transform: rotateX(89deg) translate(0.3vmin, 0.3vmin);
  position: absolute;
}





.text {
	position: absolute;
	margin-top: 55vmin;
	color: white;
	font-family: Arial, Helvetica, serif;
	font-size: 5vmin;
	text-shadow: 0 0 1px #000, 0 0 1px #000, 0 0 1px #000;
	perspective-origin: left;
	background: #af0000;
	padding: 1vmin;
	transform: rotateX(-35deg) rotateY(45deg) rotateZ(0deg) rotate3d(1, 0, 0, 90deg) translate(33.5vmin, -2vmin);
	text-align: center;
	width: 49vmin;
	
}

div#panel:before {
	content: "DO YOU LOVE ME";
	top: 3vmin;
	position: relative;
	font-size: 8vmin;
	width: 100vw;
	left: 0;
	z-index: 6;
	text-shadow: 0 0 1px #fff, 0 0 3px #fff;
	border-bottom: 1vmin dotted #fff;
}

#panel {
	position: absolute;
	background: #ff0000d0;
	color: #ffffff;
	font-family: Arial, Helvetica, serif;
	width: 90vmin;
	box-sizing: border-box;
	font-size: 3.25vmin;
	padding: 1vmin 2vmin;
	height: 60vmin;
	box-shadow: 0 0 0 100vmin #ff000060, 0 0 0 5vmin #ff000060;
	z-index: 5;
	display: none;
	text-align: center;
	text-shadow: 0 0 1px #fff, 0 0 3px #fff, 0 0 5px #fff;
	animation: warning-ligth 1s 0s infinite;
}

#panel.show {
	display: block !important;
}

#panel2 {
    position: absolute;
	background: #ff0000d0;
	color: #ffffff;
	font-family: Arial, Helvetica, serif;
	width: 90vmin;
	box-sizing: border-box;
	font-size: 3.25vmin;
	padding: 1vmin 2vmin;
	height: 60vmin;
	box-shadow: 0 0 0 100vmin #ff000060, 0 0 0 5vmin #ff000060;
	z-index: 5;
	display: none;
	text-align: center;
	text-shadow: 0 0 1px #fff, 0 0 3px #fff, 0 0 5px #fff;
	animation: warning-ligth 1s 0s infinite;
}

#panel2.show {
    display: block !important;
}

div#panel2::before {
    content: "WARNING";
	top: 3vmin;
	position: relative;
	font-size: 10vmin;
	width: 100vw;
	left: 0;
}

#msg {
	margin-top: 5vmin;
	text-shadow: 0 0 2px #fff;
    font-size: 50px;
}

#time {
	font-size: 10vmin;
	background: #00000080;
	max-width: 35vmin;
	margin: 6vmin auto 5vmin !important;
	position: relative;
	border-radius: 0.25vmin;
	text-shadow: 0 0 3px #000, 0 0 2px #000, 0 0 3px #000, 0 0 4px #000, 0 0 5px #000;
	padding: 1vmin 0;
}

#time:before {
	content: "00:0";
}

#abort {
	background: #ffffffb8;
	color: #d30303;
	cursor: pointer;
	padding: 1vmin 2.75vmin;
	font-size: 6vmin;
	border-radius: 0.25vmin;
	font-weight: bold;
	animation: highlight 1s 0s infinite;
}

#abort:hover {
  background: #ffffff;
	box-shadow: 0 0 15px 5px #fff;
}

#no {
    background: #ffffffb8;
	color: #d30303;
	cursor: pointer;
	padding: 1vmin 2.75vmin;
	font-size: 6vmin;
	border-radius: 0.25vmin;
	font-weight: bold;
	animation: highlight 1s 0s infinite;
}

#no:hover {
    background: #ffffff;
	box-shadow: 0 0 15px 5px #fff;
}

#again {
    background: #ffffffb8;
	color: #d30303;
	cursor: pointer;
	padding: 1vmin 2.75vmin;
	font-size: 6vmin;
	border-radius: 0.25vmin;
	font-weight: bold;
	animation: highlight 1s 0s infinite;
    position: absolute;
    top: 70%;
    right: 22%;
}

#again:hover {
    background: #ffffff;
	box-shadow: 0 0 15px 5px #fff;
}


@keyframes highlight {
	50% { box-shadow: 0 0 15px 5px #fff;}
}








div#turn-off {
	position: fixed;
	background: #ffffff80;
	left: 0;
	width: 100vw;
	height: 0vh;
	z-index: 7;
}

div#turn-off:before, div#turn-off:after {
	content: "";
	position: fixed;
	left: 0;
	top: 0;
	height: 0vh;
	background: #000;
	width: 100vw;
	transition: height 0.5s ease 0s;
}
div#turn-off:after {
	top: inherit;
	bottom: 0;
}


div#turn-off.close {
	height: 100vh;
}

div#turn-off.close:before, div#turn-off.close:after {
	transition: height 0.1s ease 0.1s;
	height: 49.75vh;
}




#time.crono {
	background: #ffffffba;
	transition: background 0.5s ease 0s;
	color: #ff0000;
	text-shadow: 0 0 1px #ffffff, 0 0 2px #ffffff, 0 0 2px #ffffff;
}
#detonate {
	display: none;
	color: #fff;
	z-index: 5;
	font-size: 8vmin;
	font-family: Arial, Helvetica, serif;
	text-shadow: 0 0 1px #fff, 0 0 2px #fff, 0 0 3px #fff;
}	
#detonate.show {
	display: block;
	animation: blink 0.25s 0s infinite;
}	

#abort.hide {
	display: none;
}

#no.hide {
    display: none;
}

#again.hide {
    display: none;
}


@keyframes blink {
	50% { opacity: 0;}
}








#closing {
	width: 100vw;
	height: 100vh;
	left: 0;
	position: absolute;
}

div#closing:before, div#closing:after {
	content: "";
	width: 50vw;
	height: 1.5vh;
	left: -50vw;
	top: 49vh;
	position: absolute;
	background: #000000;
	z-index: 7;
	transition: left 0.2s ease 0s;
}

div#closing:after {
	right: -50vw;
	transition: right 0.2s ease 0s;
	left: initial;
}


div#closing.close:before {
	left: 0;
	transition: left 0.2s ease 0.2s;
}


div#closing.close:after {
	right: 0;
	transition: right 0.2s ease 0.2s;
}



#restart {
	position: absolute;
	z-index: 8;
	display: none;
}
#reload {
	position: absolute;
	z-index: 8;
	width: 10vmin;
	height: 10vmin;
	border-radius: 100%;
	border: 0;
	margin-top: -5vmin;
	margin-left: -2.5vmin;
	opacity: 0;
	cursor: pointer;
	transform: rotate(0deg);
	transition: transform 0.5s ease 0s;
	outline: none;
}
#reload:hover {
	background: #ef0000;
	transform: rotate(360deg);
	transition: transform 0.5s ease 0s;
}
#restart.show { 
	display: block; 
}

#restart.show #reload {  
	animation: refresh 3.5s 0s 1; 
	opacity:1;
}


@keyframes refresh {
		0% { opacity: 0; }
	 50% { opacity: 0; }
	100% { opacity: 1; }
}


button#reload:before {
	content: "";
	width: 6vmin;
	height: 6vmin;
	position: absolute;
	left: 2vmin;
	top: 2vmin;
	border-radius: 100%;
	border: 1vmin solid #000;
	box-sizing: border-box;
	border-bottom-color: transparent;
}

button#reload:after {
	content: "";
	border: 1.25vmin solid transparent;
	border-top: 2vmin solid black;
	position: absolute;
	transform: rotate(40deg) translate(0.5vmin, 1.25vmin);
}





@keyframes warning-ligth {
	 0% { box-shadow: 0 0 0 100vmin #ff000060, 0 0 0 5vmin #ff000060; }
	50% { box-shadow: 0 0 0 100vmin #ff000020, 0 0 0 5vmin #ff000020; }
}



#mute {
    position: absolute;
    bottom: 1vmin;
    right: 1vmin;
    background: #8bc34a80;
    width: 6vmin;
    height: 6vmin;
    cursor: pointer;
    border: 0.5vmin solid #151515;
}
#mute.muted {
    background: #ff000080;
}

#mute:before {
    content: "";
    border: 0.75vmin solid transparent;
    height: 2vmin;
    border-right: 2vmin solid #151515;
    position: absolute;
    border-left-width: 0;
    top: 1.25vmin;
    right: 1.25vmin;
}
#mute:after {
    content: "";
    border: 0vmin solid transparent;
    height: 2vmin;
    border-right: 1.5vmin solid #151515;
    position: absolute;
    top: 2vmin;
    right: 3.5vmin;
}


#abort a {
    text-decoration: none;
    color: #d30303;
}
var theCount;
var alarm = document.getElementById("alarm");
var panel = document.getElementById("panel");
var turnOff = document.getElementById("turn-off");
var turnOffHor = document.getElementById("closing");
var detonate = document.getElementById("detonate");
var again = document.getElementById("again");
var panel2 = document.getElementById("panel2");
alarm.volume = 0.5; //volume level

var time = document.getElementById("time");
function showCountDown() {
	time.innerText = time.innerText - 1;
	if (time.innerText == 0) {
		clearInterval(theCount);
		time.classList.add("crono");
		abort.classList.add("hide");
        no.classList.add("hide");
        again.classList.add("hide");
        
		
        detonate.classList.add("show");
		setTimeout(function () {
			turnOff.classList.add("close");
			turnOffHor.classList.add("close");
			reload.classList.add("show");
			alarm.pause();
		}, 1500);
	}
   
}

var cover = document.getElementById("cover");
cover.addEventListener("click", function () {
	if (this.className == "box") this.classList.add("opened");
	else this.classList.remove("opened");
});

var btn = document.getElementById("activate");
activate.addEventListener("click", function () {
	this.classList.add("pushed");
	alarm.load();
	alarm.currentTime = 10.1;
	alarm.play();
	setTimeout(function () {
		panel.classList.add("show");
		theCount = setInterval(showCountDown, 1000);
		alarm.load();
		alarm.play();
	}, 500);
});

var abort = document.getElementById("abort");
abort.addEventListener("click", function () {
	btn.classList.remove("pushed");
	panel.classList.remove("show");
	clearInterval(theCount);
	time.innerText = 9;
	alarm.pause();
	alarm.currentTime = 10;
	alarm.play();
   
});

var no = document.getElementById("no");
no.addEventListener("click", function () {
	btn.classList.remove("pushed");
	panel.classList.remove("show");
	clearInterval(theCount);
	time.innerText = 9;
	alarm.pause();
	alarm.currentTime = 10;
	alarm.play();
    panel2.classList.add("show");
});

var again = document.getElementById("again");
again.addEventListener("click", function () {
	btn.classList.remove("pushed");
	panel2.classList.remove("show");
    no.classList.remove("pushed");
	clearInterval(theCount);
	time.innerText = 9;
	alarm.pause();
	alarm.currentTime = 10;
	alarm.play();
    
    
    btn.classList.add("pushed");
	alarm.load();
	alarm.currentTime = 10.1;
	alarm.play();
	setTimeout(function () {
		panel.classList.add("show");
		theCount = setInterval(showCountDown, 1000);
		alarm.load();
		alarm.play();
	}, 500);
});




var reload = document.getElementById("restart");
reload.addEventListener("click", function () {
    panel.classList.remove("show");
	turnOff.classList.remove("close");
	turnOffHor.classList.remove("close");
	abort.classList.remove("hide");
    no.classList.remove("hide");
    
    
	
    detonate.classList.remove("show");
	cover.classList.remove("opened");
	btn.classList.remove("pushed");
	this.classList.remove("show");
	time.classList.remove("crono");
	time.innerText = 9;
});

setTimeout(function () {
	cover.classList.remove("opened");
}, 100);

var mute = document.getElementById("mute");
mute.addEventListener("click", function () {
	if (this.className == "muted") {
		alarm.muted = false;
		this.classList.remove("muted");
	} else {
		alarm.muted = true;
		this.classList.add("muted");
	}
});
x
body{
    overflow: hidden;
    margin: 0;
  }
  h1{
    position: fixed;
    top: 50%;
    left: 0;
    width: 100%;
    text-align: center;
    transform:translateY(-50%);
    font-family: 'Love Ya Like A Sister', cursive;
    font-size: 40px;
    color: #c70012; 
    padding: 0 20px;
  }
  @media (min-width:1200px){
    h1{
      font-size: 60px;
    }
  }







  * {
    padding: 0;
    margin: 0;
  }
  
  body {
    background-color:bisque;
  }
  
  h1 {
    font-family: 'Love Ya Like A Sister', cursive;
    font-size: 7em;
    font-weight: 50px;
    text-align: center;
    margin-top: 2em;
    font-weight: 600;
    position: fixed;
    top: 50%;
    left: 0;
    width: 100%;
    text-align: center;
    transform:translateY(-200%);
    
  }
  
  h1 span {
    display: inline-block;
  }
  
  h1 span span{
    display: inline-block;
    width: auto;
    margin-right: -0.3em;
    animation: animate-characters 0.75s var(--index) forwards;
    animation-duration: 4s ;
    animation-iteration-count: infinite;
    opacity: 0;
    position: relative;
  }
  
  @keyframes animate-characters {
    0% {
      bottom: -0.7em;
      opacity: 1;
      color:azure;
    }
    
    50% {
      bottom: 0.7em;
      color:tomato;
    }
  
    100% {
      bottom: 0;
      opacity: 1;
    }
  }

  audio {
    
    position: absolute;
    top: 105%;
    right: 44%;
    animation: fadein ease 5s;
  }

  @keyframes fadein {
    from {
      opacity: 0;
    }
    to {
      opacity: 1;
    }
    
  }
  var canvas = document.querySelector("canvas"),
  ctx = canvas.getContext("2d");

var ww,wh;

function onResize(){
  ww = canvas.width = window.innerWidth;
  wh = canvas.height = window.innerHeight;
}

ctx.strokeStyle = "red";
ctx.shadowBlur = 25;
ctx.shadowColor = "hsla(0, 100%, 60%,0.5)";

var precision = 100;
var hearts = [];
var mouseMoved = false;
function onMove(e){
  mouseMoved = true;
  if(e.type === "touchmove"){
    hearts.push(new Heart(e.touches[0].clientX, e.touches[0].clientY));
    hearts.push(new Heart(e.touches[0].clientX, e.touches[0].clientY));
  }
  else{
    hearts.push(new Heart(e.clientX, e.clientY));
    hearts.push(new Heart(e.clientX, e.clientY));
  }
}

var Heart = function(x,y){
  this.x = x || Math.random()*ww;
  this.y = y || Math.random()*wh;
  this.size = Math.random()*2 + 1;
  this.shadowBlur = Math.random() * 10;
  this.speedX = (Math.random()+0.2-0.6) * 8;
  this.speedY = (Math.random()+0.2-0.6) * 8;
  this.speedSize = Math.random()*0.05 + 0.01;
  this.opacity = 1;
  this.vertices = [];
  for (var i = 0; i < precision; i++) {
    var step = (i / precision - 0.5) * (Math.PI * 2);
    var vector = {
      x : (15 * Math.pow(Math.sin(step), 3)),
      y : -(13 * Math.cos(step) - 5 * Math.cos(2 * step) - 2 * Math.cos(3 * step) - Math.cos(4 * step)) 
    }
    this.vertices.push(vector);
  }
}

Heart.prototype.draw = function(){
  this.size -= this.speedSize;
  this.x += this.speedX;
  this.y += this.speedY;
  ctx.save();
  ctx.translate(-1000,this.y);
  ctx.scale(this.size, this.size);
  ctx.beginPath();
  for (var i = 0; i < precision; i++) {
    var vector = this.vertices[i];
    ctx.lineTo(vector.x, vector.y);
  }
  ctx.globalAlpha = this.size;
  ctx.shadowBlur = Math.round((3 - this.size) * 10);
  ctx.shadowColor = "hsla(0, 100%, 60%,0.5)";
  ctx.shadowOffsetX = this.x + 1000;
  ctx.globalCompositeOperation = "screen"
  ctx.closePath();
  ctx.fill()
  ctx.restore();
};


function render(a){
  requestAnimationFrame(render);
  
  hearts.push(new Heart())
  ctx.clearRect(0,0,ww,wh);
  for (var i = 0; i < hearts.length; i++) {
    hearts[i].draw();
    if(hearts[i].size <= 0){
      hearts.splice(i,1);
      i--;
    }
  }
}



onResize();
window.addEventListener("mousemove", onMove);
window.addEventListener("touchmove", onMove);
window.addEventListener("resize", onResize);
requestAnimationFrame(render);
