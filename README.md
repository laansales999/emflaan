<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exquisite Madiwa Flavors</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }
        
        :root {
            --primary-blue: #0c4da2;
            --dark-blue: #0a192f;
            --gold: #f59e0b;
            --light-bg: rgba(255, 255, 255, 0.05);
            --light-text: #f8f8f8;
            --dark-text: #1e293b;
        }
        
        body {
            background: linear-gradient(135deg, var(--dark-blue) 0%, #1e3a8a 100%);
            color: var(--light-text);
            line-height: 1.6;
            padding-bottom: 80px;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        /* Header Styles */
        .main-header {
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px 0;
            margin-bottom: 30px;
            border-bottom: 2px solid var(--gold);
        }
        
        .logo-container {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .logo {
            width: 180px;
            height: auto;
        }
        
        .tagline {
            font-style: italic;
            color: var(--gold);
            margin-top: 10px;
            font-size: 1.2rem;
        }
        
        /* Footer Styles */
        footer {
            background: var(--dark-blue);
            padding: 40px 0;
            margin-top: 60px;
            border-top: 2px solid var(--gold);
        }
        
        .footer-content {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            gap: 30px;
        }
        
        .footer-about {
            flex: 2;
            min-width: 300px;
        }
        
        .footer-about h3 {
            color: var(--gold);
            margin-bottom: 15px;
            font-size: 1.5rem;
        }
        
        .footer-about p {
            margin-bottom: 15px;
            line-height: 1.8;
        }
        
        .footer-contact {
            flex: 1;
            min-width: 250px;
        }
        
        .footer-contact h3 {
            color: var(--gold);
            margin-bottom: 15px;
            font-size: 1.5rem;
        }
        
        .footer-contact p {
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .footer-bottom {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .location-prompt {
            background: rgba(14, 165, 233, 0.15);
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            margin-bottom: 30px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .location-prompt h2 {
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }
        
        .btn {
            background: var(--gold);
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 50px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
            display: inline-block;
            margin-top: 15px;
        }
        
        .btn:hover {
            background: #d97706;
            transform: translateY(-2px);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        
        .event-section {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            margin-bottom: 40px;
            align-items: center;
        }
        
        .event-image {
            flex: 1;
            min-width: 300px;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }
        
        .event-image img {
            width: 100%;
            height: auto;
            display: block;
        }
        
        .event-description {
            flex: 2;
            min-width: 300px;
            background: var(--light-bg);
            padding: 25px;
            border-radius: 10px;
            backdrop-filter: blur(10px);
        }
        
        .event-description h2 {
            color: var(--primary-blue);
            margin-bottom: 15px;
            font-size: 28px;
        }
        
        .event-description p {
            margin-bottom: 15px;
            font-size: 16px;
            line-height: 1.8;
        }
        
        .exclusive-tag {
            background: linear-gradient(135deg, var(--gold), #ef4444);
            color: white;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 14px;
            font-weight: 600;
            display: inline-block;
            margin-bottom: 15px;
        }
        
        .emf-poster {
            text-align: center;
            margin: 40px 0;
        }
        
        .emf-poster img {
            max-width: 100%;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }
        
        .special-offer {
            background: linear-gradient(135deg, var(--gold), #ef4444);
            padding: 15px;
            border-radius: 10px;
            text-align: center;
            margin: 20px 0;
            animation: pulse 2s infinite;
        }
        
        .menu-section {
            margin: 40px 0;
        }
        
        .menu-category {
            margin-bottom: 40px;
        }
        
        .menu-category h3 {
            color: var(--primary-blue);
            border-bottom: 2px solid var(--primary-blue);
            padding-bottom: 10px;
            margin-bottom: 20px;
            font-size: 24px;
        }
        
        .menu-items {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }
        
        .menu-item {
            background: var(--light-bg);
            border-radius: 10px;
            padding: 20px;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .menu-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .item-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 10px;
        }
        
        .item-name {
            font-weight: 600;
            font-size: 18px;
            color: var(--light-text);
        }
        
        .item-price {
            color: var(--gold);
            font-weight: 700;
        }
        
        .item-desc {
            color: #cbd5e1;
            font-size: 14px;
            margin-bottom: 15px;
        }
        
        .size-options {
            display: flex;
            gap: 10px;
            margin-bottom: 15px;
            flex-wrap: wrap;
        }
        
        .size-btn {
            padding: 5px 10px;
            border-radius: 20px;
            border: 1px solid var(--primary-blue);
            background: transparent;
            color: var(--light-text);
            cursor: pointer;
            font-size: 12px;
            transition: all 0.3s ease;
        }
        
        .size-btn.active {
            background: var(--primary-blue);
            color: white;
        }
        
        .item-controls {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .quantity-controls {
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .quantity-btn {
            background: var(--primary-blue);
            color: white;
            border: none;
            width: 30px;
            height: 30px;
            border-radius: 50%;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .quantity {
            font-weight: 600;
            width: 30px;
            text-align: center;
        }
        
        .limited-edition {
            background: linear-gradient(135deg, var(--gold), #ef4444);
            color: white;
            padding: 3px 10px;
            border-radius: 15px;
            font-size: 12px;
            font-weight: 600;
            display: inline-block;
            margin-top: 10px;
        }
        
        /* Drink Sizes Section */
        .drink-sizes {
            text-align: center;
            margin: 40px 0;
            padding: 20px;
            background: var(--light-bg);
            border-radius: 10px;
            backdrop-filter: blur(10px);
        }
        
        .drink-sizes h3 {
            color: var(--primary-blue);
            margin-bottom: 20px;
        }
        
        .drink-sizes img {
            max-width: 100%;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }
        
        /* Floating Cart */
        .floating-cart {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background: var(--light-bg);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            padding: 15px;
            width: 320px;
            box-shadow: 0 5px 25px rgba(0, 0, 0, 0.3);
            z-index: 1000;
            max-height: 400px;
            overflow-y: auto;
        }
        
        .cart-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
            padding-bottom: 10px;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .cart-items {
            max-height: 200px;
            overflow-y: auto;
            margin-bottom: 15px;
        }
        
        .cart-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 8px 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
            font-size: 14px;
        }
        
        .cart-item-info {
            flex: 2;
        }
        
        .cart-item-controls {
            display: flex;
            align-items: center;
            gap: 8px;
        }
        
        .remove-btn {
            color: #ef4444;
            background: none;
            border: none;
            cursor: pointer;
            font-size: 14px;
        }
        
        .cart-total {
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-weight: 700;
            font-size: 18px;
            padding-top: 10px;
            border-top: 2px solid rgba(255, 255, 255, 0.1);
        }
        
        .checkout-btn {
            width: 100%;
            padding: 12px;
            background: linear-gradient(135deg, #10b981, #059669);
            color: white;
            border: none;
            border-radius: 50px;
            font-weight: 600;
            font-size: 16px;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-top: 15px;
        }
        
        .checkout-form {
            background: var(--light-bg);
            border-radius: 10px;
            padding: 25px;
            margin-top: 40px;
            display: none;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
        }
        
        .form-group input, .form-group textarea, .form-group select {
            width: 100%;
            padding: 12px 15px;
            border-radius: 8px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            background: rgba(255, 255, 255, 0.1);
            color: white;
        }
        
        .form-group input:focus, .form-group textarea:focus, .form-group select:focus {
            outline: none;
            border-color: var(--primary-blue);
        }
        
        .payment-info {
            background: rgba(14, 165, 233, 0.1);
            padding: 15px;
            border-radius: 8px;
            margin: 20px 0;
            border-left: 4px solid var(--primary-blue);
        }
        
        .payment-info h4 {
            color: var(--gold);
            margin-bottom: 10px;
        }
        
        .whatsapp-chat {
            position: fixed;
            bottom: 90px;
            right: 20px;
            background: #25D366;
            color: white;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 28px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
            z-index: 1000;
            transition: all 0.3s ease;
        }
        
        .whatsapp-chat:hover {
            transform: scale(1.1);
        }
        
        .cart-toggle {
            position: fixed;
            bottom: 20px;
            left: 20px;
            background: var(--gold);
            color: white;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
            z-index: 1000;
            transition: all 0.3s ease;
            cursor: pointer;
        }
        
        .cart-badge {
            position: absolute;
            top: -5px;
            right: -5px;
            background: #ef4444;
            color: white;
            width: 24px;
            height: 24px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 12px;
            font-weight: 600;
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.02); }
            100% { transform: scale(1); }
        }
        
        @media (max-width: 768px) {
            .event-section {
                flex-direction: column;
            }
            
            .menu-items {
                grid-template-columns: 1fr;
            }
            
            .floating-cart {
                width: 90%;
                left: 5%;
                right: 5%;
                bottom: 80px;
            }
            
            .footer-content {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header with Logo -->
        <header class="main-header">
            <div class="logo-container">
                <img src="https://i.postimg.cc/nARGcNerCwMY4raf6/logo.png" alt="Laansale Logo" class="logo">
                <div class="tagline">Premium Culinary Experiences</div>
            </div>
        </header>

        <!-- Location Prompt Section -->
        <section class="location-prompt">
            <h2><i class="fas fa-location-dot"></i> Enable Your Location</h2>
            <p>To serve you better and provide accurate delivery, please enable location services</p>
            <button class="btn" id="enableLocation">Enable Location</button>
            <p id="locationStatus" style="margin-top: 15px;"></p>
        </section>

        <!-- Event Section -->
        <section class="event-section">
            <div class="event-image">
                <img src="https://i.postimg.cc/XfAk1ncbHZJsvYnq7/event-poster.jpg" alt="Bustani Gardens Event">
            </div>
            <div class="event-description">
                <span class="exclusive-tag">EXCLUSIVE EVENT</span>
                <h2>Bustani Gardens Masterclass Experience</h2>
                <p>Join us for an exclusive culinary experience at Bustani Gardens, Red Hill. This is not just an event—it's a transformation for the top 0.00001% who understand that marketing excellence is the key to domination in any field.</p>
                <p>Laansale101 and Exquisite Madiwa Flavors present a fusion of elite taste and marketing mastery. Learn how to capture attention, create desire, and command loyalty through sensory experience.</p>
                <p>This is where the extraordinary is ordinary, and the exceptional is expected.</p>
                <button class="btn">Reserve Your Spot</button>
            </div>
        </section>

        <!-- EMF Poster Section -->
        <section class="emf-poster">
            <img src="https://i.postimg.cc/X1jPEzpdiF8C4Vzm7/emf-poster.jpg" alt="EMF Feel Me More">
        </section>

        <!-- Special Offer Banner -->
        <div class="special-offer">
            <h3>⏰ Limited Time Offer! 🚀</h3>
            <p>Order in the first 20 minutes of any hour and get 10% OFF your entire order!</p>
            <p id="countdown" style="font-weight: bold; margin-top: 10px;"></p>
        </div>

        <!-- Drink Sizes Reference -->
        <section class="drink-sizes">
            <h3>Our Drink Sizes</h3>
            <img src="https://i.postimg.cc/rGdxLgYY3YLFbeht5/drink-sizes.jpg" alt="Drink Sizes Reference">
            <p style="margin-top: 15px;">Small (350ml) | Medium (500ml) | Large (750ml)</p>
        </section>

        <!-- Menu Section -->
        <section class="menu-section">
            <div class="menu-category">
                <h3>FRISS & 'KAK!</h3>
                <div class="menu-items">
                    <div class="menu-item">
                        <div class="item-header">
                            <span class="item-name">Classic Crunch</span>
                            <span class="item-price">450/-</span>
                        </div>
                        <img src="https://i.postimg.cc/Qznj3k2uNqu2196F6/classic-crunch.jpg" alt="Classic Crunch" style="width:100%; border-radius:8px; margin-bottom:10px;">
                        <p class="item-desc">FRIES + 10 PCS MISHIKAKI + CHEF'S SIGNATURE SAUCE</p>
                        <span class="limited-edition">Limited Edition</span>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="classic-crunch">-</button>
                                <span class="quantity" data-item="classic-crunch">0</span>
                                <button class="quantity-btn plus" data-item="classic-crunch">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="classic-crunch" data-price="450">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="menu-item">
                        <div class="item-header">
                            <span class="item-name">Grand Sultan</span>
                            <span class="item-price">550/-</span>
                        </div>
                        <img src="https://i.postimg.cc/s7gZsW7nuq75eEDe8/grand-sultan.jpg" alt="Grand Sultan" style="width:100%; border-radius:8px; margin-bottom:10px;">
                        <p class="item-desc">MEGA FRIES LOADED WITH 15 PCS MISHIKAKI + SPECIAL SAUCE</p>
                        <p class="item-desc">EXTRA MISHIKAKI @100/- PER SKEWER</p>
                        <span class="limited-edition">Limited Edition</span>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="grand-sultan">-</button>
                                <span class="quantity" data-item="grand-sultan">0</span>
                                <button class="quantity-btn plus" data-item="grand-sultan">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="grand-sultan" data-price="550">Add to Cart</button>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="menu-category">
                <h3>FRESH JUICE</h3>
                <div class="menu-items">
                    <div class="menu-item">
                        <div class="item-header">
                            <span class="item-name">Tangy Passion</span>
                            <span class="item-price" id="price-tangy-passion">250/-</span>
                        </div>
                        <img src="https://i.postimg.cc/2Ygd3YT3pHXTA7Sa6/tangy-passion.jpg" alt="Tangy Passion" style="width:100%; border-radius:8px; margin-bottom:10px;">
                        <p class="item-desc">Bold Passion, Pure Tropical Energy</p>
                        <div class="size-options">
                            <button class="size-btn active" data-item="tangy-passion" data-size="small" data-price="250">Small: 250/-</button>
                            <button class="size-btn" data-item="tangy-passion" data-size="medium" data-price="350">Medium: 350/-</button>
                            <button class="size-btn" data-item="tangy-passion" data-size="large" data-price="450">Large: 450/-</button>
                        </div>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="tangy-passion">-</button>
                                <span class="quantity" data-item="tangy-passion">0</span>
                                <button class="quantity-btn plus" data-item="tangy-passion">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="tangy-passion" data-price="250">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="menu-item">
                        <div class="item-header">
                            <span class="item-name">Mango Rush</span>
                            <span class="item-price" id="price-mango-rush">250/-</span>
                        </div>
                        <img src="https://i.postimg.cc/EFm1bkQsoTjM7SHT7/mango-rush.jpg" alt="Mango Rush" style="width:100%; border-radius:8px; margin-bottom:10px;">
                        <p class="item-desc">Thick, Juicy, Naturally Sweet</p>
                        <div class="size-options">
                            <button class="size-btn active" data-item="mango-rush" data-size="small" data-price="250">Small: 250/-</button>
                            <button class="size-btn" data-item="mango-rush" data-size="medium" data-price="350">Medium: 350/-</button>
                            <button class="size-btn" data-item="mango-rush" data-size="large" data-price="450">Large: 450/-</button>
                        </div>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="mango-rush">-</button>
                                <span class="quantity" data-item="mango-rush">0</span>
                                <button class="quantity-btn plus" data-item="mango-rush">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="mango-rush" data-price="250">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="menu-item">
                        <div class="item-header">
                            <span class="item-name">Le' Pineapple De' Mint</span>
                            <span class="item-price" id="price-pineapple-mint">250/-</span>
                        </div>
                        <img src="https://i.postimg.cc/v9ZGdZyQnjnstkeU8/pineapple-mint.jpg" alt="Le Pineapple De Mint" style="width:100%; border-radius:8px; margin-bottom:10px;">
                        <p class="item-desc">Altuty Breeze, Pineapple Squeeze</p>
                        <div class="size-options">
                            <button class="size-btn active" data-item="pineapple-mint" data-size="small" data-price="250">Small: 250/-</button>
                            <button class="size-btn" data-item="pineapple-mint" data-size="medium" data-price="350">Medium: 350/-</button>
                            <button class="size-btn" data-item="pineapple-mint" data-size="large" data-price="450">Large: 450/-</button>
                        </div>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="pineapple-mint">-</button>
                                <span class="quantity" data-item="pineapple-mint">0</span>
                                <button class="quantity-btn plus" data-item="pineapple-mint">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="pineapple-mint" data-price="250">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="menu-item">
                        <div class="item-header">
                            <span class="item-name">Tropical Mix</span>
                            <span class="item-price" id="price-tropical-mix">250/-</span>
                        </div>
                        <img src="https://i.postimg.cc/F94GZtEZRnqAi6KCA/tropical-mix.jpg" alt="Tropical Mix" style="width:100%; border-radius:8px; margin-bottom:10px;">
                        <p class="item-desc">All-in-one island infusion</p>
                        <div class="size-options">
                            <button class="size-btn active" data-item="tropical-mix" data-size="small" data-price="250">Small: 250/-</button>
                            <button class="size-btn" data-item="tropical-mix" data-size="medium" data-price="350">Medium: 350/-</button>
                            <button class="size-btn" data-item="tropical-mix" data-size="large" data-price="450">Large: 450/-</button>
                        </div>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="tropical-mix">-</button>
                                <span class="quantity" data-item="tropical-mix">0</span>
                                <button class="quantity-btn plus" data-item="tropical-mix">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="tropical-mix" data-price="250">Add to Cart</button>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="menu-category">
                <h3>MAGIC MOJITOS</h3>
                <div class="menu-items">
                    <div class="menu-item">
                        <div class="item-header">
                            <span class="item-name">Blue Lagoon</span>
                            <span class="item-price" id="price-blue-lagoon">300/-</span>
                        </div>
                        <img src="https://i.postimg.cc/2NFRzaT3f9k6ZZgm9/blue-lagoon.jpg" alt="Blue Lagoon" style="width:100%; border-radius:8px; margin-bottom:10px;">
                        <p class="item-desc">Tropical Citrus Wave, Blue Ocean</p>
                        <div class="size-options">
                            <button class="size-btn active" data-item="blue-lagoon" data-size="small" data-price="300">Small: 300/-</button>
                            <button class="size-btn" data-item="blue-lagoon" data-size="medium" data-price="400">Medium: 400/-</button>
                            <button class="size-btn" data-item="blue-lagoon" data-size="large" data-price="500">Large: 500/-</button>
                        </div>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="blue-lagoon">-</button>
                                <span class="quantity" data-item="blue-lagoon">0</span>
                                <button class="quantity-btn plus" data-item="blue-lagoon">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="blue-lagoon" data-price="300">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="menu-item">
                        <div class="item-header">
                            <span class="item-name">Red Flash</span>
                            <span class="item-price" id="price-red-flash">300/-</span>
                        </div>
                        <img src="https://i.postimg.cc/SGoJnZLtRHwUxKqF9/red-flash.jpg" alt="Red Flash" style="width:100%; border-radius:8px; margin-bottom:10px;">
                        <p class="item-desc">Bold strawberry heat meets cool mint</p>
                        <div class="size-options">
                            <button class="size-btn active" data-item="red-flash" data-size="small" data-price="300">Small: 300/-</button>
                            <button class="size-btn" data-item="red-flash" data-size="medium" data-price="400">Medium: 400/-</button>
                            <button class="size-btn" data-item="red-flash" data-size="large" data-price="500">Large: 500/-</button>
                        </div>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="red-flash">-</button>
                                <span class="quantity" data-item="red-flash">0</span>
                                <button class="quantity-btn plus" data-item="red-flash">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="red-flash" data-price="300">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="menu-item">
                        <div class="item-header">
                            <span class="item-name">Berry Breeze</span>
                            <span class="item-price" id="price-berry-breeze">300/-</span>
                        </div>
                        <img src="https://i.postimg.cc/CRbeWzVVKVUVGNucA/berry-breeze.jpg" alt="Berry Breeze" style="width:100%; border-radius:8px; margin-bottom:10px;">
                        <p class="item-desc">Smooth berry chill, island style</p>
                        <div class="size-options">
                            <button class="size-btn active" data-item="berry-breeze" data-size="small" data-price="300">Small: 300/-</button>
                            <button class="size-btn" data-item="berry-breeze" data-size="medium" data-price="400">Medium: 400/-</button>
                            <button class="size-btn" data-item="berry-breeze" data-size="large" data-price="500">Large: 500/-</button>
                        </div>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="berry-breeze">-</button>
                                <span class="quantity" data-item="berry-breeze">0</span>
                                <button class="quantity-btn plus" data-item="berry-breeze">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="berry-breeze" data-price="300">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="menu-item">
                        <div class="item-header">
                            <span class="item-name">Ginger Gold</span>
                            <span class="item-price" id="price-ginger-gold">300/-</span>
                        </div>
                        <img src="https://i.postimg.cc/KpY6B92r4vuB9acD6/ginger-gold.jpg" alt="Ginger Gold" style="width:100%; border-radius:8px; margin-bottom:10px;">
                        <p class="item-desc">Golden spice with honeyed flow</p>
                        <div class="size-options">
                            <button class="size-btn active" data-item="ginger-gold" data-size="small" data-price="300">Small: 300/-</button>
                            <button class="size-btn" data-item="ginger-gold" data-size="medium" data-price="400">Medium: 400/-</button>
                            <button class="size-btn" data-item="ginger-gold" data-size="large" data-price="500">Large: 500/-</button>
                        </div>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="ginger-gold">-</button>
                                <span class="quantity" data-item="ginger-gold">0</span>
                                <button class="quantity-btn plus" data-item="ginger-gold">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="ginger-gold" data-price="300">Add to Cart</button>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Checkout Form -->
        <section class="checkout-form" id="checkout-form">
            <h3>Complete Your Order</h3>
            <div class="form-group">
                <label for="name">Full Name</label>
                <input type="text" id="name" required>
            </div>
            <div class="form-group">
                <label for="phone">Phone Number</label>
                <input type="tel" id="phone" required>
            </div>
            <div class="form-group">
                <label for="dressing">Dressing Description (Optional)</label>
                <textarea id="dressing" rows="3"></textarea>
            </div>
            <div class="form-group">
                <label for="location">Delivery Location</label>
                <input type="text" id="delivery-location" readonly>
                <small>If the location is not accurate, please describe your location below</small>
            </div>
            <div class="form-group">
                <label for="location-details">Location Details (If needed)</label>
                <textarea id="location-details" rows="2"></textarea>
            </div>
            
            <!-- Payment Information -->
            <div class="payment-info">
                <h4>Payment Method</h4>
                <p>We accept Lipa na M-Pesa</p>
                <p><strong>Paybill:</strong> 542542</p>
                <p><strong>Account Number:</strong> 786867</p>
                <p>Please complete payment before placing your order</p>
            </div>
            
            <button class="checkout-btn" id="place-order">Place Order via WhatsApp</button>
        </section>

        <!-- Floating Cart -->
        <div class="floating-cart" id="floating-cart">
            <div class="cart-header">
                <h3>Your Order</h3>
                <span id="cart-count">0 items</span>
            </div>
            <div class="cart-items" id="cart-items">
                <p style="text-align: center; padding: 20px;">Your cart is empty</p>
            </div>
            <div class="cart-total">
                <span>Total:</span>
                <span id="cart-total">0/-</span>
            </div>
            <button class="checkout-btn" id="checkout-btn">Proceed to Checkout</button>
        </div>

        <!-- Cart Toggle Button -->
        <div class="cart-toggle" id="cart-toggle">
            <i class="fas fa-shopping-cart"></i>
            <span class="cart-badge" id="cart-badge">0</span>
        </div>

        <!-- WhatsApp Chat -->
        <a href="https://wa.me/254115030726" class="whatsapp-chat" target="_blank">
            <i class="fab fa-whatsapp"></i>
        </a>
    </div>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-about">
                    <h3>About Laansales101</h3>
                    <p>Laansales101 was born from a deep understanding of the challenges that vendors and event-goers face. What if there was a way to merge convenience with luxury, to transform an ordinary event into an extraordinary experience? That vision led to the creation of Laansales101—a cutting-edge platform designed to make ordering seamless, effortless, and uniquely personal for every event-goer.</p>
                </div>
                <div class="footer-contact">
                    <h3>Contact Us</h3>
                    <p><i class="fas fa-envelope"></i> emflavorsales@gmail.com</p>
                    <p><i class="fas fa-phone"></i> +254 115 030 726</p>
                    <p><i class="fab fa-whatsapp"></i> WhatsApp: +254 115 030 726</p>
                </div>
            </div>
            <div class="footer-bottom">
                <p>&copy; 2025 Laansales101. All Rights Reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Initialize cart
        let cart = [];
        let userLocation = null;
        
        // DOM Elements
        const enableLocationBtn = document.getElementById('enableLocation');
        const locationStatus = document.getElementById('locationStatus');
        const checkoutBtn = document.getElementById('checkout-btn');
        const checkoutForm = document.getElementById('checkout-form');
        const placeOrderBtn = document.getElementById('place-order');
        const deliveryLocation = document.getElementById('delivery-location');
        const countdownEl = document.getElementById('countdown');
        const floatingCart = document.getElementById('floating-cart');
        const cartToggle = document.getElementById('cart-toggle');
        const cartBadge = document.getElementById('cart-badge');
        
        // Enable location
        enableLocationBtn.addEventListener('click', () => {
            if (navigator.geolocation) {
                navigator.geolocation.getCurrentPosition(
                    position => {
                        userLocation = position;
                        const { latitude, longitude } = position.coords;
                        locationStatus.innerHTML = `Location enabled! Latitude: ${latitude.toFixed(6)}, Longitude: ${longitude.toFixed(6)}`;
                        locationStatus.style.color = '#10b981';
                        deliveryLocation.value = `${latitude.toFixed(6)}, ${longitude.toFixed(6)}`;
                        
                        // Try to get address from coordinates
                        getAddressFromCoords(latitude, longitude);
                    },
                    error => {
                        locationStatus.innerHTML = 'Unable to retrieve location. Please describe your location in the checkout form.';
                        locationStatus.style.color = '#ef4444';
                        deliveryLocation.value = 'Location not available. Please describe below.';
                    }
                );
            } else {
                locationStatus.innerHTML = 'Geolocation is not supported by this browser. Please describe your location in the checkout form.';
                locationStatus.style.color = '#ef4444';
                deliveryLocation.value = 'Geolocation not supported. Please describe below.';
            }
        });
        
        // Function to get address from coordinates
        function getAddressFromCoords(lat, lng) {
            // Using Nominatim (OpenStreetMap) for reverse geocoding
            fetch(`https://nominatim.openstreetmap.org/reverse?format=json&lat=${lat}&lon=${lng}`)
                .then(response => response.json())
                .then(data => {
                    if (data && data.display_name) {
                        deliveryLocation.value = data.display_name;
                    }
                })
                .catch(error => {
                    console.error('Error getting address:', error);
                });
        }
        
        // Size selection for drinks
        document.querySelectorAll('.size-btn').forEach(button => {
            button.addEventListener('click', () => {
                const item = button.getAttribute('data-item');
                const size = button.getAttribute('data-size');
                const price = button.getAttribute('data-price');
                
                // Remove active class from all buttons in this group
                button.parentNode.querySelectorAll('.size-btn').forEach(btn => {
                    btn.classList.remove('active');
                });
                
                // Add active class to clicked button
                button.classList.add('active');
                
                // Update price display
                document.getElementById(`price-${item}`).textContent = `${price}/-`;
                
                // Update add to cart button data-price
                const addButton = button.closest('.menu-item').querySelector('.add-to-cart');
                addButton.setAttribute('data-price', price);
            });
        });
        
        // Quantity controls
        document.querySelectorAll('.quantity-btn').forEach(button => {
            button.addEventListener('click', () => {
                const item = button.getAttribute('data-item');
                const quantityEl = document.querySelector(`.quantity[data-item="${item}"]`);
                let quantity = parseInt(quantityEl.textContent);
                
                if (button.classList.contains('plus')) {
                    quantity++;
                } else if (button.classList.contains('minus') && quantity > 0) {
                    quantity--;
                }
                
                quantityEl.textContent = quantity;
            });
        });
        
        // Add to cart
        document.querySelectorAll('.add-to-cart').forEach(button => {
            button.addEventListener('click', () => {
                const item = button.getAttribute('data-item');
                const price = parseInt(button.getAttribute('data-price'));
                const quantity = parseInt(document.querySelector(`.quantity[data-item="${item}"]`).textContent);
                
                if (quantity === 0) return;
                
                // Get selected size for drinks
                let size = null;
                const sizeBtn = button.closest('.menu-item').querySelector('.size-btn.active');
                if (sizeBtn) {
                    size = sizeBtn.getAttribute('data-size');
                }
                
                // Check if item already in cart
                const existingItemIndex = cart.findIndex(cartItem => 
                    cartItem.name === item && cartItem.size === size
                );
                
                if (existingItemIndex !== -1) {
                    cart[existingItemIndex].quantity += quantity;
                } else {
                    cart.push({
                        name: item,
                        price: price,
                        quantity: quantity,
                        size: size
                    });
                }
                
                updateCart();
                
                // Reset quantity
                document.querySelector(`.quantity[data-item="${item}"]`).textContent = '0';
                
                // Show cart
                floatingCart.style.display = 'block';
            });
        });
        
        // Update cart
        function updateCart() {
            const cartItems = document.getElementById('cart-items');
            const cartCount = document.getElementById('cart-count');
            const cartTotal = document.getElementById('cart-total');
            
            // Clear cart items
            cartItems.innerHTML = '';
            
            if (cart.length === 0) {
                cartItems.innerHTML = '<p style="text-align: center; padding: 20px;">Your cart is empty</p>';
                cartCount.textContent = '0 items';
                cartTotal.textContent = '0/-';
                cartBadge.textContent = '0';
                return;
            }
            
            let total = 0;
            let itemCount = 0;
            
            cart.forEach((item, index) => {
                const itemTotal = item.price * item.quantity;
                total += itemTotal;
                itemCount += item.quantity;
                
                const cartItemEl = document.createElement('div');
                cartItemEl.className = 'cart-item';
                
                let sizeInfo = '';
                if (item.size) {
                    sizeInfo = ` (${item.size})`;
                }
                
                cartItemEl.innerHTML = `
                    <div class="cart-item-info">
                        <div>${formatItemName(item.name)}${sizeInfo}</div>
                        <div>${item.price}/- x ${item.quantity}</div>
                    </div>
                    <div class="cart-item-controls">
                        <span>${itemTotal}/-</span>
                        <button class="remove-btn" data-index="${index}">
                            <i class="fas fa-trash"></i>
                        </button>
                    </div>
                `;
                
                cartItems.appendChild(cartItemEl);
            });
            
            cartCount.textContent = `${itemCount} ${itemCount === 1 ? 'item' : 'items'}`;
            cartTotal.textContent = `${total}/-`;
            cartBadge.textContent = itemCount;
            
            // Add event listeners to remove buttons
            document.querySelectorAll('.remove-btn').forEach(button => {
                button.addEventListener('click', () => {
                    const index = parseInt(button.getAttribute('data-index'));
                    cart.splice(index, 1);
                    updateCart();
                });
            });
        }
        
        // Format item name for display
        function formatItemName(name) {
            return name.split('-')
                .map(word => word.charAt(0).toUpperCase() + word.slice(1))
                .join(' ');
        }
        
        // Toggle cart visibility
        cartToggle.addEventListener('click', () => {
            if (floatingCart.style.display === 'block') {
                floatingCart.style.display = 'none';
            } else {
                floatingCart.style.display = 'block';
            }
        });
        
        // Checkout button
        checkoutBtn.addEventListener('click', () => {
            if (cart.length === 0) {
                alert('Your cart is empty. Please add items before checkout.');
                return;
            }
            
            checkoutForm.style.display = 'block';
            checkoutForm.scrollIntoView({ behavior: 'smooth' });
        });
        
        // Place order
        placeOrderBtn.addEventListener('click', () => {
            const name = document.getElementById('name').value;
            const phone = document.getElementById('phone').value;
            
            if (!name || !phone) {
                alert('Please fill in all required fields.');
                return;
            }
            
            // Create order summary
            let orderSummary = `*NEW ORDER FROM EXQUISITE MADIWA FLAVORS WEBSITE*\n\n`;
            orderSummary += `*Customer Name:* ${name}\n`;
            orderSummary += `*Phone:* ${phone}\n`;
            
            // Add location information
            const locationDetails = document.getElementById('location-details').value;
            if (deliveryLocation.value && deliveryLocation.value !== 'Location not available. Please describe below.') {
                orderSummary += `*Location:* ${deliveryLocation.value}\n`;
            }
            if (locationDetails) {
                orderSummary += `*Location Details:* ${locationDetails}\n`;
            }
            
            orderSummary += `\n*Order Details:*\n`;
            
            cart.forEach(item => {
                let sizeInfo = '';
                if (item.size) {
                    sizeInfo = ` (${item.size})`;
                }
                orderSummary += `- ${formatItemName(item.name)}${sizeInfo} x ${item.quantity} = ${item.price * item.quantity}/-\n`;
            });
            
            orderSummary += `\n*Total: ${cart.reduce((total, item) => total + (item.price * item.quantity), 0)}/-*\n\n`;
            
            const dressing = document.getElementById('dressing').value;
            if (dressing) {
                orderSummary += `*Dressing Instructions:* ${dressing}\n`;
            }
            
            orderSummary += `\n*Payment Method:* Lipa na M-Pesa\n`;
            orderSummary += `*Paybill:* 542542\n`;
            orderSummary += `*Account Number:* 786867\n`;
            
            // Encode for WhatsApp URL
            const encodedMessage = encodeURIComponent(orderSummary);
            const whatsappURL = `https://wa.me/254115030726?text=${encodedMessage}`;
            
            // Open WhatsApp
            window.open(whatsappURL, '_blank');
            
            // Reset cart and form
            cart = [];
            updateCart();
            checkoutForm.style.display = 'none';
            document.getElementById('name').value = '';
            document.getElementById('phone').value = '';
            document.getElementById('dressing').value = '';
            document.getElementById('location-details').value = '';
            
            alert('Your order has been placed! You will be redirected to WhatsApp to confirm.');
        });
        
        // Countdown timer for special offer
        function updateCountdown() {
            const now = new Date();
            const minutes = now.getMinutes();
            const seconds = now.getSeconds();
            
            if (minutes < 20) {
                const timeLeft = 20 - minutes;
                const secsLeft = 60 - seconds;
                countdownEl.textContent = `Offer ends in: ${timeLeft} min ${secsLeft} sec`;
            } else {
                const nextHour = new Date(now);
                nextHour.setHours(nextHour.getHours() + 1);
                nextHour.setMinutes(0);
                nextHour.setSeconds(0);
                
                const diff = nextHour - now;
                const minsLeft = Math.floor(diff / 60000);
                const secsLeft = Math.floor((diff % 60000) / 1000);
                
                countdownEl.textContent = `Next offer in: ${minsLeft} min ${secsLeft} sec`;
            }
        }
        
        setInterval(updateCountdown, 1000);
        updateCountdown();
    </script>
</body>
</html>
