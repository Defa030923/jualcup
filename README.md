<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Betta Store | Jual Ikan Cupang Premium</title>
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; font-family: 'Segoe UI', sans-serif; }
    body { background: #f4f6f8; color: #333; }
    header {
      background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
      color: white;
      padding: 30px;
      text-align: center;
    }
    header h1 { font-size: 2.5rem; }
    nav {
      background: #1b1b1b;
      padding: 10px;
      display: flex;
      justify-content: center;
      gap: 20px;
    }
    nav a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }
    nav a:hover { color: #00e5ff; }
    .container { padding: 30px; max-width: 1200px; margin: auto; }
    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .card {
      background: white;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      overflow: hidden;
      transition: transform 0.3s;
    }
    .card:hover { transform: scale(1.03); }
    .card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }
    .card-body { padding: 15px; }
    .card-body h3 { margin-bottom: 8px; }
    .price { color: #e53935; font-weight: bold; margin-bottom: 10px; }
    button {
      background: #0d47a1;
      color: white;
      border: none;
      padding: 10px 15px;
      border-radius: 8px;
      cursor: pointer;
      width: 100%;
    }
    button:hover { background: #1565c0; }
    footer {
      background: #1b1b1b;
      color: white;
      text-align: center;
      padding: 15px;
      margin-top: 40px;
    }
    .cart {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #ff9800;
      color: white;
      padding: 15px;
      border-radius: 50px;
      font-weight: bold;
    }
  </style>
</head>
<body>

<header>
  <h1>🐟 Betta Store</h1>
  <p>Jual Ikan Cupang Premium • Sehat • Siap Kirim</p>
</header>

<nav>
  <a href="#">Beranda</a>
  <a href="#produk">Produk</a>
  <a href="#kontak">Kontak</a>
</nav>

<div class="container" id="produk">
  <h2 style="margin-bottom:20px">Daftar Ikan Cupang</h2>
  <div class="products">
    <div class="card">
      <img src="https://images.unsplash.com/photo-1604848698030-c434ba08ece1" alt="Cupang Halfmoon">
      <div class="card-body">
        <h3>Cupang Halfmoon</h3>
        <p class="price">Rp 150.000</p>
        <button onclick="addToCart('Halfmoon')">Tambah ke Keranjang</button>
      </div>
    </div>

    <div class="card">
      <img src="https://images.unsplash.com/photo-1629217851682-7d4b4c7d42e5" alt="Cupang Plakat">
      <div class="card-body">
        <h3>Cupang Plakat</h3>
        <p class="price">Rp 120.000</p>
        <button onclick="addToCart('Plakat')">Tambah ke Keranjang</button>
      </div>
    </div>

    <div class="card">
      <img src="https://images.unsplash.com/photo-1611599538436-b953b76c0a32" alt="Cupang Koi">
      <div class="card-body">
        <h3>Cupang Koi</h3>
        <p class="price">Rp 200.000</p>
        <button onclick="addToCart('Koi')">Tambah ke Keranjang</button>
      </div>
    </div>
  </div>
</div>

<div class="container" id="kontak">
  <h2>Kontak Kami</h2>
  <p>📱 WhatsApp: 08xxxxxxxxxx</p>
  <p>📦 Pengiriman: Seluruh Indonesia</p>
  <p>📸 Instagram / TikTok: @bettastore</p>
</div>

<div class="cart" id="cart">🛒 Keranjang: 0</div>

<footer>
  <p>© 2026 Betta Store | Website Jual Ikan Cupang</p>
</footer>

<script>
  let cartCount = 0;
  function addToCart(nama) {
    cartCount++;
    document.getElementById('cart').innerText = '🛒 Keranjang: ' + cartCount;
    alert('Ikan Cupang ' + nama + ' ditambahkan ke keranjang');
  }
</script>

</body>
</html>

