# Un sito super speciale che fa qualcosa


<html>
<head>
  <title>Button Example</title>
  <script>
    function showText() {
      document.getElementById("hiddenText").style.display = "block";
    }
    function showText2() {
      document.getElementById("hiddenText2").style.display = "block";
    }
  </script>
</head>

<body>

  <h1>Ciao!</h1>
  <p>Questo sito fa qualcosa <br></p>

  <button onclick="showText()">Cosa fa questo sito?</button>

  <p id="hiddenText" style="display: none;">
    Questo sito ti mostra un link molto speciale! <br>
    non ti dico la password però<br>
    <br>
    https://dax-0.itch.io/velocity <br>
    
    Grazie e non scordarti paypal <br>

    <button onclick="showText2()">Non mi sembra molto impressionante</button>
  </p>

  <p id="hiddenText2" style="display: none;">
    Hai proprio degli standard alti tu <br>
    ribadisco che la password non te la dirò mai<br>
    punto esclamativo<br>
    <br>

    <button onclick="">Wow!</button>
  </p>

</body>
</html>
