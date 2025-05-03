
<html lang="id">
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
      border-radius: 15px;
      padding: 20px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.2);
      text-align: center;
      width: 300px;
      animation: fadeIn 1.5s ease;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    h1 {
      font-size: 1.6rem;
      color: #ff6f91;
      margin-bottom: 10px;
    }

    p {
      font-size: 1rem;
      margin-bottom: 10px;
      color: #555;
    }

    img {
      width: 120px;
      height: 120px;
      object-fit: cover;
      border-radius: 10px;
      margin-bottom: 15px;
      animation: floatImage 3s ease-in-out infinite;
    }

    @keyframes floatImage {
      0% { transform: translateY(0px); }
      50% { transform: translateY(-6px); }
      100% { transform: translateY(0px); }
    }

    .btn-group {
      display: flex;
      justify-content: center;
      gap: 10px;
      flex-wrap: nowrap;
      margin-top: 10px;
    }

    button {
      padding: 8px 15px;
      font-size: 0.9rem;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: 0.3s;
      white-space: nowrap;
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
      margin-top: 12px;
      font-weight: bold;
      color: #ff1d58;
      font-size: 0.95rem;
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>HAI CINTA</h1>
    <img src="april.png" alt="Foto Cinta">
    <p>Aku cuma mau bilang...</p>
    <p style="font-size: 1.3rem;"><strong>AKU MENCINTAIMU</strong></p>

    <div class="btn-group">
      <button class="yes" onclick="loveBack()">AKU JUGA CINTA KAMU</button>
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
