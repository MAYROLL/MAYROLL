<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>MAYROLL | Premium Food Brand</title>
  <meta name="description" content="MAYROLL - Premium Food Brand dengan risol renyah dan isian lembut yang bikin nagih. ONE BITE - FULL DELIGHT.">
  <link rel="icon" type="image/png" href="LOGO ROLL.png">
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600&display=swap" rel="stylesheet">

  <style>
    body {
      margin: 0;
      font-family: 'Montserrat', sans-serif;
      background-color: #yellow;
      color: #D4AF37;
    }

    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 40px;
      border-bottom: 1px solid #D4AF37;
    }

    .logo-box {
      display: flex;
      align-items: center;
      gap: 20px;
    }

    .logo-box img {
      height: 220px;
      border-radius: 8px;
    }

    header h1 {
      font-weight: 600;
      letter-spacing: 3px;
      color: #D4AF37;
      margin: 0;
    }

    nav a {
      color: #D4AF37;
      margin: 0 15px;
      text-decoration: none;
      font-weight: 600;
    }

    nav a:hover {
      color: white;
    }

    .cart-icon {
      cursor: pointer;
      position: relative;
      font-size: 1.4em;
    }

    .cart-count {
      position: absolute;
      top: -8px;
      right: -10px;
      background: red;
      color: white;
      font-size: 0.7em;
      padding: 2px 5px;
      border-radius: 50%;
    }

    section {
      padding: 60px 20px;
      text-align: center;
    }

    .produk-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 25px;
      margin-top: 40px;
      padding: 0 40px;
    }

    .produk {
      background: #111;
      border: 1px solid #D4AF37;
      border-radius: 8px;
      padding-bottom: 15px;
      transition: all 0.3s ease;
    }

    .produk:hover {
      transform: scale(1.05);
      box-shadow: 0 0 15px rgba(212,175,55,0.4);
    }

    .produk img {
      width: 100%;
      height: 150px;
      object-fit: cover;
      border-bottom: 1px solid #D4AF37;
      border-top-left-radius: 8px;
      border-top-right-radius: 8px;
    }

    .produk h3 { margin: 10px 0 5px 0; }
    .produk p { margin: 5px 0; color: #ccc; font-size: 0.9em; }

    .jumlah-box {
      display: flex;
      justify-content: center;
      align-items: center;
      margin: 8px 0;
    }

    .jumlah-input {
      width: 50px;
      text-align: center;
      background: #000;
      color: #D4AF37;
      border: 1px solid #D4AF37;
      border-radius: 6px;
      padding: 4px;
      margin: 0 5px;
    }

    .minus, .plus {
      background: #D4AF37;
      color: #000;
      border: none;
      border-radius: 6px;
      font-size: 18px;
      font-weight: bold;
      width: 28px;
      height: 28px;
      cursor: pointer;
      transition: 0.2s;
    }

    .minus:hover, .plus:hover {
      background: #f5e1a4;
      transform: scale(1.1);
    }

    .produk button {
      background-color: #D4AF37;
      color: #000;
      border: none;
      padding: 8px 16px;
      cursor: pointer;
      border-radius: 4px;
      font-weight: bold;
    }

    .produk button:hover {
      background-color: #b8860b;
    }

    .cart-popup {
      position: fixed;
      top: 70px;
      right: 30px;
      width: 320px;
      background: #111;
      border: 1px solid red;
      border-radius: 8px;
      padding: 20px;
      display: none;
      z-index: 100;
    }

    .cart-popup h3 { margin-top: 0; }
    .cart-item {
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-bottom: 1px solid #333;
      padding: 8px 0;
    }

    .cart-item span { color: #ddd; font-size: 0.9em; }
    .cart-item button { background: none; border: none; color: red; font-size: 1em; cursor: pointer; }

    .cart-popup button.checkout,
    .cart-popup button.clear {
      background-color: #D4AF37;
      color: #000;
      width: 100%;
      padding: 10px;
      margin-top: 10px;
      font-weight: bold;
      border: none;
      border-radius: 5px;
    }

    .cart-popup button.checkout:hover,
    .cart-popup button.clear:hover {
      background-color: #b8860b;
    }

    #admin-btn {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background-color: #D4AF37;
      color: #000;
      border: none;
      padding: 10px 15px;
      border-radius: 50px;
      cursor: pointer;
      font-weight: bold;
      z-index: 101;
    }

    #admin-popup, #login-popup {
      position: fixed;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      background: #111;
      border: 1px solid #D4AF37;
      border-radius: 8px;
      padding: 20px;
      display: none;
      z-index: 102;
      width: 300px;
    }

    #admin-popup input, #login-popup input, #admin-popup select {
      width: 100%;
      padding: 6px;
      margin: 5px 0;
      border-radius: 4px;
      border: none;
    }

    #admin-popup button, #login-popup button {
      background-color: #D4AF37;
      color: #000;
      border: none;
      padding: 8px 12px;
      cursor: pointer;
      font-weight: bold;
      border-radius: 4px;
      margin-top: 5px;
    }

    #admin-popup button:hover, #login-popup button:hover {
      background-color: #b8860b;
    }
