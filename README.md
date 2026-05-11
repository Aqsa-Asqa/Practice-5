<!DOCTYPE html>
<html>

<head>
  <title>Birthday Surprise 🎂</title>

  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #ffe6f0;
      text-align: center;
      padding-top: 100px;
    }

    .page {
      display: none;
    }

    h1 {
      color: #ff4081;
    }

    p {
      font-size: 24px;
    }

    button {
      display: block;
      margin: 15px auto;
      padding: 12px 25px;
      font-size: 18px;
      border: none;
      border-radius: 10px;
      background-color: #ff4081;
      color: white;
      cursor: pointer;
      width: 250px;
    }

    button:hover {
      background-color: #e91e63;
    }
  </style>
</head>

<body>

  <!-- PAGE 1 -->
  <div id="page1" class="page" style="display:block;">
    <h1>Question 1 😄</h1>

    <p>Who is the most amazing person?</p>

    <button onclick="showPage('page2')">Me 😎</button>
    <button onclick="showPage('page2')">Definitely Me ✨</button>
    <button onclick="showPage('page2')">Obviously Me 😂</button>
  </div>

  <!-- PAGE 2 -->
  <div id="page2" class="page">
    <h1>Question 2 🎁</h1>

    <p>What do you deserve today?</p>

    <button onclick="showPage('page3')">Cake 🎂</button>
    <button onclick="showPage('page3')">Gifts 🎁</button>
    <button onclick="showPage('page3')">Everything 💖</button>
  </div>

  <!-- PAGE 3 -->
  <div id="page3" class="page">
    <h1>Final Question ✨</h1>

    <p>Ready for your birthday surprise?</p>

    <button onclick="showPage('page4')">YESSSS 😍</button>
    <button onclick="showPage('page4')">Absolutely 🎉</button>
    <button onclick="showPage('page4')">Show Me 👀</button>
  </div>

  <!-- PAGE 4 -->
  <div id="page4" class="page">
    <h1>Happy Birthday 🎉</h1>

    <p>Dear Friend,</p>

    <p>You are amazing and I’m so lucky to have you! 💖</p>

    <p>
      May your life always be full of happiness,
      laughter and success ✨
    </p>

    <p>Enjoy your special day 🎂</p>
  </div>

  <script>
    function showPage(pageId) {

      document.getElementById("page1").style.display = "none";
      document.getElementById("page2").style.display = "none";
      document.getElementById("page3").style.display = "none";
      document.getElementById("page4").style.display = "none";

      document.getElementById(pageId).style.display = "block";
    }
  </script>

</body>

</html>
