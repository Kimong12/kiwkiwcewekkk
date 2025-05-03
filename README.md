
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Surat Cinta</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(135deg, #ffd6e8, #ffeef9);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      overflow: hidden;
    }

    .card {
      background: white;
      border-radius: 20px;
      padding: 30px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
      text-align: center;
      max-width: 500px;
      animation: fadeIn 2s ease;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    h1 {
      font-size: 2rem;
      color: #ff6f91;
    }

    p {
      font-size: 1.1rem;
      margin-bottom: 20px;
      color: #555;
    }

    img {
      max-width: 100%;
      border-radius: 15px;
      margin-bottom: 20px;
      animation: floatImage 4s ease-in-out infinite;
    }

    @keyframes floatImage {
      0% { transform: translateY(0px); }
      50% { transform: translateY(-10px); }
      100% { transform: translateY(0px); }
    }

    .btn-group {
      display: flex;
      justify-content: center;
      gap: 15px;
    }

    button {
      padding: 10px 20px;
      font-size: 1rem;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: 0.3s;
    }

    .yes {
      background-color: #6ee7b7;
      color: #065f46;
    }

    .yes:hover {
      background-color: #34d399;
    }

    .no {
      background-color: #fca5a5;
      color: #7f1d1d;
    }

    .no:hover {
      background-color: #f87171;
    }

    .message {
      margin-top: 20px;
      font-weight: bold;
      color: #ff1d58;
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>HAI CINTA</h1>
    <img src="april.png"/>
    <p> Aku cuma mau bilang...</p>
    <p style="font-size: 1.5rem;"><strong>I LOVE YOU </strong></p>

    <div class="btn-group">
      <button class="yes" onclick="loveBack()">I LOVE YOU TOO MG IMAN</button>
      <button class="no" onclick="noLove()">GA DULU WLEE</button>
    </div>

    <div class="message" id="message"></div>
  </div>

  <script>
    function loveBack() {
      document.getElementById("message").innerHTML = "Aku juga sayang kamu banget april bot!";
    }

    function noLove() {
      const msg = document.getElementById("message");
      msg.innerHTML = "Eits... tombol ini gak bisa, coba yang satunya yaa~";
    }
  </script>
</body>
</html>