#notif { position: fixed; top: 20px; right: 20px; background: rgba(212,175,55,0.95); 
color: #000; padding: 12px 20px; border-radius: 8px; 
font-weight: 600; box-shadow: 0 4px 15px rgba(0,0,0,0.3); 
opacity: 0; transform: translateY(-20px); 
transition: all 0.4s ease; z-index: 999; } 

#notif.show { opacity: 1; transform: translateY(0); }
 
 #notif.red {
  background: rgba(255, 60, 60, 0.95);
  color: #fff;
  border: 2px solid #ff0000;
}

#notif.green {
  background: rgba(40, 180, 99, 0.95);
  color: #fff;
  border: 2px solid #00cc66;
}

#notif.orange {
  background: rgba(255, 165, 0, 0.95);
  color: #000;
  border: 2px solid #ffae00;
}



    footer {
      text-align: center;
      border-top: 1px solid #D4AF37;
      padding: 20px;
      font-size: 0.9em;
    }

    footer a {
      color: #D4AF37;
      text-decoration: none;
    }

    footer a:hover {
      color: #fff;
    }
  </style>
</head>
<body>

<header>
  <div class="logo-box">
    <img src="LOGO ROLL.png" alt="Logo MAYROLL">
    <h1>MAYROLL</h1>
  </div>

  <nav>
    <a href="#home">Home</a>
    <a href="#produk">Produk</a>
    <a href="#tentang">Tentang</a>
    <a href="#kontak">Kontak</a>
  </nav>

  <div class="cart-icon" onclick="toggleCart()"><img src="keranjang.png" alt="Logo keranjang" style="width:50px; vertical-align:middle; margin-right:20px;"><span class="cart-count" id="cart-count">0</span></div>
</header>

<section id="home">
  <h2>WELCOME TO MAYROLL</h2><br><h3>ONE BITE - FULL DELIGHT</h3>
  <p>Di setiap gigitan MAYROLL, kami percaya bahwa kebahagiaan bisa dimulai dari sesuatu yang sederhana - satu risol dengan rasa yang bikin nagih.
  Dibuat dari bahan terbaik, kulit renyah, dan isian lembut yang kaya rasa, setiap varian menghadirkan sensasi berbeda di setiap gigitannya.
  Kami bukan sekadar menjual risol - kami menghadirkan momen penuh kelezatan.
  <strong>ONE BITE - FULL DELIGHT.</strong> Karena dari satu gigitan, kamu bisa jatuh cinta.</p>
</section>

<section id="produk">
  <h2>Produk Kami</h2>
  <div class="produk-container" id="produk-container"></div>
</section>

<div class="cart-popup" id="cart-popup">
  <h3>Keranjang</h3>
  <div id="cart-items"></div>
  <p id="cart-total">Total: Rp0</p>
  <button class="checkout" onclick="checkout()">Checkout (WhatsApp)</button>
  <button class="checkout" onclick="checkoutEmail()">Checkout (Email)</button>
  <button class="clear" onclick="clearCart()">Kosongkan Keranjang</button>
</div>

<button id="admin-btn" onclick="showLogin()">Admin</button>

<div id="login-popup">
  <h3>Login Admin</h3>
  <input type="password" id="admin-password" placeholder="Masukkan password">
  <button onclick="checkPassword()">Login</button>
</div>

<div id="admin-popup">
  <h3>Admin Panel</h3>
  <select id="admin-produk-select"></select>
  <input type="number" id="admin-harga" placeholder="Harga">
  <input type="number" id="admin-stok" placeholder="Stok">
  <button onclick="updateProduk()">Update Produk</button>
  <button onclick="closeAdmin()">Tutup</button>
</div>

<section id="tentang">
  <h2>Tentang MAYROLL</h2><br><h3>
  <p>MAYROLL lahir dari keinginan sederhana: bikin risol yang bukan cuma enak, tapi punya vibe dan rasa yang ngangenin.
