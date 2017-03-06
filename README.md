<DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <style>
      body {
         background-color: white;
      }
      
      h1 {
         text-align: center;
         padding-top: 100px;
      {
      
      .normal {                    <!--These are all the original styles for the page, not included in the .css stylesheet-->
         font-size: 12px;
         color: black;
         background: white;
         padding-left: 15px;
      }
      
      a {
        color: black;
      }
      
      a:hover {
        color: gray;
        text-decoration: none;
      }
      
      .fade-out {
        opacity: 0;
        transition: none;
      }
      
      span {
         display: block;
      }
      
      div.relative {
        position: relative;
        left: 30px;
      }
      
      .slides {
        display: none;
      }
      
      .center {
         text-align: center;
      }
      
      .fade {
        webkit-animation-name: fade;
        webkit-animation-duration: 2s;
        animation-name: fade;
        animation-duration: 2s;
      }
      
      @-webkit-keyframes {
        from {opacity: .2;}
        to {opacity: 1;}
      }
      
      @keyframes fade {
        from {opacity: .2;}
        to {opacity: 1;}
      }
      
      
                                   <!--Down to this point.-->
    </style>
    <title>Call It Photography</title>
    <link rel="stylesheet" type="text/css" href="Style.css">
    
    <script>
      
      function load() {
        var opacity = 0.0;
        document.body.style.opacity = 1;
        document.body.style.transition = '2s opacity';
      }
      
      window.onload = load;
    </script>
    
  </head>
  <body id="mainContainer" class="fade-out">
    <main>
      
    <h1 id="large"><img src="Call it.PNG" alt="First Picture"/> </h1>
    
    <ul style="text-align: center;list-style-type: none;">
      <li id="links" style="list-style-type: none;text-align:center;display: inline;">
        <span style="padding-right: 30px;"><a style="font-size: 18px;color: black;text-decoration: none;" href="index.html">Home</a></span>
        <span style="padding-right: 30px;"><a style="font-size: 18px;color: black;text-decoration: none;" href="photos.html">Photos</a></span>
        <span style="padding-right: 30px;"><a style="font-size: 18px;color: black;text-decoration: none;" href="prices.html">Prices</a></span>
        <a style="font-size: 18px;color: black;text-decoration: none;" href="contact.html">Contact Me</a>
      </li>
    </ul>
    
    <div style="border-top: thin solid black;"/>
    
    <h2>Introduction</h2>
    <p id="p1">Call It Photography</p>
    
    
    <br>
    <br>
    <span class="normal">pictures of you</span> <br>
    <span class="normal">pictures of me</span>
    <br>
    <br><br><br><br><br>
    
    <h3>My Pictures</h3>
    <div style="text-align:center;max-width: 500px">
      <div class="fade">
        <img class="slides" src="1.JPG" alt="First Picture" style="width:100%;">
        </div>
      <div class="fade">
        <img class="slides" src="2.JPG" alt="Second Picture" style="width:100%;">
        </div>
      <div class="fade">
        <img class="slides" src="3.JPG" alt="Third Picture" style="width:100%;">
        </div>
      <div class="fade">
        <img class="slides" src="4.JPG" alt="Fourth Picture" style="width:100%;">
        </div>
      <div class="fade">
        <img class="slides" src="5.JPG" alt="Fourth Picture" style="width:100%;">
        </div>
      <div class="fade">
        <img class="slides" src="6.JPG" alt="Fourth Picture" style="width:100%;">
        </div>
      <div class="fade">
        <img class="slides" src="7.JPG" alt="Fourth Picture" style="width:100%;">
        </div>
        <!--<img class="slides" src="7.JPG" alt="Seventh Picture" style="width:100%;">-->
        <!--<img class="slides" src="8.JPG" alt="Eighth Picture" style="width:100%;">-->
        <!--<img class="slides" src="9.JPG" alt="Ninth Picture" style="width:100%;">-->
    </div>
    <script>
      var slide = 0;
      changePicture();

      function changePicture() {
        var number = 0;
        var slideNumber = document.getElementsByClassName("slides");
        
        for (var i = 0; i < slideNumber.length; i++) {
          slideNumber[i].style.display = "none";
        }
        
        slide++;
        if (slide > slideNumber.length) {
          slide = 1;
        }
        
        slideNumber[slide-1].style.display = "inline-block";
        setTimeout(changePicture, 3000);
      }
    </script>
    <br>
    
    <hr>
    <a href="../index.html">Home Directory</a>
    <br>
    </main>
  </body>
</html>
