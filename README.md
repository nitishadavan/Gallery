# Ex.08 Design of Interactive Image Gallery
# Date:05-05-2025
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
~~~
gallery.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>image gallery</title>
    <link rel="stylesheet" href="gallery.css">
</head>
  <body>
    <center>
    <h1>GALLERY</h1>
</center>
<div class="ful-img" id="fulimgbox">
  <center>  <img src="image1.jpg" id="fulimg"></center>
  <span onclick="closefulimg()">❌</span>
</div>
<div class="gallery">
    <img src="image1.jpg" onclick="openfulimg(this.src)">
    <img src="image2.avif" onclick="openfulimg(this.src)">
    <img src="image3.avif" onclick="openfulimg(this.src)">
    <img src="image4.webp" onclick="openfulimg(this.src)">
    <img src="image5.jpg" onclick="openfulimg(this.src)">
    <img src="image6.avif" onclick="openfulimg(this.src)">
    <img src="image7.avif" onclick="openfulimg(this.src)">
    
    
</div>
  </body>
  <script>
    var fulimgbox=document.getElementById("fulimgbox");
    var fulimg=document.getElementById("fulimg");

    function openfulimg(pic){
        fulimgbox.style.display= "flex"
        fulimg.src=pic
    }
    function closefulimg(){
        fulimgbox.style.display="none";
       
    }
    
  </script>
  <footer>
   <h1> DISIGNED AND DEVELOPED BY</h1>
   <h2>D.NITISH ADAVAN</h2>
  </footer>
</html>

gallery.css
*{
    margin: 0%;
    padding: 0%;
    font-family: sans-serif;
}
h1{
    color: rgba(227, 98, 7, 0.903);
}
body{
    background-color: azure;
}
.gallery{
    width: 80%;
    margin: 100px auto 50px;
    grid-template-columns: repeat(auto-fit, minmax(260px,1fr));
     
}
.gallery img{
    width: 250px;
    cursor: pointer;
    transition: 1;
}
.gallery img:hover{
transform: scale(1.1) rotate(-360deg);
border-radius: 16px;
box-shadow: 10px 25px rgba(68, 77, 136, 0.2);
transition: ease 0.5s;
}
.ful-img{
    width: 100%;
    height: 100vh;
    background: rgba(0, 0, 0, 0.592);
    top: 0;
    left: 0;
    position: fixed;
    display: none;
    align-items: center;
    justify-content: center;
    z-index: 100;

}
.ful-img img{
    width: 600px;
    height: 600px;
    
}
.ful-img span{
    top: 5%;
    right: 5%;
    position: absolute;
    font-size: 36px;
    color: aliceblue;
    cursor: pointer;
}
.ful-img span:hover{
    transform: scale(1.8) rotate(-360deg) ;
    transition: ease 1s;
}

~~~
# OUTPUT:
![alt text](<Screenshot 2025-05-05 202426.png>)

![alt text](<Screenshot 2025-05-05 202440.png>)

![alt text](<Screenshot 2025-05-05 202504.png>)
# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
