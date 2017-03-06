<DOCTYPE html>
<html>
  <head>
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
      
      .center {
         text-align: center;
      }
                                   <!--Down to this point.-->
    </style>
    <title>Call It Photography</title>
    <link rel="stylesheet" type="text/css" href="Style.css">
    
    <script>
      var randomColor = Math.floor(Math.random()*16777215).toString(16);
    </script>
    
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
    <div class="relative">
      <img src="Horses.JPG" alt="First Picture" style="width:900px;height:440px;text-align:center;"/>
    </div>
    <br>
    
    <hr>
    <a href="../index.html">Home Directory</a>
    <br>
    </main>
  </body>
</html>
