<!DOCTYPE html>
<html lang="en-us">
 
<head>
<meta charset="utf-8">
<title>Bouncing Clouds</title>
<script src="http://www.kirupa.com/js/prefixfree.min.js"></script>
 
<style>
#mainContent {
    background-color: #A2BFCE;
    border-radius: 4px;
    padding: 10px;
    width: 600px;
    height: 300px;
    overflow: hidden;
}
.cloud {
    position: absolute;
}
#bigcloud {
	animation: bobble 2s infinite;
    margin-left: 100px;
    margin-top: 15px;
}
#smallcloud {
    animation: bobble 4s infinite;
    margin-top: 65px;
    margin-left: 200px;
}

@keyframes bobble {
    0% {
        transform: translate3d(50px, 40px, 0px);
        animation-timing-function: ease-in;
    }
    50% {
        transform: translate3d(50px, 50px, 0px);
        animation-timing-function: ease-out;
    }
    100% {
        transform: translate3d(50px, 40px, 0px);
    }
}

.animated {
  transition: background-color 2s;
  -webkit-transition: background-color 2s;
  -o-transition: background-color 2s;
  -moz-transition: 2s;
}


</style>
</head>
 
<body>
    <div id="mainContent">
        <img id="bigcloud" alt="#" class="cloud" height="154" src="http://www.kirupa.com/images/bigCloud.png" width="238">
		 <img id="smallcloud" alt="#" class="cloud" height="103" src="http://www.kirupa.com/images/smallCloud.png" width="158">
    </div>
	
	<div class="animated" onclick="this.style.background='green'">
  <span style="font-size:150%">Click to animate (no IE, no FF&lt;4)</span>
</div>

	
</body>
 
</html>
