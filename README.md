
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gaming Recharge</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background-color: #1e1e2f;
            color: #fff;
        }

        .header {
            background: linear-gradient(90deg, #3a3a5a, #222);
            padding: 1em 0;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.5);
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8em;
            font-weight: bold;
            color: #ff9900;
        }

        .games {
            padding: 3em 1em;
            text-align: center;
        }

        .game {
            background: #292942;
            border-radius: 10px;
            padding: 1.5em;
            width: 200px;
            text-align: center;
            margin: 0 auto;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .game:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
        }

        .game img {
            width: 100%;
            height: 120px;
            border-radius: 5px;
            object-fit: cover;
            margin-bottom: 1em;
        }

        .game h4 {
            margin: 0.5em 0;
            font-size: 1.2em;
        }

        .diamond-list {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            margin-top: 2em;
        }

        .diamond-package {
            background-color: #292942;
            padding: 1.5em;
            border-radius: 10px;
            width: 200px;
            text-align: center;
            margin: 1em;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }

        .diamond-package h4 {
            font-size: 1.5em;
        }

        .diamond-package p {
            font-size: 1.2em;
            margin: 1em 0;
        }

        .diamond-package .btn-pay {
            background: #28a745;
            color: #fff;
            padding: 10px 20px;
            text-decoration: none;
            border-radius: 5px;
            font-size: 1em;
            display: inline-block;
        }

        .diamond-package .btn-pay:hover {
            background: #218838;
        }

        .footer {
            background: #222;
            color: #aaa;
            text-align: center;
            padding: 1.5em 0;
            margin-top: 2em;
            font-size: 0.9em;
        }

        .footer p a {
            color: #ff9900;
            text-decoration: none;
        }

        .input-field {
            background-color: #292942;
            padding: 1em;
            border-radius: 5px;
            width: 100%;
            margin: 1em 0;
            color: #fff;
            border: none;
        }

        .external-link img {
            width: 150px;
            margin-top: 2em;
            cursor: pointer;
        }
    </style>
</head>
<body>

    <header class="header">
        <div class="container">
            <h1 class="logo">GameTopUp</h1>
        </div>
    </header>

    <main>
        <section class="games">
            <h3>Select Your Game</h3>
            <!-- Mobile Legends Game -->
            <div class="game">
                <img src="https://upload.wikimedia.org/wikipedia/commons/1/1f/Mobile_Legends_Logo_2020.png" alt="Mobile Legends">
                <h4>Mobile Legends Recharge</h4>
                <button class="btn-pay" onclick="showRechargeForm()">Buy Now</button>
            </div>
        </section>

        <!-- Diamond Price List -->
        <section class="diamond-list">
            <div class="diamond-package">
                <h4>100 Diamonds</h4>
                <p>Price: $1.99</p>
                <button class="btn-pay">Buy Now</button>
            </div>
            <div class="diamond-package">
                <h4>500 Diamonds</h4>
                <p>Price: $8.99</p>
                <button class="btn-pay">Buy Now</button>
            </div>
            <div class="diamond-package">
                <h4>1200 Diamonds</h4>
                <p>Price: $19.99</p>
                <button class="btn-pay">Buy Now</button>
            </div>
            <div class="diamond-package">
                <h4>2500 Diamonds</h4>
                <p>Price: $39.99</p>
                <button class="btn-pay">Buy Now</button>
            </div>
        </section>

        <!-- Recharge Form Section (Initially Hidden) -->
        <section id="recharge-form" style="display:none; padding: 2em 1em; text-align: center;">
            <h3>Enter Your Server ID for Recharge</h3>
            <form id="payment-form" action="#" method="POST">
                <input class="input-field" type="text" name="server-id" placeholder="Enter Server ID" required>
                <br>
                <button type="submit" class="btn-pay">Proceed to Payment</button>
            </form>
        </section>

        <!-- External link section -->
        <section class="external-link" style="text-align:center;">
            <a href="https://ibb.co/VqCv3MP" target="_blank">
                <img src="https://i.ibb.co/W2zcsBY/ec9dd32c001ab51f4637a6d56b0e22e1.png" alt="ec9dd32c001ab51f4637a6d56b0e22e1">
            </a>
        </section>

    </main>

    <footer class="footer">
        <p>&copy; 2024 GameTopUp. All Rights Reserved.</p>
    </footer>

    <script>
        // Function to show the recharge form when "Buy Now" button is clicked
        function showRechargeForm() {
            // Hide the game section and show the recharge form
            document.querySelector('.games').style.display = 'none';
            document.getElementById('recharge-form').style.display = 'block';
        }
    </script>
</body>
</html>
