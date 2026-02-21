
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SUPER STORE - Grocery, Dairy & Gift Mart</title>
    <style>
        :root {
            --primary-blue: #0056b3;
            --accent-red: #d9534f;
            --whatsapp-green: #25D366;
            --bg-light: #f4f7f6;
            --white: #ffffff;
            --bonn-gold: #f39c12;
        }

        * { box-sizing: border-box; }

        body { 
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif; 
            margin: 0; padding: 0; color: #333; line-height: 1.6; 
            background-color: var(--bg-light); text-align: center; 
        }
        
        /* Header */
        header { 
            background-color: var(--primary-blue); color: white; padding: 40px 20px; 
            border-bottom: 6px solid var(--accent-red);
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
        }
        header h1 { margin: 0; font-size: 2.5em; letter-spacing: 1px; }
        .sub-header { font-size: 1.2em; margin-top: 5px; opacity: 0.9; display: block; }
        
        /* Hero Section */
        .hero { padding: 30px 15px; max-width: 1200px; margin: 0 auto; }
        
        .card-info { 
            border-radius: 20px; max-width: 600px; margin: 0 auto 40px; 
            padding: 30px; background: var(--white); 
            box-shadow: 0 10px 30px rgba(0,0,0,0.1); border: 1px solid #eee;
        }
        
        .delivery-tag { 
            background: var(--accent-red); color: white; padding: 12px 25px; 
            border-radius: 50px; font-weight: bold; display: inline-block; 
            margin-bottom: 20px; font-size: 1.1em; animation: pulse 2s infinite; 
        }
        
        @keyframes pulse { 
            0% { transform: scale(1); } 
            70% { transform: scale(1.05); } 
            100% { transform: scale(1); } 
        }

        /* Buttons */
        .btn-container { display: flex; flex-direction: column; gap: 12px; align-items: center; margin: 20px 0; }
        
        .btn { 
            width: 90%; max-width: 350px; padding: 16px; text-decoration: none; 
            border-radius: 50px; font-weight: bold; font-size: 1.1em; 
            transition: 0.3s ease; display: flex; align-items: center; 
            justify-content: center; gap: 10px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);
        }
        .whatsapp-btn { background-color: var(--whatsapp-green); color: white; }
        .call-btn { background-color: var(--primary-blue); color: white; }
        .btn:hover { transform: translateY(-3px); opacity: 0.9; }

        /* Bonn Special Showcase */
        .bonn-section {
            background: #fff; border-radius: 20px; padding: 25px;
            margin: 20px auto 40px; border: 2px solid var(--bonn-gold);
            max-width: 1000px; box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        .bonn-header { border-bottom: 2px solid #fef5e7; padding-bottom: 15px; margin-bottom: 20px; }
        .bonn-header h2 { margin: 0; color: #d35400; font-style: italic; font-size: 1.8em; }
        .bonn-header p { margin: 5px 0 0; font-weight: bold; color: #7f8c8d; }

        .product-gallery {
            display: grid; grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
            gap: 15px;
        }
        .product-item {
            background: #fff9f0; padding: 15px; border-radius: 12px;
            border: 1px solid #ffeaa7; transition: 0.3s;
        }
        .product-item:hover { transform: translateY(-5px); border-color: var(--bonn-gold); }
        .product-item .img-box { font-size: 40px; margin-bottom: 8px; }
        .product-item p { font-size: 0.8em; font-weight: bold; margin: 0; color: #444; text-transform: uppercase; }

        /* General Product Categories */
        .product-grid { 
            display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); 
            gap: 20px; margin: 30px auto; 
        }
        
        .product-category { 
            background: var(--white); padding: 25px; border-radius: 15px; 
            transition: all 0.3s ease; border: 1px solid #ddd;
        }
        .product-category:hover { border-color: var(--primary-blue); transform: translateY(-5px); }
        .product-category .icon { font-size: 3em; margin-bottom: 10px; display: block; }
        .product-category h4 { margin: 10px 0; color: var(--primary-blue); font-size: 1.3em; border-bottom: 2px solid #f0f0f0; padding-bottom: 8px; }
        
        .brand-list { display: flex; flex-wrap: wrap; justify-content: center; gap: 6px; margin-top: 10px; }
        .brand-badge { 
            background: #eef2f7; color: #495057; padding: 4px 10px; 
            border-radius: 4px; font-weight: 600; font-size: 0.85em; border: 1px solid #dee2e6;
        }

        footer { background: #222; color: #ccc; padding: 40px 20px; margin-top: 60px; }
        .footer-contact { font-size: 1.2em; color: white; margin-top: 10px; font-weight: bold; }

        @media (max-width: 600px) {
            header h1 { font-size: 1.8em; }
            .product-grid { grid-template-columns: 1fr 1fr; gap: 10px; }
            .product-category { padding: 15px; }
            .product-category h4 { font-size: 1em; }
        }
    </style>
</head>
<body>

<header>
    <h1>SUPER STORE</h1>
    <span class="sub-header">Grocery, Dairy & Gift Mart</span>
    <p>📍 Near Munna Sweets, Sector 9/11</p>
</header>

<div class="hero">
    <div class="card-info">
        <div class="delivery-tag">🚚 FREE HOME DELIVERY</div>
        <h2 style="margin-top:0;">All Branded Products Available</h2>
        <p>🕒 <strong>Timing:</strong> 8:00 AM to 9:00 PM</p>
        
        <div class="btn-container">
            <a href="https://wa.me/919416882751?text=Hello%20Super%20Store!%20I%20want%20to%20place%20an%20order." class="btn whatsapp-btn">
                 💬 Order via WhatsApp
            </a>
            <a href="tel:+919416882751" class="btn call-btn">
                 📞 Call Now
            </a>
        </div>
    </div>

    <div class="bonn-section">
        <div class="bonn-header">
            <h2>Bread matlab BONN</h2>
            <p>Our Special Range</p>
        </div>
        <div class="product-gallery">
            <div class="product-item">
                <div class="img-box">🍞</div>
                <p>White Bread</p>
            </div>
            <div class="product-item">
                <div class="img-box">🌾</div>
                <p>High Fibre Brown</p>
            </div>
            <div class="product-item">
                <div class="img-box">🥨</div>
                <p>Multi Grain</p>
            </div>
            <div class="product-item">
                <div class="img-box">🥖</div>
                <p>100% Atta Bread</p>
            </div>
            <div class="product-item">
                <div class="img-box">🥪</div>
                <p>Whole Wheat</p>
            </div>
        </div>
    </div>

    <h3 style="color: var(--primary-blue); font-size: 1.8em; margin-bottom: 25px;">Product Categories</h3>
    
    <div class="product-grid">
        <div class="product-category">
            <span class="icon">🍪</span>
            <h4>Snacks & Namkeen</h4>
            <div class="brand-list">
                <span class="brand-badge">Haldiram</span>
                <span class="brand-badge">BC</span>
                <span class="brand-badge">Bikano</span>
                <span class="brand-badge">Sonu Namkeen</span>
            </div>
        </div>

        <div class="product-category">
            <span class="icon">🧼</span>
            <h4>Personal Care</h4>
            <div class="brand-list">
                <span class="brand-badge">Dove</span>
                <span class="brand-badge">Head & Shoulders</span>
                <span class="brand-badge">Clinic Plus</span>
                <span class="brand-badge">Colgate</span>
            </div>
        </div>

        <div class="product-category">
            <span class="icon">🧸</span>
            <h4>Toys</h4>
            <div class="brand-list">
                <span class="brand-badge" style="background: #fff3cd;">All Types Available</span>
            </div>
        </div>

        <div class="product-category">
            <span class="icon">🎁</span>
            <h4>Gift Items</h4>
            <div class="brand-list">
                <span class="brand-badge">Mugs</span>
                <span class="brand-badge">Frames</span>
                <span class="brand-badge">Birthday Decor</span>
            </div>
        </div>

        <div class="product-category">
            <span class="icon">🥛</span>
            <h4>Dairy Products</h4>
            <div class="brand-list">
                <span class="brand-badge">Amul</span>
                <span class="brand-badge">Vita</span>
                <span class="brand-badge">Fresh Paneer</span>
                <span class="brand-badge">Curd</span>
            </div>
        </div>

        <div class="product-category">
            <span class="icon">🌾</span>
            <h4>Staples & Oils</h4>
            <div class="brand-list">
                <span class="brand-badge">Aashirvaad</span>
                <span class="brand-badge">Fortune</span>
                <span class="brand-badge">Shakti Bhog</span>
            </div>
        </div>
    </div>
</div>

<footer>
    <p>&copy; 2026 SUPER STORE - Sector 9/11</p>
    <div class="footer-contact">
        Contact: 9416882751, 8168951112
    </div>
</footer>

</body>
</html>
<!DOCTYPE html>
<html>

