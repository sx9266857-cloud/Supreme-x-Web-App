# Supreme-x-Web-App
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>SUPREME X Web App</title>
  <link rel="icon" href="favicon.ico" />
  <meta name="description" content="Welcome to SUPREME X – your gateway to the ultimate experience." />
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to bottom, #0d0d0d, #1a1a1a);
      color: #ffffff;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
      text-align: center;
      position: relative;
      overflow: hidden;
    }

    .flame-overlay {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: url('flame.gif') center center / cover no-repeat;
      opacity: 0.15;
      pointer-events: none;
      animation: flicker 3s infinite ease-in-out;
      z-index: 0;
    }

    @keyframes flicker {
      0% { opacity: 0.1; }
      50% { opacity: 0.2; }
      100% { opacity: 0.1; }
    }

    .logo {
      width: 200px;
      height: auto;
      margin-bottom: 1rem;
      box-shadow: 0 0 25px rgba(255, 69, 0, 0.6);
      border-radius: 8px;
      z-index: 1;
    }

    .loader {
      border: 6px solid #333;
      border-top: 6px solid #ff4500;
      border-radius: 50%;
      width: 50px;
      height: 50px;
      animation: spin 1s linear infinite;
      margin: 1.5rem 0;
      z-index: 1;
    }

    @keyframes spin {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }

    .message {
      font-size: 1.1rem;
      color: #cccccc;
      margin-bottom: 1rem;
      z-index: 1;
    }

    .enter-button {
      background-color: #ff4500;
      color: #fff;
      padding: 12px 24px;
      border-radius: 6px;
      text-decoration: none;
      font-weight: bold;
      font-size: 1rem;
      transition: box-shadow 0.3s ease, transform 0.2s ease;
      z-index: 1;
    }

    .enter-button:hover {
      box-shadow: 0 0 15px #ffae42;
      transform: scale(1.05);
    }

    audio {
      display: none;
    }
  </style>
</head>
<body>
  <!-- 🔥 Flame Background -->
  <div class="flame-overlay"></div>

  <!-- 🔊 Sound Effect -->
  <audio autoplay>
    <source src="flame-sound.mp3" type="audio/mpeg" />
  </audio>

  <!-- 🔥 Logo -->
  <img src="supreme-x-logo.jpeg" alt="SUPREME X Logo" class="logo" />

  <!-- 🔄 Loader -->
  <div class="loader"></div>

  <!-- ⏳ Message & Button -->
  <p class="message">Welcome to SUPREME X.<br>Click below to enter the experience.</p>
  <a href="https://tinyurl.com/SXCAPP" class="enter-button">Enter Now</a>
</body>
</html>
