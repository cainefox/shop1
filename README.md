
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Homepage Jualan Kue</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-image: url('blur.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
}

header {
    background-color: #e67e22;
    color: white;
    padding: 20px;
    text-align: center;
}

nav {
    background-color: #333;
}

nav ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
}

nav ul li {
    float: left;
}

nav ul li a {
    display: block;
    color : white;
    text-align: center;
    padding: 14px 20px;
    text-decoration: none;
}

nav ul li a:hover {
    background-color: #555;
}

section {
    padding: 20px;
}

section#home {
    text-align: center;
}

section#home img {
    max-width: 100%;
    height: auto;
    border-radius: 10px;
}

section#products {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
}

.product {
    background-color: white;
    padding: 10px;
    margin: 10px;
    text-align: center;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    width: 200px;
}

.product img {
    max-width: 100%;
    height: auto;
    border-radius: 10px;
}
button {
    background-color: #4CAF50;
    color: white;
    border: none;
    padding: 10px 20px;
    text-decoration: none;
    display: inline-block;
    margin-top: 10px;
    cursor: pointer;
}

button:hover {
    background-color: #45a049;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
    margin-top: 20px;

}
h2{
    color: white;
}

</style>
</head>
<body>
    <header>
        <h1>Selamat Datang di Toko Kue Kami</h1>
        <p>Kue Lezat untuk Setiap Kesempatan</p>
    </header>
        
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">Tentang Kami</a></li>
            <li><a href="produk.html">Produk</a></li>
        </ul>
    </nav>

    <section id="home">
        <img src="images/kue.jpg" alt="Kue Lezat">
        <h2>Berbagai Pilihan Kue yang Menggugah Selera</h2>
        <p>Temukan kue favorit Anda di sini!</p>
    </section>

    <section id="about">
        <h2>Tentang Kami</h2>
        <p>Kami adalah toko kue yang menyediakan berbagai jenis kue buatan rumah dengan kualitas terbaik.</p>
    </section>

    <section id="products">
        <h2>Produk Kami</h2>
        <div class="product">
            <img src="kukernutela.jpeg" alt="Kue Kering Nutella">
            <h3>Kue Kering Nutella</h3>
            <p>Rp. 50.000</p>
            <button onclick="sendToWhatsApp('Kue Kering Nutella', 'Rp50,000')">Pesan via WhatsApp</button>
        </div>
        <div class="product">
            <img src="kukermede.jpeg" alt= " kue coklat mede">
            <h3>Kue Kering Coklat Mede</h3>
            <p>Rp. 60.000</p>
            <button onclick="sendToWhatsApp('Kue Coklat Mede', 'Rp60,000')">Pesan via WhatsApp</button>
        </div>
        <div class="product">
            <img src="matcha.jpeg" alt="Kue matcha">
            <h3>Kue Matcha Almond</h3>
            <p>Rp. 60.000</p>
             <button onclick="sendToWhatsApp('Kue Matcha', 'Rp60,000')">Pesan via WhatsApp</button>
        </div>
        <div class="product">
            <img src="nastar.jpeg" alt="Kue Nastar">
            <h3>Kue Nastar</h3>
            <p>Rp. 70.000</p>
             <button onclick="sendToWhatsApp('Kue Kering Nutella', 'Rp50,000')">Pesan via WhatsApp</button>
        </div>
        <div class="product">
            <img src="Dessert.jpeg" alt="Dessert">
            <h3>Berbagai Macam Dessert Pencuci Mulut</h3>
            <p>Rp. 75.000</p>
             <button onclick="sendToWhatsApp('Dessert', 'Rp75,000')">Pesan via WhatsApp</button>
        </div>
        <!-- Tambahkan lebih banyak produk di sini -->
    </section>

</section>
    
    <footer>
        <p>&copy; 2024 Toko Kue. All rights reserved.</p>
    </footer>
    <script>
        function sendToWhatsApp(name, price) {
            var encodedMessage = encodeURIComponent("Halo, saya ingin memesan " + "Kue Kering Nutella" + " dengan harga " + "Rp50,000" + ".");
            var whatsappUrl = "https://wa.me/62895353266100" + encodedMessage; // Ganti dengan nomor WhatsApp Anda
            window.open(whatsappUrl, '_blank');
        }
    </script>
</body>
</html>
