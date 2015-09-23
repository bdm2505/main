# main
<html>
  <head>
    <meta charset="utf-8"/>
    <title>Квадрат</title>
    <script type="text/javascript">
      function draw(){
  var canvas = document.getElementById('canvas');
  if (canvas.getContext){
     	var ctx = canvas.getContext('2d');

    	var path=new Path2D();
    	path.arc(75,75,50,0,Math.PI*2,true); // Outer circle
    	path.moveTo(110,75);
    	path.arc(75,75,35,0,Math.PI,false);  // Mouth (clockwise)
    	path.moveTo(65,65);
    	path.arc(60,65,5,0,Math.PI*2,true);  // Left eye
   	 	path.moveTo(95,65);
   	 	path.arc(90,65,5,0,Math.PI*2,true);  // Right eye
    	ctx.stroke(path);
  		}
      }
    </script>
    <style type="text/css">
      canvas { border: 1px solid black; }
    </style>
  </head>
  <body onload="draw();">
    <canvas id="tutorial" width="400" height="400"></canvas>
    <img src="http://kvadrat002.my1.ru/zd.png">
   $POWERED_BY$
  </body>
  <!-- <popup> -->
  <!-- </popup> -->
</html>
