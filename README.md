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
      
      .slides {
        display: none;
      }
      
      .center {
         text-align: center;
      }
      
      .fade {
        -webkit-animation-name: fade;
        -webkit-animation-duration: 2s;
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
    <hr>
    
    <h2>Introduction</h2>
    <p id="p1">Call It Photography</p>
    <br>
    <br>
    <div style="margin-left: auto;margin-right: auto;max-width: 500px;max-height: 600px">
      <div class="slides fade">
        <img src="1.JPG" alt="First Picture" style="width:100%;">
        </div>
      <div class="slides fade">
        <img src="2.JPG" alt="Second Picture" style="width:100%;">
        </div>
      <div class="slides fade">
        <img src="3.JPG" alt="Third Picture" style="width:100%;">
        </div>
      <div class="slides fade">
        <img src="4.JPG" alt="Fourth Picture" style="width:100%;">
        </div>
      <div class="slides fade">
        <img src="5.JPG" alt="Fifth Picture" style="width:100%;">
        </div>
      <div class="slides fade">
        <img src="6.JPG" alt="Sixth Picture" style="width:100%;">
        </div>
      <div class="slides fade">
        <img src="7.JPG" alt="Seventh Picture" style="width:100%;">
        </div>
      <div class="slides fade">
        <img src="8.JPG" alt="Eighth Picture" style="width:100%;">
        </div>
      <div class="slides fade">
        <img src="9.JPG" alt="Ninth Picture" style="width:100%;">
        </div>
      <div class="slides fade">
        <img src="10.JPG" alt="Tenth Picture" style="width:100%;">
        </div>
      <div class="slides fade">
        <img src="11.JPG" alt="11 Picture" style="width:100%;">
        </div>
      <div class="slides fade">
        <img src="12.JPG" alt="12 Picture" style="width:100%;">
        </div>
      <div class="slides fade">
        <img src="13.JPG" alt="13 Picture" style="width:100%;">
        </div>
      <div class="slides fade">
        <img src="14.JPG" alt="14 Picture" style="width:100%;">
        </div>
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
        setTimeout(changePicture, 4000);
      }
    </script>
    <br>
    
    </main>
  </body>
</html>
