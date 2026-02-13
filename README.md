# Valentine
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>For My Bubu 💖</title>
  <style>
    body {
      background: linear-gradient(to right, #ff9a9e, #fad0c4);
      font-family: Arial, sans-serif;
      height: 100vh;
      margin: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
    }
    .card {
      background: white;
      padding: 25px;
      border-radius: 20px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
      max-width: 380px;
    }
    img {
      width: 100%;
      border-radius: 15px;
      margin-bottom: 15px;
    }
    h1 {
      color: #ff4d6d;
    }
    .quote {
      font-style: italic;
      color: #555;
      margin: 8px 0;
    }
    button {
      padding: 10px 25px;
      font-size: 16px;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      margin: 10px;
    }
    #yes {
      background-color: #ff4d6d;
      color: white;
    }
    #no {
      background-color: #ccc;
      position: absolute;
    }
  </style>
</head>
<body>

  <!-- Background Music -->
  <audio autoplay loop>
    <source src="mast-magan.mp3" type="audio/mpeg">
  </audio>

  <div class="card">
    <img src="bubu.jpg" alt="Us together 💕">

    <h1>Hey Bubu 💕</h1>

    <p class="quote">“With you, even silence feels beautiful.”</p>
    <p class="quote">“You are my favorite feeling.”</p>
    <p class="quote">“Every love song suddenly makes sense because of you.”</p>

    <h2>Will you be my Valentine? 💘</h2>

    <button id="yes" onclick="yesClicked()">Yes 💖</button>
    <button id="no" onmouseover="moveNo()">No 🙈</button>
  </div>

  <script>
    function yesClicked() {
      document.body.innerHTML = `
        <div style="
          text-align:center;
          background: linear-gradient(to right, #ff9a9e, #fad0c4);
          height:100vh;
          display:flex;
          flex-direction:column;
          justify-content:center;
          align-items:center;
          font-family:Arial;
          padding:20px;
        ">
          <h1 style="color:#ff4d6d;">Yayyy Bubu! 💞</h1>

          <p style="font-size:20px;">You just made my heart skip a beat 🥰</p>

          <p style="font-style:italic;">
            “If I had to choose again, I’d still choose you — every single time.”
          </p>

          <p style="margin-top:15px;">Forever yours ❤️</p>
        </div>
      `;
    }

    function moveNo() {
      const noBtn = document.getElementById("no");
      const x = Math.random() * (window.innerWidth - 120);
      const y = Math.random() * (window.innerHeight - 60);
      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    }
  </script>

</body>
</html>