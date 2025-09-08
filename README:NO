<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Secret Crush 💖</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: pink;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      overflow: hidden;
    }
    .container {
      background: #fff;
      padding: 25px;
      border-radius: 20px;
      box-shadow: 0px 5px 15px rgba(0,0,0,0.2);
      text-align: center;
      max-width: 400px;
      width: 100%;
      position: relative;
      z-index: 10;
    }
    h2 {
      color: #ff4d6d;
    }
    input, select, button {
      width: 90%;
      padding: 10px;
      margin: 10px 0;
      border-radius: 10px;
      border: 1px solid #ccc;
      font-size: 14px;
    }
    button {
      background-color: #ff4d6d;
      color: white;
      border: none;
      cursor: pointer;
      font-size: 16px;
    }
    button:hover {
      background-color: #e6004c;
    }
    .hidden {
      display: none;
    }
    .whatsapp-btn {
      background-color: #25D366;
      color: white;
      text-decoration: none;
      padding: 12px 20px;
      border-radius: 10px;
      display: inline-block;
      margin-top: 15px;
      font-size: 16px;
      position: relative;
      z-index: 20;
    }
    .whatsapp-btn:hover {
      background-color: #1ebd5f;
    }

    /* Floating hearts */
    .heart {
      position: fixed;
      top: -10px;
      color: red;
      font-size: 24px;
      animation: fall linear forwards;
    }
    @keyframes fall {
      to {
        transform: translateY(110vh);
        opacity: 0;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <h2>💖 Secret Crush 💖</h2>
    <form id="friendForm">
      <input type="text" id="name" placeholder="Your Name" required>
      <input type="text" id="nickname" placeholder="Your Nickname">
      <input type="date" id="birthday" placeholder="Your Birthday">
      
      <label for="love">Do you believe in love at first sight?</label>
      <select id="love" required>
        <option value="">--Choose--</option>
        <option value="Yes">Yes 💖</option>
        <option value="No">No 😅</option>
      </select>

      <button type="submit">Submit</button>
    </form>
    <div id="thankYou" class="hidden">
      <h3 id="message"></h3>
      <a href="https://wa.me/919587254424" target="_blank" class="whatsapp-btn">Message Me on WhatsApp</a>
    </div>
  </div>

  <script>
    const form = document.getElementById("friendForm");
    const thankYou = document.getElementById("thankYou");
    const message = document.getElementById("message");

    form.addEventListener("submit", function(event) {
      event.preventDefault();
      const name = document.getElementById("name").value;
      const nickname = document.getElementById("nickname").value;
      const birthday = document.getElementById("birthday").value;
      const love = document.getElementById("love").value;

      message.innerHTML = `🎉 Thank you ${name} (${nickname}) 💖<br>
        Your Birth Date: ${birthday} 🎂<br>
        Love at first sight: ${love}`;
      
      form.classList.add("hidden");
      thankYou.classList.remove("hidden");

      // Floating hearts start
      setInterval(createHeart, 500);
    });

    function createHeart() {
      const heart = document.createElement("div");
      heart.classList.add("heart");
      heart.innerHTML = "💖";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.animationDuration = (2 + Math.random() * 3) + "s";
      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 5000);
    }
  </script>
</body>
</html>
