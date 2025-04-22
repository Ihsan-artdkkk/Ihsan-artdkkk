<!DOCTYPE html>
<html>
<head>
  <title>Surprise</title>
  <style>
    body {
      margin: 0;
      background: black;
      overflow: hidden;
    }
    #scare {
      position: fixed;
      width: 100%;
      height: 100%;
      background: url('https://i.imgur.com/Frq2Hgk.jpg') no-repeat center center;
      background-size: cover;
      display: none;
    }
  </style>
</head>
<body>
  <div id="scare"></div>
  <audio id="scream" src="https://www.soundjay.com/human/sounds/scream-01.mp3" preload="auto"></audio>
  <script>
    setTimeout(() => {
      document.getElementById('scare').style.display = 'block';
      document.getElementById('scream').play();
    }, 1000); // muncul setelah 1 detik
  </script>
</body>
</html>
