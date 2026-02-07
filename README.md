<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Be My Valentine 💘</title>
  < style >
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(135deg, #ff758c, #ff7eb3);
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      color: white;
      text-align: center;
    }

    .box {
      background: rgba(255, 255, 255, 0.15);
      padding: 40px;
      border-radius: 20px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
      max-width: 350px;
    }

    h1 {
      font-size: 2rem;
      margin-bottom: 10px;
    }

    p {
      font-size: 1.1rem;
      margin-bottom: 30px;
    }

    button {
      padding: 12px 25px;
      margin: 10px;
      font-size: 1rem;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      transition: transform 0.2s;
    }

    button:hover {
      transform: scale(1.1);
    }

    .yes {
      background: #ff4d6d;
      color: white;
    }

    .no {
      background: #444;
      color: white;
    }

    .hidden {
      display: none;
    }

    .emoji {
      font-size: 3rem;
      margin-top: 15px;
    }
  </style>
</head>
<body>

  <div class="box" id="question">
    <h1>Hey Love 💕</h1>
    <p>Will you be my Valentine? 🌹</p>
    <button class="yes" onclick="yesClicked()">Yes 💖</button>
    <button class="no" onclick="noClicked()">No 💔</button>
  </div>

  <div class="box hidden" id="yes">
    <h1>I knew it 😍</h1>
    <p>Lots and lots of love for you 💞💞💞</p>
    <div class="emoji">🥰💋❤️🌹💖</div>
  </div>

  <div class="box hidden" id="no">
    <h1>Wait WHAT 😭</h1>
    <p>How dare you say no 😤</p>
    <p>Now I’m crying 😭😭😭</p>
    <div class="emoji">💔😢</div>
  </div>

  <script>
    function yesClicked() {
      document.getElementById("question").classList.add("hidden");
      document.getElementById("yes").classList.remove("hidden");
    }

    function noClicked() {
      document.getElementById("question").classList.add("hidden");
      document.getElementById("no").classList.remove("hidden");
    }
  </script>

</body>
</html>
