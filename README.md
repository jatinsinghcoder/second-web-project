<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>shopio</title>
</head>
<body>
   <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>SHOPIO - Electronics Store</title>
  <style>
    /* Reset */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      background: #f9f9f9;
      color: #333;
    }

    /* Header */
    header {
      background: #111;
      color: #fff;
      padding: 20px 50px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    header h1 {
      font-size: 26px;
      font-weight: bold;
      letter-spacing: 2px;
    }

    nav ul {
      list-style: none;
      display: flex;
      gap: 20px;
    }

    nav ul li {
      display: inline;
    }

    nav ul li a {
      text-decoration: none;
      color: #fff;
      font-weight: bold;
      transition: 0.3s;
    }

    nav ul li a:hover {
      color: #ff9800;
    }

    /* Hero Section */
    .hero {
      background: url('https://images.unsplash.com/photo-1511707171634-5f897ff02aa9') no-repeat center center/cover;
      height: 70vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: white;
      position: relative;
    }

    .hero::after {
      content: "";
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background: rgba(0,0,0,0.5);
    }

    .hero h2 {
      font-size: 48px;
      position: relative;
      z-index: 2;
      margin-bottom: 20px;
    }

    .hero button {
      position: relative;
      z-index: 2;
      padding: 12px 25px;
      border: none;
      background: #ff9800;
      color: white;
      font-size: 18px;
      font-weight: bold;
      border-radius: 5px;
      cursor: pointer;
      transition: 0.3s;
    }

    .hero button:hover {
      background: #e68900;
    }

    /* Products */
    .products {
      padding: 50px;
      text-align: center;
    }

    .products h2 {
      margin-bottom: 20px;
      font-size: 32px;
    }

    .product-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .product {
      background: #fff;
      border-radius: 10px;
      padding: 20px;
      box-shadow: 0px 2px 8px rgba(0,0,0,0.1);
      transition: 0.3s;
    }

    .product:hover {
      transform: translateY(-5px);
    }

    .product img {
      width: 100%;
      border-radius: 10px;
    }

    .product h3 {
      margin: 15px 0;
    }

    .product p {
      color: #666;
      font-size: 14px;
    }

    .product button {
      margin-top: 10px;
      padding: 10px 15px;
      border: none;
      background: #ff9800;
      color: white;
      font-weight: bold;
      border-radius: 5px;
      cursor: pointer;
      transition: 0.3s;
    }

    .product button:hover {
      background: #e68900;
    }

    /* About */
    .about {
      padding: 50px;
      background: #f1f1f1;
      text-align: center;
    }

    .about h2 {
      margin-bottom: 20px;
    }

    .about p {
      max-width: 600px;
      margin: auto;
      font-size: 16px;
      line-height: 1.6;
    }

    /* Contact */
    .contact {
      padding: 50px;
      text-align: center;
    }

    .contact form {
      max-width: 500px;
      margin: auto;
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    .contact input, .contact textarea {
      padding: 12px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    .contact button {
      padding: 12px;
      background: #111;
      color: white;
      font-weight: bold;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: 0.3s;
    }

    .contact button:hover {
      background: #ff9800;
    }

    /* Footer */
    footer {
      background: #111;
      color: white;
      padding: 20px;
      text-align: center;
      margin-top: 30px;
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <h1>SHOPIO</h1>
    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#products">Products</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="hero">
    <div>
      <h2>Welcome to SHOPIO - Your Electronics Store</h2>
      <button>Shop Now</button>
    </div>
  </section>

  <!-- Products -->
  <section class="products" id="products">
    <h2>Featured Electronics</h2>
    <div class="product-grid">
      <div class="product">
        <img src="https://via.placeholder.com/250" alt="Smartphone">
        <h3>Smartphone</h3>
        <p>Latest 5G Android Smartphone with high performance.</p>
        <button>Add to Cart</button>
      </div>
      <div class="product">
        <img src="https://via.placeholder.com/250" alt="Wireless Earbuds">
        <h3>Wireless Earbuds</h3>
        <p>Noise-cancelling Bluetooth earbuds with long battery life.</p>
        <button>Add to Cart</button>
      </div>
      <div class="product">
        <img src="https://via.placeholder.com/250" alt="Smartwatch">
        <h3>Smartwatch</h3>
        <p>Track fitness, health, and notifications on the go.</p>
        <button>Add to Cart</button>
      </div>
      <div class="product">
        <img src="https://via.placeholder.com/250" alt="Gaming Laptop">
        <h3>Gaming Laptop</h3>
        <p>High-speed laptop built for gaming and productivity.</p>
        <button>Add to Cart</button>
      </div>
      <div class="product">
        <img src="https://via.placeholder.com/250" alt="Bluetooth Speaker">
        <h3>Bluetooth Speaker</h3>
        <p>Portable waterproof speaker with deep bass.</p>
        <button>Add to Cart</button>
      </div>
      <div class="product">
        <img src="https://via.placeholder.com/250" alt="Power Bank">
        <h3>Power Bank</h3>
        <p>20000mAh fast charging power bank for all devices.</p>
        <button>Add to Cart</button>
      </div>
    </div>
  </section>

  <!-- About -->
  <section class="about" id="about">
    <h2>About SHOPIO</h2>
    <p>
      Welcome to SHOPIO!  
      We specialize in high-quality electronics, from smartphones and laptops to smartwatches and accessories.  
      SHOPIO is designed not just as a professional e-commerce platform, but also as a showcase of my portfolio as a B.Tech student and aspiring Software Engineer.
    </p>
  </section>

  <!-- Contact -->
  <section class="contact" id="contact">
    <h2>Contact Us</h2>
    <form>
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea rows="5" placeholder="Your Message"></textarea>
      <button type="submit">Send</button>
    </form>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 SHOPIO | Designed by Jatin</p>
  </footer>

</body>
</html>
source code