Setiap varian kami dibuat dengan bahan terbaik, kulit yang renyah, dan isian yang penuh karakter - dari mayonais creamy, ayam pedas daun jeruk, sampai bolognese gurih yang bikin jatuh cinta di gigitan pertama.
Buat kami, makanan bukan cuma soal kenyang, tapi soal mood.
ONE BITE - FULL DELIGHT. Karena dari satu gigitan aja, kamu udah bisa ngerasain kebahagiaan versi MAYROLL.</p>
</section>

<section id="kontak">
  <h2>Kontak Kami</h2>
  <p><img src="email.png" alt="Logo email" style="width:20px; vertical-align:middle; margin-right:5px;"><a href="https://mail.google.com/mail/?view=cm&to=mayrollofficial2025@gmail.com">mayrollofficial2025@gmail.com</a>
  <p><img src="instagram.png" alt="Logo Instagram" style="width:20px; vertical-align:middle; margin-right:5px;">
  <a href="https://www.instagram.com/mayroll_official?igsh=MTl1YXJoMnBlbm43cg==" target="_blank">Instagram</a> |<img src="tiktok.png" alt="Logo Instagram" style="width:20px; vertical-align:middle; margin-right:5px;">  
  <a href="https://vm.tiktok.com/ZSHc6nAVaNCer-BUdVe/" target="_blank">TikTok</a></p>
</section>

<footer>
  <p>© 2025 MAYROLL. All Rights Reserved.</p>
</footer>

<div id="notif"></div>

<script>
localStorage.removeItem("produkData"); // reset otomatis

let produkData = JSON.parse(localStorage.getItem("produkData")) || [
  { id:1, nama:"RISOLL ROGOUT", harga:3000, stok:10, gambar:"rogout.png" },
  { id:2, nama:"RISOLL HATI&AMPELA AYAM", harga:3000, stok:5, gambar:"hati&ampela.png" },
  { id:3, nama:"RISOLL AYAM PEDAS", harga:3000, stok:100, gambar:"ayampedas.png" },
  { id:4, nama:"RISOLL MAYO", harga:3000, stok:12, gambar:"mayo.png" },
  { id:5, nama:"Risol Bolognese", harga:3000, stok:3, gambar:"bolognase.png" },
];
const container = document.getElementById('produk-container');
const cartPopup = document.getElementById('cart-popup');
const cartCount = document.getElementById('cart-count');
const cartItemsContainer = document.getElementById('cart-items');
const cartTotal = document.getElementById('cart-total');
const notif = document.getElementById('notif');
let cart = [];

function saveProduk() {
  localStorage.setItem("produkData", JSON.stringify(produkData));
}

function showNotif(text, color="#000") {
  notif.textContent = text;
  notif.style.color = color;
  notif.classList.add('show');
  setTimeout(() => notif.classList.remove('show'), 2500);
}

function renderProduk() {
  container.innerHTML = '';
  produkData.forEach(p => {
    const div = document.createElement('div');
    div.className = 'produk';
    div.innerHTML = `
      <img src="${p.gambar}" alt="${p.nama}">
      <h3>${p.nama}</h3>
      <p>Harga: Rp${p.harga.toLocaleString()}</p>
      <p>Stok: ${p.stok}</p>
      <div class="jumlah-box">
        <button class="minus" onclick="ubahJumlah(${p.id}, -1)">-</button>
        <input type="number" id="jumlah-${p.id}" value="1" min="1" max="${p.stok}" class="jumlah-input">
        <button class="plus" onclick="ubahJumlah(${p.id}, 1)">+</button>
      </div>
      <button id="btn-${p.id}" onclick="addToCart(${p.id})" ${p.stok <= 0 ? 'disabled style="background:#777;cursor:not-allowed;"' : ''}>${p.stok > 0 ? 'Tambah ke Keranjang' : 'Stok Habis'}</button>
    `;
    container.appendChild(div);
  });
}

function ubahJumlah(id, perubahan) {
  const input = document.getElementById(`jumlah-${id}`);
  let nilai = parseInt(input.value) || 1;
  nilai += perubahan;
  if (nilai < 1) nilai = 1;
  const produk = produkData.find(p => p.id === id);
  if (nilai > produk.stok) nilai = produk.stok;
  input.value = nilai;
}

