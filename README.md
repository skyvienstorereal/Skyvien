
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Skyvien Store</title>
  <style>
    /* Global Styles */
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: radial-gradient(circle, #121212, #1a1a1a);
      color: #ffffff;
      text-align: center;
    }
    .welcome {
      font-size: 2rem;
      font-weight: bold;
      margin-top: 20px;
    }
    .panel-list {
      margin: 20px auto;
      max-width: 600px;
      text-align: left;
    }
    .panel-item {
      padding: 15px;
      border: 1px solid #444;
      border-radius: 8px;
      margin: 10px 0;
      background-color: #222;
      box-shadow: 0 0 10px rgba(255, 255, 255, 0.2);
    }
    .panel-item a {
      color: #4CAF50;
      text-decoration: none;
      font-weight: bold;
    }
    .panel-item a:hover {
      color: #81c784;
    }
    .price {
      font-size: 1.2rem;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <div id="welcome" class="welcome">SELAMAT DATANG DI SKYVIEN STORE</div>
  <div class="panel-list">
    <div class="panel-item">
      <p>1GB | CPU 40%: <span class="price">1.000</span></p>
      <a href="https://wa.me/6285283253700?text=BANG+MAU+BELI+PANEL+1GB" target="_blank">Beli Sekarang</a>
    </div>
    <div class="panel-item">
      <p>2GB | CPU 50%: <span class="price">2.000</span></p>
      <a href="https://wa.me/6285283253700?text=BANG+MAU+BELI+PANEL+2GB" target="_blank">Beli Sekarang</a>
    </div>
    <div class="panel-item">
      <p>RESELLER PANEL - <span class="price">5K</span></p>
      <a href="https://wa.me/6285283253700?text=BANG+MAU+BELI+RESELLER" target="_blank">Beli Sekarang</a>
    </div>
    <div class="panel-item">
      <p>ADMIN PANEL - <span class="price">10K</span></p>
      <a href="https://wa.me/6285283253700?text=BANG+MAU+BELI+ADP+DONG" target="_blank">Beli Sekarang</a>
    </div>
    <div class="panel-item">
      <p>OWNER PANEL - <span class="price">20K</span></p>
      <a href="https://wa.me/6285283253700?text=BANG+MAU+BELI+OWNER+PANEL" target="_blank">Beli Sekarang</a>
    </div>
  </div>

  <script>
    // Change color of welcome text every 1 second
    const welcomeText = document.getElementById('welcome');
    const welcomeColors = ['#FF5733', '#33FF57', '#3357FF', '#FF33A6', '#FFFF33'];
    let welcomeIndex = 0;

    setInterval(() => {
      welcomeText.style.color = welcomeColors[welcomeIndex];
      welcomeIndex = (welcomeIndex + 1) % welcomeColors.length;
    }, 1000);

    // Change color of prices every 2 seconds
    const prices = document.querySelectorAll('.price');
    const priceColors = ['#FF5733', '#33FF57', '#3357FF', '#FF33A6', '#FFFF33'];
    let priceIndex = 0;

    setInterval(() => {
      prices.forEach(price => {
        price.style.color = priceColors[priceIndex];
      });
      priceIndex = (priceIndex + 1) % priceColors.length;
    }, 2000);
  </script>
</body>
</html>
