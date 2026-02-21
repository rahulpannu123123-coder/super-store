
<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>सुपर स्टोर - ग्रोसरी, डेयरी एवं गिफ्ट मार्ट</title>
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
        
        header { 
            background-color: var(--primary-blue); color: white; padding: 40px 20px; 
            border-bottom: 6px solid var(--accent-red);
        }
        header h1 { margin: 0; font-size: 2.5em; }

        .hero { padding: 30px 15px; max-width: 1200px; margin: 0 auto; }
        
        .card-info { 
            border-radius: 20px; max-width: 600px; margin: 0 auto 40px; 
            padding: 30px; background: var(--white); 
            box-shadow: 0 10px 30px rgba(0,0,0,0.1); 
        }
        
        .delivery-tag { 
            background: var(--accent-red); color: white; padding: 12px 25px; 
            border-radius: 50px; font-weight: bold; display: inline-block; 
            margin-bottom: 20px; animation: pulse 2s infinite; 
        }
        
        @keyframes pulse { 
            0% { transform: scale(1); } 
            70% { transform: scale(1.05); } 
            100% { transform: scale(1); } 
        }

        /* Bonn Special Section */
        .bonn-section {
            background: #fff; border-radius: 20px; padding: 25px;
            margin: 20px auto 40px; border: 2px solid var(--bonn-gold);
            max-width: 1000px;
        }
        .bonn-header { color: #d35400; border-bottom: 2px solid #eee; padding-bottom: 10px; margin-bottom: 20px; }
        .bonn-header h2 { margin: 0; font-style: italic; }

        .product-gallery {
            display: grid; grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 15px;
        }
        .product-item {
            background: #fff9f0; padding: 15px; border-radius: 10px;
            border: 1px solid #ffeaa7; transition: 0.3s;
        }
        .product-item:hover { transform: scale(1.05); background: #fdf2e9; }
        .product-item img { width: 60px; height: 60px; margin-bottom: 10px; } /* आइकॉन की तरह */
        .product-item p { font-size: 0.85em; font-weight: bold; margin: 0; color: #555; }

        /* General Product Grid */
        .product-grid { 
            display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); 
            gap: 20px; margin: 30px auto; 
        }
        
        .product-category { 
            background: var(--white); padding: 25px; border-radius: 15px; 
            transition: all 0.3s ease; box-shadow: 0 2px 10px rgba(0,0,0,0.05);
        }
        .product-category:hover { transform: translateY(-8px); box-shadow: 0 15px 30px rgba(0,0,0,0.1); }
        .product-category .icon { font-size: 3em; }
        
        .brand-list { display: flex; flex-wrap: wrap; justify-content: center; gap: 8px; margin-top: 10px; }
        .brand-badge { 
            background: #eef2f7; color: #495057; padding: 5px 12px; 
            border-radius: 6px; font-weight: 600; font-size: 0.9em; 
        }

        .btn { 
            width: 90%; max-width: 350px; padding: 16px; text-decoration: none; 
            border-radius: 50px; font-weight: bold; display: flex; 
            align-items: center; justify-content: center; gap: 12px; margin: 10px auto;
        }
        .whatsapp-btn { background-color: var(--whatsapp-green); color: white; }
        .call-btn { background-color: var(--primary-blue); color: white; }

        footer { background: #222; color: #eee; padding: 40px 20px; margin-top: 60px; }

        @media (max-width: 600px) {
            .product-grid { grid-template-columns: 1fr 1fr; }
            .product-gallery { grid-template-columns: 1fr 1fr; }
        }
    </style>
</head>
<body>

<header>
    <h1>सुपर स्टोर (SUPER STORE)</h1>
    <p><strong>ग्रोसरी, डेयरी एवं गिफ्ट मार्ट</strong></p>
    <p>📍 मुन्ना स्वीट्स के पास, सेक्टर 9/11</p>
</header>

<div class="hero">
    <div class="card-info">
        <div class="delivery-tag">🚚 फ्री होम डिलीवरी</div>
        <h2>Bread matlab BONN 🍞</h2>
        <div class="btn-container">
            <a href="https://wa.me/919416882751" class="btn whatsapp-btn">💬 WhatsApp ऑर्डर</a>
            <a href="tel:+919416882751" class="btn call-btn">📞 अभी कॉल करें</a>
        </div>
    </div>

    <div class="bonn-section">
        <div class="bonn-header">
            <h2>Bonn Special Gallery</h2>
            <p>"Bread matlab Bonn"</p>
        </div>
        <main class="product-gallery">
            <div class="product-item">
                <div style="font-size: 40px;">🍞</div>
                <p>WHITE BREAD</p>
            </div>
            <div class="product-item">
                <div style="font-size: 40px;">🌾</div>
                <p>HIGH FIBRE BROWN</p>
            </div>
            <div class="product-item">
                <div style="font-size: 40px;">🥨</div>
                <p>MULTI GRAIN</p>
            </div>
            <div class="product-item">
                <div style="font-size: 40px;">🥖</div>
                <p>100% ATTA BREAD</p>
            </div>
            <div class="product-item">
                <div style="font-size: 40px;">🥪</div>
                <p>WHOLE WHEAT</p>
            </div>
        </main>
    </div>

    <h3 style="color: var(--primary-blue); font-size: 1.8em;">अन्य उत्पाद श्रेणियाँ</h3>
    
    <div class="product-grid">
        <div class="product-category">
            <span class="icon">🍪</span>
            <h4>स्नैक्स (Snacks)</h4>
            <div class="brand-list">
                <span class="brand-badge">Haldiram</span>
                <span class="brand-badge">BC</span>
                <span class="brand-badge">Bikano</span>
            </div>
        </div>

        <div class="product-category">
            <span class="icon">🧼</span>
            <h4>कॉस्मेटिक्स</h4>
            <div class="brand-list">
                <span class="brand-badge">Dove</span>
                <span class="brand-badge">Head & Shoulders</span>
                <span class="brand-badge">Colgate</span>
            </div>
        </div>

        <div class="product-category">
            <span class="icon">🧸</span>
            <h4>खिलौने एवं गिफ्ट</h4>
            <div class="brand-list">
                <span class="brand-badge">All Toys</span>
                <span class="brand-badge">Photo Frames</span>
            </div>
        </div>

        <div class="product-category">
            <span class="icon">🥛</span>
            <h4>डेयरी</h4>
            <div class="brand-list">
                <span class="brand-badge">Amul</span>
                <span class="brand-badge">Vita</span>
                <span class="brand-badge">Paneer</span>
            </div>
        </div>
    </div>
</div>

<footer>
    <p>&copy; 2026 सुपर स्टोर - सेक्टर 9/11 | संपर्क: 9416882751</p>
</footer>

</body>
</html>
