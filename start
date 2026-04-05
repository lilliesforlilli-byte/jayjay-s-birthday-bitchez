<!DOCTYPE html>
<html>
<head>
  <title>Mission: Soup 🎮</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to bottom, #020024, #090979, #000);
      color: #fff;
      text-align: center;
      overflow-x: hidden;
    }

    h1 {
      margin-top: 60px;
      font-size: 36px;
    }

    .btn {
      margin-top: 30px;
      padding: 14px 30px;
      font-size: 18px;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      background: #00c3ff;
      color: #000;
      box-shadow: 0 0 15px #00c3ff;
      transition: 0.3s;
    }

    .btn:hover {
      transform: scale(1.1);
      box-shadow: 0 0 25px #00c3ff;
    }

    .hidden {
      display: none;
    }

    .companions {
      display: flex;
      justify-content: center;
      gap: 25px;
      margin-top: 40px;
      flex-wrap: wrap;
    }

    .comp-btn {
      background: rgba(255,255,255,0.05);
      border-radius: 20px;
      padding: 15px;
      width: 150px;
      cursor: pointer;
      transition: 0.3s;
      backdrop-filter: blur(6px);
    }

    .comp-btn img {
      width: 100%;
      border-radius: 12px;
    }

    /* UNIQUE GLOWS */
    .snow:hover {
      box-shadow: 0 0 20px #4cc9f0;
      transform: translateY(-6px);
    }

    .death:hover {
      box-shadow: 0 0 20px #ff006e;
      transform: translateY(-6px);
    }

    .dread:hover {
      box-shadow: 0 0 20px #ffd60a;
      transform: translateY(-6px);
    }

    .letter {
      max-width: 600px;
      margin: 50px auto;
      background: rgba(255,255,255,0.08);
      padding: 30px;
      border-radius: 15px;
      backdrop-filter: blur(10px);
      display: none;
      text-align: left;
      line-height: 1.7;
    }

    .music {
      margin-top: 30px;
    }

    audio {
      width: 80%;
      margin-top: 10px;
    }

    /* SNOW EFFECT */
    .snow-bg {
      position: fixed;
      width: 100%;
      height: 100%;
      pointer-events: none;
      background-image:
        radial-gradient(2px 2px at 20px 30px, white, transparent),
        radial-gradient(2px 2px at 40px 70px, white, transparent),
        radial-gradient(1.5px 1.5px at 90px 40px, white, transparent);
      background-size: 200px 200px;
      animation: snow 12s linear infinite;
      opacity: 0.5;
    }

    @keyframes snow {
      0% { background-position: 0 -200px; }
      100% { background-position: 0 100vh; }
    }
  </style>
</head>

<body>

<div class="snow-bg"></div>

<h1>🎮 Mission: Soup's Birthday</h1>

<button class="btn" onclick="startMission()">Start Mission</button>

<div id="companions" class="companions hidden">

  <!-- SNOW MIRAGE -->
  <div class="comp-btn snow" onclick="chooseCompanion('snow')">
    <img src="snowmirage.jpg">
    <p>Snow Mirage ❄️</p>
  </div>

  <!-- DEATH KNELL -->
  <div class="comp-btn death" onclick="chooseCompanion('deathknell')">
    <img src="deathknell.png">
    <p>Death Knell ☠️</p>
  </div>

  <!-- DREADWOLF -->
  <div class="comp-btn dread" onclick="chooseCompanion('dreadwolf')">
    <img src="dreadwolf.jpg">
    <p>Dreadwolf ⚡</p>
  </div>

</div>

<div id="letter" class="letter"></div>

<div id="music" class="music hidden">
  <h3>🎧 Mission Soundtrack</h3>

  <!-- REPLACE WITH YOUR FILES -->
  <button class="btn" onclick="playMusic('song1.mp3')">Track 1</button>
  <button class="btn" onclick="playMusic('song2.mp3')">Track 2</button>
  <button class="btn" onclick="playMusic('song3.mp3')">Track 3</button>

  <br>
  <audio id="player" controls></audio>
</div>

<script>
  function startMission() {
    document.getElementById("companions").classList.remove("hidden");
  }

  function chooseCompanion(choice) {
    const letter = document.getElementById("letter");

    if (choice === "snow") {
      letter.innerHTML = `
        <p><strong>Mission Log: Snow Mirage ❄️</strong></p>
        <p>You chose the calmest and strongest one… just like you.</p>
        <p>You’ve always been someone who stays, who protects, who cares quietly but deeply.</p>
        <p>That kind of strength? Not everyone has it.</p>
        <p>Happy Birthday, weirdo 💙</p>
      `;
    }

    if (choice === "deathknell") {
      letter.innerHTML = `
        <p><strong>Mission Log: Death Knell ☠️</strong></p>
        <p>Bold choice. Chaotic energy. Very you.</p>
        <p>You bring chaos in the best way—laughter, energy, and life into everything.</p>
        <p>But behind that? You're one of the most genuine people I know.</p>
      `;
    }

    if (choice === "dreadwolf") {
      letter.innerHTML = `
        <p><strong>Mission Log: Dreadwolf ⚡</strong></p>
        <p>Fast, sharp, unstoppable.</p>
        <p>You don’t hesitate—you move, you act, you protect.</p>
        <p>There’s something powerful about the way you face things head-on.</p>
        <p>I admire that more than you know.</p>
      `;
    }

    letter.style.display = "block";
    document.getElementById("music").classList.remove("hidden");
  }

  function playMusic(file) {
    const player = document.getElementById("player");
    player.src = file;
    player.play();
  }
</script>

</body>
</html>
