<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>EaseMart - Welcome</title>
  <style>
    /* Reset */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background: radial-gradient(circle at center, #0a0a1f, #000);
      color: #fff;
      height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
    }

    /* Animated glowing orbs */
    .orb {
      position: absolute;
      width: 250px;
      height: 250px;
      background: rgba(150, 100, 255, 0.4);
      border-radius: 50%;
      filter: blur(100px);
      animation: float 8s infinite ease-in-out;
    }

    .orb:nth-child(1) {
      top: 10%;
      left: 15%;
      animation-delay: 0s;
    }

    .orb:nth-child(2) {
      bottom: 20%;
      right: 20%;
      background: rgba(100, 200, 255, 0.4);
      animation-delay: 3s;
    }

    .orb:nth-child(3) {
      top: 50%;
      left: 70%;
      background: rgba(255, 100, 200, 0.4);
      animation-delay: 6s;
    }

    @keyframes float {
      0%, 100% { transform: translateY(0px); }
      50% { transform: translateY(-30px); }
    }

    /* Center Content */
    .content {
      text-align: center;
      z-index: 10;
    }

    .tag {
      display: inline-block;
      background: #111;
      color: #8ef4c0;
      border: 2px solid #8ef4c0;
      padding: 5px 15px;
      border-radius: 20px;
      font-weight: bold;
      animation: pulse 2s infinite;
    }

    @keyframes pulse {
      0%, 100% { box-shadow: 0 0 10px #8ef4c0; }
      50% { box-shadow: 0 0 25px #8ef4c0; }
    }

    h1 {
      margin-top: 20px;
      font-size: 2.8rem;
      font-weight: 700;
    }

    h2 {
      margin-top: 10px;
      font-size: 1.5rem;
      color: #baffd6;
      margin-bottom: 30px;
    }

    /* Button */
    .btn {
      padding: 12px 30px;
      font-size: 1.2rem;
      color: white;
      background: linear-gradient(90deg, #00ffcc, #0077ff);
      border: none;
      border-radius: 30px;
      cursor: pointer;
      transition: 0.3s;
    }
    .btn:hover {
      transform: scale(1.1);
      box-shadow: 0 0 20px #00ffcc;
    }

    /* Decorative glowing lines */
    .line {
      position: absolute;
      width: 120%;
      height: 3px;
      background: linear-gradient(90deg, transparent, #8ef4c0, transparent);
      top: 80%;
      left: -10%;
      animation: wave 6s infinite linear;
    }

    @keyframes wave {
      0% { transform: rotate(0deg) translateY(0px); }
      50% { transform: rotate(2deg) translateY(-20px); }
      100% { transform: rotate(0deg) translateY(0px); }
    }
  </style>
</head>
<body>
  <!-- Floating glowing background orbs -->
  <div class="orb"></div>
  <div class="orb"></div>
  <div class="orb"></div>

  <!-- Main content -->
  <div class="content">
    <div class="tag">EaseMart</div>
    <h1>WELCOME TO EASEMART</h1>
    <h2>Your Cool Shopping Destination</h2>
    <button class="btn" onclick="location.href='shop.html'">Enter EaseMart</button>
  </div>

  <!-- Decorative glowing line -->
  <div class="line"></div>
</body>
</html>
