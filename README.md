html,
body {
	width: 100%;
	height: 100%;
	outline: none;
}

body {
	background-color: #F08080;
	background: linear-gradient(to bottom, #F08080 0%, #E9967A 50%, #FF7F50 100%);
	background: -webkit-linear-gradient(top, #F08080 0%, #E9967A 50%,#FF7F50 100%);
	background: -moz-linear-gradient(top, #F08080 0%, #E9967A 50%,#FF7F50 100%);
	background: -o-linear-gradient(top, #F08080 0%, #E9967A 50%,#FF7F50 100%);
	background: -ms-linear-gradient(top, #F08080 0%, #E9967A 50%,#FF7F50 100%);
	filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#F08080', endColorstr='#FF7F50',GradientType=0);
}

.cake {
	position: absolute;
	width: 600px;
	height: 500px;
	top: 50%;
	left: 50%;
	margin-top: -250px;
	margin-left: -300px;
}

.cake > * {
	position: relative;
}

.layer, 
.icing {
	display: block;
	width: 100%;
	border-bottom-left-radius: 50%;
	border-bottom-right-radius: 50%;
	border: solid 1px #000000;
}

.layer {
	margin-top: -100px;
	height: 200px;
	background: #553c13;
	z-index: 0;
}

.bottom {
	z-index: 1;
}

.middle {
	 z-index: 2;
}

.top {
	 z-index: 3;
}

.top,
.icing {
	border-top-left-radius: 25%;
	border-top-right-radius: 25%;
}

.icing {
	margin-top: 0px;
	height: 100px;
	background: #f0e4d0;
	z-index: 4;
}

.drip {
	border-bottom-left-radius: 50%;
	border-bottom-right-radius: 50%;
	background-color: #f0e4d0;
	border-bottom: solid 1px #000000;
	z-index: 5;
}

.drip:nth-child(1) {
	width: 40px;
	height: 50px;
	margin-top: 35px;
	margin-left: -1px;
	border-left: solid 1px #000000;
	border-right: solid 1px #000000;
	transform: skewY(20deg);
}

.drip:nth-child(2) {
	width: 175px;
	height: 100px;
	margin-top: -60px;
	margin-left: 40px;
}

.drip:nth-child(3) {
	width: 200px;
	height: 100px;
	margin-top: -60px;
	margin-left: 200px;
}

.drip:nth-child(4) {
	width: 175px;
	height: 100px;
	margin-top: -130px;
	margin-left: 395px;
}

.drip:nth-child(5) {
	width: 40px;
	height: 50px;
	margin-top: -90px;
	margin-left: 559px;
	border-left: solid 1px #000000;
	border-right: solid 1px #000000;
	transform: skewY(-20deg);
}

.candle {
	position: absolute;
	width: 18px;
	height: 100px;
	top: 50%;
	left: 50%;
	margin-top: -325px;
	margin-left: -10px;
	background: #ffffff;
	border-top-left-radius: 10px;
	border-top-right-radius: 10px;
	z-index: 5;
	
}

.candle:after,
.candle:before {
	background: rgba(255, 0, 0, 0.4);
	content: "";
	position: absolute;
	width: 100%;
	height: 3px;
	border-radius: 100%;
	transform: skewY(-50deg);
}

.candle:after {
	top: 25%;
	left: 0;
}

.candle:before {
	top: 50%;
	left: 0;
}

.flame {
	border-radius: 100%;
	position: relative;
	width: 7px;
	height: 18px;
	top: 0px;
	left: 50%;
	margin-left: -3.2px;
	margin-top: -18px;
}
.flame:nth-child(1) {
	animation: flame 2s 0s infinite;
}
.flame:nth-child(2) {
	animation: flame 1.5s 0s infinite;
}
.flame:nth-child(3) {
	animation: flame 1s 0s infinite;
}
.flame:nth-child(4) {
	animation: flame 0.5s 0s infinite;
}
.flame:nth-child(5) {
	animation: flame 0.25s 0s infinite;
}

@keyframes flame {
	0%, 100% {
		background: rgba(254, 248, 97, 0.5);
		box-shadow: 0 0 40px 10px rgba(248, 233, 209, 0.2);
		transform: translateY(0) scale(1);
	}
	50% {
		background: rgba(255, 50, 0, 0.1);
		box-shadow: 0 0 40px 20px rgba(248, 233, 209, 0.2);
		transform: translateY(-20px) scale(0);
	}
}

.message {
	position: absolute;
	width: 600px;
	top: 50%;
	left: 50%;
	margin-top: 250px;
	margin-left: -300px;
	text-align: center;
	font-family: 'Leckerli One', cursive;
	font-size: 40;
	color: #f0e4d0;
}
