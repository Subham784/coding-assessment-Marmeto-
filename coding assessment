<<<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Embrace Sideboard</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f8f8f8;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        .product-container {
            display: flex;
            background: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
        }
        .product-image img {
            width: 300px;
            border-radius: 10px;
        }
        .product-details {
            margin-left: 20px;
            max-width: 400px;
        }
        .product-title {
            font-size: 24px;
            font-weight: 600;
        }
        .product-price {
            font-size: 20px;
            color: #388e3c;
            font-weight: 600;
        }
        .original-price {
            text-decoration: line-through;
            color: grey;
            font-size: 16px;
        }
        .discount {
            color: red;
            font-size: 14px;
        }
        .color-options, .size-options {
            display: flex;
            gap: 10px;
            margin: 10px 0;
        }
        .color-box {
            width: 30px;
            height: 30px;
            border-radius: 5px;
            cursor: pointer;
            border: 2px solid transparent;
        }
        .color-box.selected {
            border: 2px solid black;
        }
        .size-option {
            padding: 5px 10px;
            border: 1px solid black;
            cursor: pointer;
            border-radius: 5px;
        }
        .size-option.selected {
            background: black;
            color: white;
        }
        .quantity-selector {
            display: flex;
            align-items: center;
            gap: 10px;
        }
        .btn {
            background: #007bff;
            color: white;
            padding: 10px 15px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
            font-size: 16px;
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <div class="product-container">
        <div class="product-image">
            <img src="https://images.unsplash.com/photo-1598626430994-7514b6981e81" alt="Product Image">
        </div>
        <div class="product-details">
            <div class="product-title">Embrace Sideboard</div>
            <div class="product-price">$12999 <span class="original-price">$19999</span> <span class="discount">35% Off</span></div>
            <h4>Choose a Color</h4>
            <div class="color-options">
                <div class="color-box" style="background: #ECDECC;"></div>
                <div class="color-box" style="background: #BBD278;"></div>
                <div class="color-box" style="background: #BBC1F8;"></div>
                <div class="color-box" style="background: #FFD3F8;"></div>
            </div>
            <h4>Choose a Size</h4>
            <div class="size-options">
                <div class="size-option">Small</div>
                <div class="size-option">Medium</div>
                <div class="size-option">Large</div>
                <div class="size-option">Extra large</div>
                <div class="size-option">XXL</div>
            </div>
            <h4>Quantity</h4>
            <div class="quantity-selector">
                <button id="decrease">-</button>
                <span id="quantity">1</span>
                <button id="increase">+</button>
            </div>
            <button class="btn" id="addToCart">Add To Cart</button>
            <hr>
        </div>
    </div>

    <script>
        document.querySelectorAll('.color-box').forEach(color => {
            color.addEventListener('click', function() {
                document.querySelectorAll('.color-box').forEach(c => c.classList.remove('selected'));
                this.classList.add('selected');
            });
        });
        
        document.querySelectorAll('.size-option').forEach(size => {
            size.addEventListener('click', function() {
                document.querySelectorAll('.size-option').forEach(s => s.classList.remove('selected'));
                this.classList.add('selected');
            });
        });
        
        let quantity = 1;
        document.getElementById('increase').addEventListener('click', () => {
            quantity++;
            document.getElementById('quantity').textContent = quantity;
        });
        document.getElementById('decrease').addEventListener('click', () => {
            if (quantity > 1) {
                quantity--;
                document.getElementById('quantity').textContent = quantity;
            }
        });
        
        document.getElementById('addToCart').addEventListener('click', () => {
            alert('Added to cart!');
      
        });
    </script>
</body>
</html>
