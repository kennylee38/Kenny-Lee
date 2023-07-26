<!DOCTYPE html>
<html lang="en">

	<head>
	<meta charset="UTF-8">
	<meta name="viewpoint" content="width=device-width, initial=-scale=1.0">
	<meta http-equiv="X-UA-Compatible" content="ie=edge">
	
	<script src="Favorvideo.js"defer></script>
	<link rel="stylesheet" type="text/css" href="One_page_website.css">
	</head>

		<!--home-->
		<div id="home"></div>
		<p>Hey! Over here</p>
		<p>This is my favorite dance music video!</p>
		
	<!--gallery-->
	<div id="gallery"></div>

	<div>
       <a href="https://youtu.be/OK_OyQxce7Q">Classic_Dance</a>
    </div>
		<div>
	</div>	
	
	<html>
<style>
#container {
  width: 400px;
  height: 400px;
  position: relative;
  background: yellow;
}
#animate {
  width: 50px;
  height: 50px;
  position: absolute;
  background-color: red;
}
</style>
<body>

<p><button onclick="myMove()">Click Me</button></p> 

<div id ="container">
  <div id ="animate"></div>
</div>

<script>
function myMove() {
  let id = null;
  const elem = document.getElementById("animate");   
  let pos = 0;
  clearInterval(id);
  id = setInterval(frame, 5);
  function frame() {
    if (pos == 350) {
      clearInterval(id);
    } else {
      pos++; 
      elem.style.top = pos + "px"; 
      elem.style.left = pos + "px"; 
    }
  }
}
</script>

</body>
</html>