function addToCart(id) {
  const produk = produkData.find(p => p.id === id);
  const jumlahInput = document.getElementById(`jumlah-${id}`);
  const jumlah = parseInt(jumlahInput.value) || 0;
  if (jumlah <= 0) return showNotif("Masukkan jumlah!", "red");
  if (jumlah > produk.stok) return showNotif("Stok tidak cukup!", "red");

  const item = cart.find(c => c.id === id);
  if (item) {
    if (item.jumlah + jumlah > produk.stok) return showNotif("Stok tidak cukup!", "red");
    item.jumlah += jumlah;
  } else {
    cart.push({ id, jumlah });
  }

  showNotif(`${jumlah}x ${produk.nama} ditambahkan`, "green");
  updateCart();
}

function toggleCart() {
  cartPopup.style.display = cartPopup.style.display === 'block' ? 'none' : 'block';
}

function updateCart() {
  cartCount.textContent = cart.reduce((a,c)=>a+c.jumlah,0);
  cartItemsContainer.innerHTML = '';
  let total = 0;
  cart.forEach(c=>{
    const p = produkData.find(p=>p.id===c.id);
    total += c.jumlah * p.harga;
    const div = document.createElement('div');
    div.className='cart-item';
    div.innerHTML = `<span>${p.nama} x${c.jumlah}</span><span>Rp${(p.harga*c.jumlah).toLocaleString()}</span><button onclick="removeCart(${c.id})">?</button>`;
    cartItemsContainer.appendChild(div);
  });
  cartTotal.textContent = `Total: Rp${total.toLocaleString()}`;
}

function removeCart(id) {
  cart = cart.filter(c=>c.id!==id);
  updateCart();
  showNotif("Item dihapus dari keranjang", "red");
}

function clearCart() {
  if (cart.length === 0) return showNotif("Keranjang sudah kosong!", "red");
  cart = [];
  updateCart();
  showNotif("Keranjang dikosongkan");
}

function checkout() {
  if (cart.length === 0) return alert("Keranjang kosong!");

  // Kurangi stok produk sesuai isi keranjang
  cart.forEach(c => {
    const p = produkData.find(p => p.id === c.id);
    if (p) p.stok -= c.jumlah;
  });
  saveProduk(); // simpan stok baru
  renderProduk(); // tampilkan ulang stok baru

  // Buat pesan untuk WhatsApp
  let message = "Halo, saya ingin memesan:\n\n";
  cart.forEach(c => {
    const p = produkData.find(p => p.id === c.id);
    message += `- ${p.nama} x${c.jumlah}\n`;
  });
  const total = cart.reduce((a,c)=>a + produkData.find(p=>p.id===c.id).harga*c.jumlah,0);
  message += `\nTotal: Rp${total.toLocaleString()}\n\nTerima kasih `;

  const encodedMessage = encodeURIComponent(message);
  window.open(`https://wa.me/62881022526255?text=${encodedMessage}`);

  cart = [];
  updateCart();
  showNotif("Checkout berhasil! ", "green");
}

function checkoutEmail() {
  if(cart.length===0) return showNotif("Keranjang kosong!", "red");
  let body = "Halo, saya ingin memesan:%0A";
  cart.forEach(c=>{
    const p = produkData.find(p=>p.id===c.id);
    body += `- ${p.nama} x${c.jumlah}%0A`;
  });
  const total = cart.reduce((a,c)=>a + produkData.find(p=>p.id===c.id).harga*c.jumlah,0);
  body += `Total: Rp${total.toLocaleString()}`;
  window.location.href = `mailto:mayroll.brand@gmail.com?subject=Pesanan MAYROLL&body=${body}`;
  showNotif("Checkout via Email dibuka", "green");
}

function showLogin() {
  document.getElementById('login-popup').style.display='block';
}

function checkPassword() {
  const pass = document.getElementById('admin-password').value;
  if(pass === "gendis2007") {
    document.getElementById('login-popup').style.display='none';
    document.getElementById('admin-popup').style.display='block';
    const select = document.getElementById('admin-produk-select');
    select.innerHTML = '';
    produkData.forEach(p=>{
      const option = document.createElement('option');
      option.value = p.id;
      option.textContent = p.nama;
      select.appendChild(option);
    });
  } else showNotif("Password salah!", "red");
}

function updateProduk() {
  const id = parseInt(document.getElementById('admin-produk-select').value);
  const harga = parseInt(document.getElementById('admin-harga').value);
  const stok = parseInt(document.getElementById('admin-stok').value);
  const p = produkData.find(p=>p.id===id);
  if(!p) return;
  if(harga>0) p.harga=harga;
  if(stok>=0) p.stok=stok;
  saveProduk();
  renderProduk();
  showNotif("Produk diperbarui!", "green");
}

function closeAdmin() {
  document.getElementById('admin-popup').style.display='none';
}

renderProduk();
</script>


</body>
</html>
