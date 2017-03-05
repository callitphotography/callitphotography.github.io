<DOCTYPE html>
<html>
  <head>
    <style>
      .normal {                    <!--These are all the original styles for the page, not included in the .css stylesheet-->
         font-size: 12px;
         color: black;
         background: white;
         padding-left: 15px;
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
        draw();
      }
      
      window.onload = load;
    </script>
    
  </head>
  <body id="mainContainer" class="fade-out">
    <main>
      
    <h1 id="large">Coilett Industries</h1>
    <h2>Introduction</h2>
    <p id="p1">Coilett Industries is a company made to help people who have disabilities or problems mentally.  We strive
    to find out why the brain is working the way it is, and want to learn how we can better fix it.</p>
    
    <script>
      document.getElementById("p1").style.color = "red";
      document.getElementById("p1").style.backgroundColor = "randomColor";
      document.getElementById("p1").style.border = "medium solid black";
    </script>
    
    <button type="button" onclick="document.getElementById('p1').style.color = 'blue'">
      Change the CSS!</button>
    <br>
    <br>
    <span class="normal">Since there are so many different opinions on the different subjects of the brain</span>
    <span class="normal">we feel it's important to post an article written by one of our own:</span>
    <br>
    <br>
    <a class="center" id="large" href="How Psychotherapy Changes the Brain.docx">How Psychotherapy Changes the Brain</a>
    <br><br><br>
    <button type="button" onclick="document.querySelector('#mainContainer').style.backgroundColor = 'orange'">Change the page</button>
    <br>
    
    <h3>Canvas API</h3>
    <h4>Now Serving: </h4>
    <div class="relative">
      <canvas id="canvas" width="350" height="400"></canvas>
    </div>
    <p>This whole section other than the headers was done using Canvas API, here's where I learned how:
    <a href="https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes">Drawing shapes</a>
    </p>
    <br>
    
    <h1>End Of Page</h1>
    <p class="important">If you really want to go to the next page just make sure you click on the link for page 2.
    The "Home Directory" link will bring you back to the original page, and the "Week 03 Team assignment" will bring
    you do the team activity for this week.</p>
    
    <a class="page2" href="FunPage.html">Continue to page 2 >> </a>
    <hr>
    <a href="../index.html">Home Directory</a>
    <br>
    </main>
  </body>
</html>
