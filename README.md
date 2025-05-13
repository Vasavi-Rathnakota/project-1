<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple E-commerce Website</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Simple E-commerce</h1>
        <div id="cart-container">
            <button onclick="viewCart()">View Cart (<span id="cart-count">0</span>)</button>
        </div>
    </header>

    <main>
        <div class="product-list">
            <!-- Example products -->
            <div class="product">
                <img src="https://via.placeholder.com/150" alt="Product 1">
                <h3>Product 1</h3>
                <p>$100</p>
                <button onclick="addToCart('Product 1', 100)">Add to Cart</button>
            </div>

            <div class="product">
                <img src="https://via.placeholder.com/150" alt="Product 2">
                <h3>Product 2</h3>
                <p>$150</p>
                <button onclick="addToCart('Product 2', 150)">Add to Cart</button>
            </div>

            <div class="product">
                <img src="https://via.placeholder.com/150" alt="Product 3">
                <h3>Product 3</h3>
                <p>$200</p>
                <button onclick="addToCart('Product 3', 200)">Add to Cart</button>
            </div>
        </div>
    </main>

    <div id="cart-modal" class="modal">
        <div class="modal-content">
            <h2>Your Cart</h2>
            <ul id="cart-items"></ul>
            <p>Total: $<span id="total-price">0</span></p>
            <button onclick="checkout()">Checkout</button>
            <button onclick="closeCart()">Close</button>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
