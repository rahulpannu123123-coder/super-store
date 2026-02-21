
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
        }
        body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; margin: 0; padding: 0; color: #333; line-height: 1.6; background-color: var(--bg-light); text-align: center; }
        
        header { background-color: var(--primary-blue); color: white; padding: 40px 20px; border-bottom: 6px solid var(--accent-red); }
        header h1 { margin: 0; font-size: 2.2em; }
        
        .hero { padding: 30px 15px; }
        
        .card-info { border-radius: 20px; max-width: 600px; margin: 0 auto 40px; padding: 25px; background: white; box-shadow: 0 10px 25px rgba(0,0,0,0.1); border: 1px solid #eee; }
        
        .delivery-tag { background: var(--accent-red); color: white; padding: 10px 20px; border-radius: 50px; font-weight: bold; display: inline-block; margin-bottom: 20px; font-size: 1.1em; animation: pulse 2s infinite; }
        
        @keyframes pulse { 0% { transform: scale(1); } 50% { transform: scale(1.05); } 100% { transform: scale(1); } }

        .btn-container { display: flex; flex-direction: column; gap: 12px; align-items: center; margin: 20px 0; }
        
        .btn { width: 85%; max-width: 320px; padding: 15px; text-decoration: none; border-radius: 35px; font-weight: bold; font-size: 1.1em; transition: 0.3s; display: flex; align-items: center; justify-content: center; gap: 10px; }
        
        .whatsapp-btn { background-color: var(--whatsapp-green); color: white; }
        .call-btn { background-color: var(--primary-blue); color: white; }
        
        .product-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(160px, 1fr)); gap: 15px; max-width: 1000px; margin: 30px auto; padding: 0 20px; }
        
        .product-category { background: #fff; border: 1px solid #ddd; padding: 20px; border-radius: 15px; transition: 0.3s; display: flex; flex-direction: column; align-items: center; }
        .product-category:hover { border-color: var(--primary-blue); background: #f0f7ff; transform: translateY(-5px); }
        .product-category .icon { font-size: 2.2em; margin-bottom: 8px; }
        .product-category h4 { margin: 10px 0 5px; color: var(--primary-blue); font-size: 1.1em; border-bottom: 2px solid #f0f0f0; width: 100%; padding-bottom: 5px; }
        
        .brand-list { font-size: 0.85em; color: #555; margin-top: 8px; display: flex; flex-wrap: wrap; justify-content: center; gap: 5px; }
        .brand-badge { background: #e9ecef; color: #495057; padding: 2px 8px; border-radius: 4px; font-weight: bold; border: 1px solid #dee2e6; }
        .special-badge { background: #fff3cd; color: #856404; border: 1px solid #ffeeba; }

        footer { background: #222; color: #ccc; padding: 30px; margin-top: 50px; }
    </style>
</head>
<body>

<header>
    <h1>सुपर स्टोर (SUPER STORE)</h1>
    <p style="font-size: 1.3em; margin: 10px 0;"><strong>ग्रोसरी, डेयरी एवं गिफ्ट मार्ट</strong></p>
    <p>📍 मुन्ना स्वीट्स के पास, सेक्टर 9/11</p>
</header>

<div class="hero">
    <div class="card-info">
        <div class="delivery-tag">🚚 फ्री होम डिलीवरी (FREE DELIVERY)</div>
        <h2 style="margin-top:0;">सभी ब्रांडेड प्रोडक्ट्स उपलब्ध हैं</h2>
        <p>🕒 <strong>समय:</strong> सुबह 8:00 से रात 9:00 तक</p>
        
        <div class="btn-container">
            <a href="https://wa.me/919416882751?text=नमस्ते%20सुपर%20स्टोर!%20मुझे%20सामान%20ऑर्डर%20करना%20है।" class="btn whatsapp-btn">
                 WhatsApp पर ऑर्डर भेजें
            </a>
            <a href="tel:+919416882751" class="btn call-btn">
                 अभी कॉल करें
            </a>
        </div>
    </div>

    <h3 style="color: var(--primary-blue); font-size: 1.6em;">हमारे मुख्य उत्पाद</h3>
    
    <div class="product-grid">
        <div class="product-category">
            <span class="icon">🍞</span>
            <h4>ब्रेड (Bread)</h4>
            <div class="brand-list">
                <span class="brand-badge">Bonn</span>
                <span class="brand-badge">Harvest</span>
                <span class="brand-badge">Britannia</span>
                <span class="brand-badge">English Oven</span>
            </div>
        </div>

        <div class="product-category">
            <span class="icon">🍪</span>
            <h4>स्नैक्स (Snacks)</h4>
            <div class="brand-list">
                <span class="brand-badge">Haldiram</span>
                <span class="brand-badge">BC</span>
                <span class="brand-badge">Bikano</span>
                <span class="brand-badge">Sonu Namkeen</span>
            </div>
        </div>

        <div class="product-category">
            <span class="icon">🧼</span>
            <h4>कॉस्मेटिक्स</h4>
            <div class="brand-list">
                <span class="brand-badge">Dove</span>
                <span class="brand-badge">Head & Shoulders</span>
                <span class="brand-badge">Clinic Plus</span>
                <span class="brand-badge">Colgate</span>
            </div>
        </div>

        <div class="product-category">
            <span class="icon">🧸</span>
            <h4>खिलौने (Toys)</h4>
            <div class="brand-list">
                <span class="brand-badge special-badge">सभी प्रकार के खिलौने उपलब्ध</span>
            </div>
        </div>

        <div class="product-category">
            <span class="icon">🎁</span>
            <h4>गिफ्ट आइटम्स</h4>
            <div class="brand-list">
                <span class="brand-badge">Mugs</span>
                <span class="brand-badge">Frames</span>
                <span class="brand-badge">Birthday Items</span>
            </div>
        </div>

        <div class="product-category">
            <span class="icon">🥛</span>
            <h4>डेयरी उत्पाद</h4>
            <div class="brand-list">
                <span class="brand-badge">Amul</span>
                <span class="brand-badge">Vita</span>
                <span class="brand-badge">Paneer</span>
            </div>
        </div>

        <div class="product-category">
            <span class="icon">🌾</span>
            <h4>आटा एवं तेल</h4>
            <div class="brand-list">
                <span class="brand-badge">Aashirvaad</span>
                <span class="brand-badge">Fortune</span>
            </div>
        </div>
    </div>
</div>

<footer>
    <p>&copy; 2026 सुपर स्टोर ग्रोसरी एवं गिफ्ट मार्ट - सेक्टर 9/11</p>
    <p>संपर्क: 9416882751, 8168951112</p>
</footer>

</body>
</html>
