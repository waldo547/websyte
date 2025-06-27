<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>The New York Times – Actualizar método de pago</title>
  <link href="https://fonts.googleapis.com/css2?family=Libertine:wght@400;700&family=Helvetica:wght@400;700&display=swap" rel="stylesheet">
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body {
      font-family: 'Helvetica', sans-serif;
      background: #fafafa;
      color: #111;
      display: flex;
      flex-direction: column;
      min-height: 100vh;
    }
    header {
      padding: 20px;
      text-align: center;
      background: #fff;
      border-bottom: 1px solid #e0e0e0;
    }
    header img {
      height: 24px;
    }
    main {
      flex: 1;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 40px 20px;
    }
    .box {
      background: #fff;
      padding: 32px;
      border: 1px solid #e0e0e0;
      border-radius: 4px;
      max-width: 420px;
      width: 100%;
      text-align: center;
    }
    h1 {
      font-family: 'Libertine', serif;
      font-size: 24px;
      margin-bottom: 24px;
    }
    .current-card {
      border: 1px solid #ccc;
      border-radius: 4px;
      padding: 16px;
      text-align: left;
      margin-bottom: 24px;
      display: flex;
      align-items: center;
    }
    .current-card img {
      height: 24px;
      margin-right: 12px;
    }
    .current-card .text {
      font-size: 14px;
    }
    .btn {
      display: block;
      width: 100%;
      padding: 14px;
      margin-bottom: 16px;
      font-size: 16px;
      font-weight: bold;
      background: #fff;
      color: #111;
      border: 1px solid #111;
      border-radius: 2px;
      cursor: pointer;
      transition: background .2s, color .2s;
    }
    .btn:hover {
      background: #111;
      color: #fff;
    }
    .btn.paypal {
      display: flex;
      justify-content: center;
      align-items: center;
      background: #fff;
      border: 1px solid #ccc;
    }
    .btn.paypal img {
      height: 24px;
    }
    .secure {
      margin-top: 24px;
      font-size: 14px;
      color: #2a7b2a;
      display: flex;
      align-items: center;
      justify-content: center;
    }
    .secure img {
      height: 16px;
      margin-right: 8px;
    }
    footer {
      padding: 16px 0;
      text-align: center;
      font-size: 12px;
      color: #666;
      background: #fff;
      border-top: 1px solid #e0e0e0;
    }
    footer a {
      color: #111;
      text-decoration: underline;
      margin: 0 8px;
    }
  </style>
</head>
<body>
  <header>
    <img src="https://static01.nyt.com/images/misc/NYT_logo_rss_2x.png" alt="NYT Logo">
  </header>
  <main>
    <div class="box">
      <h1>Payment details</h1>
      <div class="current-card">
        <img src="https://upload.wikimedia.org/wikipedia/commons/0/04/Mastercard-logo.png" alt="Mastercard">
        <div class="text">Card ending in <strong>1645</strong></div>
      </div>
      <button class="btn" id="update-card">Update with Credit Card</button>
      <button class="btn paypal" id="update-paypal">
        <img src="https://www.paypalobjects.com/webstatic/icon/pp258.png" alt="PayPal">
      </button>
      <div class="secure">
        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e7/Padlock_icon.svg/512px-Padlock_icon.svg.png" alt="Secure">
        <span>Secure Transaction</span>
      </div>
    </div>
  </main>
  <footer>
    Need help? <a href="#">Contact Customer Care</a><br>
    © 2025 The New York Times Company<br>
    <a href="#">Privacy Policy</a> |
    <a href="#">California Notice</a>
  </footer>

  <script>
    document.getElementById('update-card').addEventListener('click', () => {
      alert('Aquí iría el flujo para actualizar con tarjeta de crédito.');
    });
    document.getElementById('update-paypal').addEventListener('click', () => {
      alert('Aquí iría el flujo para actualizar con PayPal.');
    });
  </script>
</body>
</html>
