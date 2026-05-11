<!DOCTYPE html>
<html>

<head>
  <title>Birthday Surprise 🎂</title>

  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      padding-top: 80px;
      margin: 0;
      overflow: hidden;

      /* Beautiful Gradient Background */
      background: linear-gradient(-45deg,
          #ff9a9e,
          #fad0c4,
          #fbc2eb,
          #a18cd1);

      background-size: 400% 400%;
      animation: gradientBG 10s ease infinite;
    }

    /* Animated Gradient */
    @keyframes gradientBG {
      0% {
        background-position: 0% 50%;
      }

      50% {
        background-position: 100% 50%;
      }

      100% {
        background-position: 0% 50%;
      }
    }

    /* Floating Balloons */
    .balloon {
      position: absolute;
      bottom: -150px;
      width: 80px;
      height: 100px;
      border-radius: 50%;
      opacity: 0.8;
      animation: float 10s infinite;
    }

    .balloon:before {
      content: "";
      position: absolute;
      width: 2px;
      height: 80px;
      background: white;
      top: 100px;
      left: 40px;
    }

    .b1 {
      background: #ff4081;
      left: 10%;
      animation-delay: 0s;
    }

    .b2 {
      background: #7c4dff;
      left: 30%;
      animation-delay: 2s;
    }

    .b3 {
      background: #ff9800;
      left: 50%;
      animation-delay: 4s;
    }

    .b4 {
      background: #00c853;
      left: 70%;
      animation-delay: 1s;
    }

    .b5 {
      background: #00b0ff;
      left: 90%;
      animation-delay: 3s;
    }

    @keyframes float {
      0% {
        transform: translateY(0);
      }

      100% {
        transform: translateY(-120vh);
      }
    }

    .page {
      display: none;
      position: relative;
      z-index: 2;
    }

    h1 {
      color: white;
      font-size: 50px;
      text-shadow: 2px 2px 10px rgba(0, 0, 0, 0.3);
    }

    p {
      font-size: 28px;
      color: white;
      text-shadow: 1px 1px 5px rgba(0, 0, 0, 0.3);
    }

    button {
      display: block;
      margin: 15px auto;
      padding: 14px 28px;
      font-size: 20px;
      border: none;
      border-radius: 50px;
      background: white;
      color: #ff4081;
      cursor: pointer;
      width: 280px;
      font-weight: bold;
      transition: 0.3s;
    }

    button:hover {
      transform: scale(1.08);
      background: #fff0f5;
    }
  </style>
</head>

<body>

  <!-- Floating Balloons -->
  <div class="balloon b1"></div>
  <div class="balloon b2"></div>
  <div class="balloon b3"></div>
  <div class="balloon b4"></div>
  <div class="balloon b5"></div>

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
