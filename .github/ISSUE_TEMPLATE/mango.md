---
name: Mango
about: Mango Logo

---

<head>

  <meta charset="UTF-8">
  <link rel="shortcut icon" type="image/x-icon" href="https://static.codepen.io/assets/favicon/favicon-8ea04875e70c4b0bb41da869e81236e54394d63638a1ef12fa558a4a835f1164.ico">
  <link rel="mask-icon" type="" href="https://static.codepen.io/assets/favicon/logo-pin-f2d2b6d2c61838f7e76325261b7195c27224080bc099486ddd6dccb469b8e8e6.svg" color="#111">
  <title>CodePen - Mango 2015</title>
  
  
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css">

  
      <style>
      @import url(https://fonts.googleapis.com/css?family=Montserrat:400,700);
body {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  /*	&:before {
  		position: fixed;
  		top: 0;
  		bottom: 0;
  		left: 50%;
  		width: 2px;
  		height: 100vh;
  		background: rgba(black, .05);
  		content: "";
  	}*/
}

h1 {
  font: bold 10vw Montserrat;
  pointer-events: none;
  cursor: default;
}

span {
  display: inline-block;
  position: relative;
  transition: 0.3s;
}
span:after {
  position: absolute;
  top: calc(50% -  2.5vw);
  left: calc(50% - 2.5vw);
  content: "";
  width: 5vw;
  height: 5vw;
  background: currentColor;
  border-radius: 50%;
  -webkit-transform: scale(0) translateX(0);
          transform: scale(0) translateX(0);
  transition: inherit;
}
span:before {
  display: block;
  -webkit-transform: scale(1);
          transform: scale(1);
  transition: inherit;
}
span:nth-child(1) {
  transition-delay: 0.05s;
}
span:nth-child(1):before {
  content: "M";
}
span:nth-child(2) {
  transition-delay: 0.1s;
}
span:nth-child(2):before {
  content: "a";
}
span:nth-child(3) {
  transition-delay: 0.15s;
}
span:nth-child(3):before {
  content: "n";
}
span:nth-child(4) {
  transition-delay: 0.2s;
}
span:nth-child(4):before {
  content: "g";
}
span:nth-child(5) {
  transition-delay: 0.25s;
}
span:nth-child(5):before {
  content: "o";
}
span:nth-child(6) {
  transition-delay: 0.3s;
}
span:nth-child(6):before {
  content: "_";
}

.go span {
  -webkit-animation: float 1.2s ease-in-out infinite;
          animation: float 1.2s ease-in-out infinite;
}
.go span:before {
  -webkit-transform: scale(0);
          transform: scale(0);
}
.go span:after {
  -webkit-transform: scale(1);
          transform: scale(1);
}
.go span:nth-child(4), .go span:nth-child(6) {
  -webkit-transform: scale(0);
          transform: scale(0);
  transition-duration: 0.075s;
  -webkit-transform-origin: center right;
          transform-origin: center right;
  -webkit-animation: none;
          animation: none;
}
.go span:nth-child(1):after {
  -webkit-transform: scale(1) translateX(60%);
          transform: scale(1) translateX(60%);
}
.go span:nth-child(2) {
  -webkit-animation-delay: 0.09s;
          animation-delay: 0.09s;
}
.go span:nth-child(2):after {
  -webkit-transform: scale(1) translateX(95%);
          transform: scale(1) translateX(95%);
}
.go span:nth-child(3) {
  -webkit-animation-delay: 0.18s;
          animation-delay: 0.18s;
}
.go span:nth-child(3):after {
  -webkit-transform: scale(1) translateX(140%);
          transform: scale(1) translateX(140%);
}
.go span:nth-child(5) {
  -webkit-animation-delay: 0.27s;
          animation-delay: 0.27s;
}
.go span:nth-child(5):after {
  -webkit-transform: scale(1) translateX(55%);
          transform: scale(1) translateX(55%);
}

span:nth-child(1), span:nth-child(4) {
  color: #4285F4;
}
span:nth-child(2), span:nth-child(6) {
  color: #EA4335;
}
span:nth-child(3) {
  color: #FBBC05;
}
span:nth-child(5) {
  color: #34A853;
}

@-webkit-keyframes float {
  from, to {
    -webkit-transform: none;
            transform: none;
  }
  25%, 75% {
    -webkit-transform: translateY(-10%);
            transform: translateY(-10%);
  }
  50% {
    -webkit-transform: translateY(10%);
            transform: translateY(10%);
  }
}

@keyframes float {
  from, to {
    -webkit-transform: none;
            transform: none;
  }
  25%, 75% {
    -webkit-transform: translateY(-10%);
            transform: translateY(-10%);
  }
  50% {
    -webkit-transform: translateY(10%);
            transform: translateY(10%);
  }
}

    </style>

  <script>
  window.console = window.console || function(t) {};
</script>

  
  
  <script>
  if (document.location.search.match(/type=embed/gi)) {
    window.parent.postMessage("resize", "*");
  }
</script>


</head>

<body translate="no">

  <h1><span data-letter="1"></span><span data-letter="2"></span><span data-letter="3"></span><span data-letter="4"></span><span data-letter="5"></span></h1>
    <script src="//static.codepen.io/assets/common/stopExecutionOnTimeout-b2a7b3fe212eaa732349046d8416e00a9dec26eb7fd347590fbced3ab38af52e.js"></script>

  <script src="//cdnjs.cloudflare.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>

  

    <script>
      setTimeout(function(){
	$("html").addClass("go");

	setTimeout(function(){
		$("html").removeClass("go");			
	}, 3300);

}, 600);

$("html").hover(
	function() {
		$(this).addClass("go");
	},
	function() {
		$(this).removeClass("go");
	}
);
      //# sourceURL=pen.js
    </script>



  
  




 </body>
