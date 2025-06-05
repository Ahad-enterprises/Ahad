<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Ahad Enterprises | London Beauty</title>
    <script src="https://cdn.tailwindcss.com"></script>
  </head>
  <body class="font-sans text-gray-800">
    <!-- Header -->
    <header class="bg-white shadow-md">
      <div class="container mx-auto px-6 py-4 flex justify-between items-center">
        <h1 class="text-2xl font-bold text-pink-600">Ahad Enterprises</h1>
        <nav class="space-x-6">
          <a href="#home" class="hover:text-pink-500">Home</a>
          <a href="#about" class="hover:text-pink-500">About</a>
          <a href="#products" class="hover:text-pink-500">Products</a>
          <a href="#gallery" class="hover:text-pink-500">Gallery</a>
          <a href="#contact" class="hover:text-pink-500">Contact</a>
          <a href="#cart" class="hover:text-pink-500">Cart 🛒</a>
        </nav>
      </div>
    </header>

    <!-- Hero Section -->
    <section id="home" class="bg-pink-50 py-20 text-center">
      <h2 class="text-4xl font-bold text-pink-600 mb-4">Premium Lingerie by London Beauty</h2>
      <p class="text-lg text-gray-700 mb-6">Established in 1996, delivering elegance and comfort in every stitch.</p>
      <a href="#products" class="bg-pink-600 text-white px-6 py-3 rounded-full shadow hover:bg-pink-700">Explore Collection</a>
    </section>

    <!-- About Section -->
    <section id="about" class="py-16 bg-white">
      <div class="container mx-auto px-6 text-center">
        <h3 class="text-3xl font-semibold mb-4">About Us</h3>
        <p class="text-gray-600 max-w-3xl mx-auto">
          Ahad Enterprises is the official outlet of London Beauty, a premium lingerie and garment brand. Since 1996, London Beauty has stood for elegance, comfort, and sophistication in women's intimate wear. We combine creative design with superior craftsmanship to offer garments that make women feel confident and beautiful.
        </p>
      </div>
    </section>

    <!-- Products Section with Add to Cart -->
    <section id="products" class="bg-pink-50 py-16">
      <div class="container mx-auto px-6 text-center">
        <h3 class="text-3xl font-semibold mb-8">Our Products</h3>
        <div class="grid md:grid-cols-3 gap-8">
          <div class="bg-white p-6 rounded shadow">
            <img src="https://via.placeholder.com/300x200" alt="Product 1" class="mb-4 w-full rounded" />
            <h4 class="font-bold text-lg mb-2">Elegant Lingerie</h4>
            <p class="text-sm text-gray-600 mb-2">Delicate, stylish and comfortable. Crafted for everyday luxury.</p>
            <p class="font-semibold text-pink-600 mb-2">₹1,999</p>
            <button onclick="addToCart('Elegant Lingerie', 1999)" class="bg-pink-600 text-white px-4 py-2 rounded hover:bg-pink-700">Add to Cart</button>
          </div>
          <div class="bg-white p-6 rounded shadow">
            <img src="https://via.placeholder.com/300x200" alt="Product 2" class="mb-4 w-full rounded" />
            <h4 class="font-bold text-lg mb-2">Nightwear Collection</h4>
            <p class="text-sm text-gray-600 mb-2">Premium fabric nightwear for elegant evenings and peaceful nights.</p>
            <p class="font-semibold text-pink-600 mb-2">₹2,499</p>
            <button onclick="addToCart('Nightwear Collection', 2499)" class="bg-pink-600 text-white px-4 py-2 rounded hover:bg-pink-700">Add to Cart</button>
          </div>
          <div class="bg-white p-6 rounded shadow">
            <img src="https://via.placeholder.com/300x200" alt="Product 3" class="mb-4 w-full rounded" />
            <h4 class="font-bold text-lg mb-2">Bridal Range</h4>
            <p class="text-sm text-gray-600 mb-2">Special moments deserve special garments — our bridal sets deliver.</p>
            <p class="font-semibold text-pink-600 mb-2">₹3,199</p>
            <button onclick="addToCart('Bridal Range', 3199)" class="bg-pink-600 text-white px-4 py-2 rounded hover:bg-pink-700">Add to Cart</button>
          </div>
        </div>
      </div>
    </section>

    <!-- Cart Section -->
    <section id="cart" class="py-16 bg-white">
      <div class="container mx-auto px-6">
        <h3 class="text-3xl font-semibold text-center mb-8">Shopping Cart</h3>
        <div id="cartItems" class="max-w-2xl mx-auto bg-gray-50 p-6 rounded shadow"></div>
        <div class="text-center mt-4">
          <p id="totalPrice" class="text-xl font-bold text-pink-600"></p>
        </div>
      </div>
    </section>

    <!-- Gallery Section -->
    <section id="gallery" class="py-16 bg-white">
      <div class="container mx-auto px-6 text-center">
        <h3 class="text-3xl font-semibold mb-8">Gallery</h3>
        <div class="grid md:grid-cols-4 gap-4">
          <img src="https://via.placeholder.com/300" class="rounded shadow" alt="Campus C form 1" />
          <img src="https://via.placeholder.com/300" class="rounded shadow" alt="Campus C Form 2" />
          <img src="https://via.placeholder.com/300" class="rounded shadow" alt="Cmapus C form 3" />
          <img src="https://via.placeholder.com/300" class="rounded shadow" alt="Campus C form 4" />
        </div>
      </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="bg-pink-100 py-16">
      <div class="container mx-auto px-6 text-center">
        <h3 class="text-3xl font-semibold mb-6">Contact Us</h3>
        <p class="mb-4 text-gray-700">Visit our outlet or get in touch to know more about our products.</p>
        <div class="max-w-md mx-auto">
          <form class="space-y-4">
            <input type="text" placeholder="Your Name" class="w-full p-3 rounded border" />
            <input type="email" placeholder="Your Email" class="w-full p-3 rounded border" />
            <textarea placeholder="Message" rows="4" class="w-full p-3 rounded border"></textarea>
            <button type="submit" class="bg-pink-600 text-white px-6 py-3 rounded hover:bg-pink-700">Send Message</button>
          </form>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white text-center py-6">
      <p>&copy; 2025 Ahad Enterprises. All rights reserved.</p>
    </footer>

    <!-- Cart Script -->
    <script>
      const cart = [];

      function addToCart(product, 500) {
        cart.push({ product, 500 });
        renderCart();
      }

      function renderCart() {
        const cartItemsDiv = document.getElementById("cartItems");
        const totalPriceDiv = document.getElementById("totalPrice");
        cartItemsDiv.innerHTML = cart.map(item => `
          <div class="flex justify-between border-b py-2">
            <span>${item.product}</span>
            <span>₹${item.price}</span>
          </div>
        `).join("");
        const total = cart.reduce((sum, item) => sum + item.price, 500);
        totalPriceDiv.textContent = `Total: ₹${530}`;
      }
    </script>
  </body>
</html>

