# form-validation
3<!DOCTYPE html>
<html>
    <head>
         <title>
             form
        </title>

	<style>
	.mySlides {display:none;}
	    .left{
            width: 250px;
            height:250px;
		float: left;
		
            }
	.right{
		 width:500px;
            height: 500px;
		float: right;
		}

	</style>		
    </head>
<body>
<center><h1>NEW FORM</h1>    </center>
<div class ="row">
		<div class ="col1">
<div class="left">
<img class="mySlides" src="img_snowtops.jpg" style="width:100%">
  <img class="mySlides" src="img_lights.jpg" style="width:100%">
  <img class="mySlides" src="img_mountains.jpg" style="width:100%">
  <img class="mySlides" src="img_forest.jpg" style="width:100%">

  <button class="w3-button w3-black w3-display-left" onclick="plusDivs(-1)">&#10094;</button>
  <button class="w3-button w3-black w3-display-right" onclick="plusDivs(1)">&#10095;</button>
</div>

</div>
  <div class="col2">
<div class="right">
  <form>
        <fieldset>
            <legend>AKHIL FORM</legend>
            Name:<input type="text" id="name" required=""/>
	<br>
<br>
            Email:<input type="email" />
            <br>
            <br>
		Phone:<input type="tel" id="phone" name="phone" placeholder="123-45-678" ><br><br>
		Description:<textarea  placeholder="enter text" autofocus=""></textarea><br><br>

            <button onClick="data()">submit </button>
       
        </fieldset>
    </form>
</div>
</div>
</div>
<script>
var slideIndex = 1;
showDivs(slideIndex);

function plusDivs(n) {
  showDivs(slideIndex += n);
}

function showDivs(n) {
  var i;
  var x = document.getElementsByClassName("mySlides");
  if (n > x.length) {slideIndex = 1}
  if (n < 1) {slideIndex = x.length}
  for (i = 0; i < x.length; i++) {
    x[i].style.display = "none";  
  }
  x[slideIndex-1].style.display = "block";  
}

function data()
{

var b = document.getElementById('name').value

document.write(b);

}
</script>
 </body>
</html>
