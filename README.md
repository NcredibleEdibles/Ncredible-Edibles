# Ncredible-Edibles
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ncredible Edibles | Elevated Confections</title>
    <style>
        :root {
            --thc-green: #39ff14;
            --alert-red: #ff073a;
            --ui-black: #0a0a0a;
            --card-bg: #141414;
        }

        body {
            background-color: var(--ui-black);
            color: #e0e0e0;
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

        /* Top Warning Bar */
        .legal-bar {
            background: var(--alert-red);
            color: #000;
            text-align: center;
            font-size: 0.75rem;
            font-weight: bold;
            padding: 5px 0;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        header {
            text-align: center;
            padding: 60px 20px;
            border-bottom: 1px solid #222;
        }

        h1 {
            color: #fff;
            font-size: 3rem;
            margin: 0;
            letter-spacing: -1px;
        }

        h1 span { color: var(--thc-green); }

        .tagline {
            color: #666;
            font-size: 1rem;
            margin-top: 10px;
            text-transform: uppercase;
            letter-spacing: 3px;
        }

        .container {
            max-width: 1000px;
            margin: 40px auto;
            padding: 0 20px;
        }

        /* Product Display */
        .product-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
            margin-bottom: 60px;
        }

        .edible-card {
            background: var(--card-bg);
            border-radius: 20px;
            overflow: hidden;
            border: 1px solid #222;
            transition: 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }

        .edible-card:hover {
            border-color: var(--thc-green);
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(57, 255, 20, 0.1);
        }

        .img-box {
            width: 100%;
            height: 300px;
            background: #000;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #333;
            font-weight: bold;
            border-bottom: 2px solid var(--alert-red);
        }

        .details {
            padding: 25px;
        }

        .potency-badge {
            background: rgba(255, 7, 58, 0.15);
            color: var(--alert-red);
            padding: 4px 12px;
            border-radius: 50px;
            font-size: 0.7rem;
            font-weight: bold;
            text-transform: uppercase;
        }

        .product-name {
            font-size: 1.8rem;
            margin: 15px 0 10px 0;
        }

        .price {
            color: var(--thc-green);
            font-size: 1.4rem;
            font-weight: bold;
        }

        /* Contact Section */
        .contact-wrap {
            background: linear-gradient(145deg, #111, #080808);
            padding: 40px;
            border-radius: 30px;
            border: 1px solid #333;
        }

        .contact-wrap h2 {
            color: var(--thc-green);
            margin-top: 0;
        }

        .input-group {
            margin-bottom: 20px;
        }

        label {
            display: block;
            margin-bottom: 8px;
            font-size: 0.85rem;
            color: #888;
        }

        input, textarea {
            width: 100%;
            padding: 15px;
            background: #000;
            border: 1px solid #222;
            border-radius: 12px;
            color: #fff;
            font-size: 1rem;
        }

        input:focus {
            border-color: var(--thc-green);
            outline: none;
        }

        .btn-send {
            background: var(--alert-red);
            color: #fff;
            width: 100%;
            padding: 18px;
            border: none;
            border-radius: 12px;
            font-weight: bold;
            font-size: 1.1rem;
            cursor: pointer;
            transition: 0.3s;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .btn-send:hover {
            background: #cc0033;
            transform: scale(0.98);
        }

        footer {
            text-align: center;
            padding: 50px;
            color: #444;
            font-size: 0.8rem;
        }

        @media (max-width: 768px) {
            .product-grid { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>

    <div class="legal-bar">
        21+ ONLY | Please Consume Responsibly | Keep Out of Reach of Children
    </div>

    <header>
        <h1>Ncredible  <span>Edibles</span></h1>
        <div class="tagline">Premium THC Infusions</div>
    </header>

    <div class="container">
        
        <div class="product-grid">
            <div class="edible-card">
                <div class="img-box">IMAGE: FLAVOR_01</div>
                <div class="details">
                    <span class="potency-badge">High Potency</span>
                    <h2 class="product-name">Atomic Gummies</h2>
                    <div class="price">$35.00</div>
                    <p>Shatter-infused sour rings with a 50mg kick per piece. Clean, fast-acting, and delicious.</p>
                </div>
            </div>

            <div class="edible-card">
                <div class="img-box">IMAGE: FLAVOR_02</div>
                <div class="details">
                    <span class="potency-badge">Full Spectrum</span>
                    <h2 class="product-name">Midnight Fudge</h2>
                    <div class="price">$40.00</div>
                    <p>Indica-dominant dark chocolate. Crafted for deep sleep and full-body relaxation.</p>
                </div>
            </div>
        </div>

        <div class="contact-wrap">
            <h2>Secure Inquiry</h2>
            <p>Ready to experience the best? Send us a message for ordering details and local delivery zones.</p>
            
            <form>
                <div class="input-group">
                    <label>Preferred Name</label>
                    <input type="text" placeholder="How should we address you?">
                </div>
                <div class="input-group">
                    <label>Contact Method</label>
                    <input type="text" placeholder="Email or Phone Number">
                </div>
                <div class="input-group">
                    <label>Your Inquiry</label>
                    <textarea rows="4" placeholder="Which products are you interested in?"></textarea>
                </div>
                <button type="submit" class="btn-send">Send Inquiry</button>
            </form>
        </div>

    </div>

    <footer>
        &copy; 2020 Ncredible Edibles. All items are produced in compliance with local regulations.
    </footer>

</body>
</html>business website 
