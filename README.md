<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kashyap Digital Service Point - Bhoja, Begusarai</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #f5f5f5;
            color: #333;
        }
        
        /* Header */
        .header {
            background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
            color: white;
            padding: 20px 0;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .header-content {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }
        
        .logo h1 {
            font-size: 1.8em;
            margin-bottom: 5px;
        }
        
        .logo p {
            font-size: 0.9em;
            opacity: 0.9;
        }
        
        .contact-quick {
            text-align: right;
        }
        
        .contact-quick a {
            color: white;
            text-decoration: none;
            font-size: 1.3em;
            font-weight: bold;
            display: block;
            margin-bottom: 5px;
        }
        
        .contact-quick small {
            opacity: 0.9;
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 60px 20px;
            text-align: center;
        }
        
        .hero h2 {
            font-size: 2.5em;
            margin-bottom: 20px;
            animation: fadeInUp 1s;
        }
        
        .hero p {
            font-size: 1.3em;
            margin-bottom: 30px;
            opacity: 0.95;
        }
        
        .cta-buttons {
            display: flex;
            gap: 20px;
            justify-content: center;
            flex-wrap: wrap;
        }
        
        .btn {
            padding: 15px 35px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            font-size: 1.1em;
            transition: all 0.3s;
            display: inline-block;
        }
        
        .btn-primary {
            background: white;
            color: #667eea;
        }
        
        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
        }
        
        .btn-secondary {
            background: transparent;
            color: white;
            border: 2px solid white;
        }
        
        .btn-secondary:hover {
            background: white;
            color: #667eea;
        }
        
        /* Services Section */
        .services {
            max-width: 1200px;
            margin: 60px auto;
            padding: 0 20px;
        }
        
        .section-title {
            text-align: center;
            font-size: 2.5em;
            color: #1e3c72;
            margin-bottom: 50px;
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
        }
        
        .service-card {
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            text-align: center;
            transition: all 0.3s;
        }
        
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 40px rgba(0,0,0,0.2);
        }
        
        .service-icon {
            font-size: 3em;
            margin-bottom: 15px;
        }
        
        .service-card h3 {
            color: #1e3c72;
            margin-bottom: 10px;
            font-size: 1.4em;
        }
        
        .service-card p {
            color: #666;
            line-height: 1.6;
        }
        
        /* Why Choose Us */
        .why-us {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 60px 20px;
            margin: 60px 0;
        }
        
        .why-us-content {
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .feature {
            text-align: center;
            padding: 20px;
        }
        
        .feature-icon {
            font-size: 2.5em;
            margin-bottom: 15px;
        }
        
        .feature h4 {
            font-size: 1.3em;
            margin-bottom: 10px;
        }
        
        /* Location Section */
        .location {
            max-width: 1200px;
            margin: 60px auto;
            padding: 0 20px;
        }
        
        .location-content {
            background: white;
            padding: 40px;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
        }
        
        .location-info h3 {
            color: #1e3c72;
            font-size: 1.8em;
            margin-bottom: 20px;
        }
        
        .info-item {
            margin: 15px 0;
            display: flex;
            align-items: center;
            gap: 15px;
        }
        
        .info-icon {
            font-size: 1.5em;
            color: #667eea;
        }
        
        .info-text {
            line-height: 1.6;
        }
        
        .info-text strong {
            display: block;
            color: #1e3c72;
            margin-bottom: 5px;
        }
        
        /* Footer */
        .footer {
            background: #1e3c72;
            color: white;
            padding: 40px 20px;
            text-align: center;
        }
        
        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .social-links {
            margin: 20px 0;
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }
        
        .social-btn {
            background: white;
            color: #1e3c72;
            padding: 10px 25px;
            border-radius: 25px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s;
        }
        
        .social-btn:hover {
            transform: scale(1.1);
            box-shadow: 0 5px 15px rgba(255,255,255,0.3);
        }
        
        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .header-content {
                text-align: center;
            }
            
            .contact-quick {
                text-align: center;
                margin-top: 15px;
            }
            
            .hero h2 {
                font-size: 2em;
            }
            
            .section-title {
                font-size: 2em;
            }
            
            .cta-buttons {
                flex-direction: column;
                align-items: center;
            }
        }
        
        /* Floating WhatsApp Button */
        .whatsapp-float {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background: #25D366;
            color: white;
            border-radius: 50%;
            width: 60px;
            height: 60px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2em;
            box-shadow: 0 5px 20px rgba(37, 211, 102, 0.5);
            cursor: pointer;
            transition: all 0.3s;
            z-index: 1000;
            animation: pulse 2s infinite;
        }
        
        .whatsapp-float:hover {
            transform: scale(1.1);
        }
        
        @keyframes pulse {
            0%, 100% {
                box-shadow: 0 5px 20px rgba(37, 211, 102, 0.5);
            }
            50% {
                box-shadow: 0 5px 30px rgba(37, 211, 102, 0.8);
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="header-content">
            <div class="logo">
                <h1>🏪 Kashyap Digital Service Point</h1>
                <p>आपका विश्वसनीय डिजिटल साथी</p>
            </div>
            <div class="contact-quick">
                <a href="tel:06243222300">📞 06243-222300</a>
                <small>Bhoja, Chhaurahi, Begusarai</small>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <h2>सभी डिजिटल सेवाएं एक छत के नीचे</h2>
        <p>आधार, पैन कार्ड, प्रिंटिंग, रिचार्ज और भी बहुत कुछ!</p>
        <div class="cta-buttons">
            <a href="tel:06243222300" class="btn btn-primary">📞 अभी कॉल करें</a>
            <a href="https://wa.me/916243222300" class="btn btn-secondary">💬 WhatsApp करें</a>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services">
        <h2 class="section-title">हमारी सेवाएं</h2>
        <div class="services-grid">
            <div class="service-card">
                <div class="service-icon">🆔</div>
                <h3>आधार कार्ड सेवाएं</h3>
                <p>नया आधार, अपडेट, प्रिंट - सभी आधार संबंधित सेवाएं तुरंत उपलब्ध</p>
            </div>
            
            <div class="service-card">
                <div class="service-icon">💳</div>
                <h3>PAN Card सेवाएं</h3>
                <p>नया पैन कार्ड, करेक्शन, रीप्रिंट - सभी सेवाएं उपलब्ध</p>
            </div>
            
            <div class="service-card">
                <div class="service-icon">🖨️</div>
                <h3>प्रिंटिंग सर्विसेज</h3>
                <p>Printing, Xerox, Scanning, Lamination - Best Quality, Low Price</p>
            </div>
            
            <div class="service-card">
                <div class="service-icon">📱</div>
                <h3>रिचार्ज & बिल पेमेंट</h3>
                <p>Mobile Recharge, DTH, Bill Payment - सभी ऑपरेटर्स उपलब्ध</p>
            </div>
            
            <div class="service-card">
                <div class="service-icon">💻</div>
                <h3>Computer Services</h3>
                <p>Computer/Laptop Repair, Data Recovery, Software Installation</p>
            </div>
            
            <div class="service-card">
                <div class="service-icon">📄</div>
                <h3>Online Form Filling</h3>
                <p>सभी प्रकार के Online Forms, Applications, Registrations</p>
            </div>
            
            <div class="service-card">
                <div class="service-icon">🏦</div>
                <h3>Banking Services</h3>
                <p>CSC Banking, Money Transfer, Account Opening Support</p>
            </div>
            
            <div class="service-card">
                <div class="service-icon">📸</div>
                <h3>Photo Services</h3>
                <p>Passport Photo, Photo Print, Photo Editing - Quick Service</p>
            </div>
        </div>
    </section>

    <!-- Why Choose Us -->
    <section class="why-us">
        <div class="why-us-content">
            <h2 class="section-title" style="color: white;">हमें क्यों चुनें?</h2>
            <div class="features-grid">
                <div class="feature">
                    <div class="feature-icon">⚡</div>
                    <h4>तेज़ सेवा</h4>
                    <p>ज्यादातर सेवाएं 30 मिनट में पूरी</p>
                </div>
                
                <div class="feature">
                    <div class="feature-icon">💰</div>
                    <h4>उचित दाम</h4>
                    <p>सस्ती और पारदर्शी कीमतें</p>
                </div>
                
                <div class="feature">
                    <div class="feature-icon">🤝</div>
                    <h4>विश्वसनीय</h4>
                    <p>सालों का अनुभव और हजारों खुश ग्राहक</p>
                </div>
                
                <div class="feature">
                    <div class="feature-icon">👨‍💼</div>
                    <h4>Professional Team</h4>
                    <p>अनुभवी और trained स्टाफ</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Location Section -->
    <section class="location">
        <h2 class="section-title">हमसे संपर्क करें</h2>
        <div class="location-content">
            <div class="location-info">
                <h3>📍 हमारा पता</h3>
                <div class="info-item">
                    <div class="info-icon">📍</div>
                    <div class="info-text">
                        <strong>Location:</strong>
                        Kashyap Digital Service Point<br>
                        Bhoja, Chhaurahi<br>
                        Begusarai, Bihar
                    </div>
                </div>
                
                <div class="info-item">
                    <div class="info-icon">📞</div>
                    <div class="info-text">
                        <strong>Phone:</strong>
                        <a href="tel:06243222300" style="color: #667eea; text-decoration: none;">06243-222300</a>
                    </div>
                </div>
                
                <div class="info-item">
                    <div class="info-icon">⏰</div>
                    <div class="info-text">
                        <strong>Timing:</strong>
                        सुबह 9:00 AM - रात 9:00 PM<br>
                        <small>(7 दिन खुला रहता है)</small>
                    </div>
                </div>
                
                <div class="info-item">
                    <div class="info-icon">💬</div>
                    <div class="info-text">
                        <strong>WhatsApp:</strong>
                        <a href="https://wa.me/916243222300" style="color: #25D366; text-decoration: none;">Message us on WhatsApp</a>
                    </div>
                </div>
            </div>
            
            <div class="location-map">
                <h3>🗺️ हम यहां हैं</h3>
                <p style="margin: 20px 0; line-height: 1.8;">
                    <strong>Landmark:</strong> Chhaurahi के पास<br>
                    <strong>District:</strong> Begusarai, Bihar<br><br>
                    
                    <strong>कैसे पहुंचें:</strong><br>
                    • Bhoja Chhaurahi से सिर्फ 2 मिनट<br>
                    • Main Road पर स्थित<br>
                    • आसानी से दिखने वाली दुकान
                </p>
                <a href="https://www.google.com/maps/search/Bhoja+Chhaurahi+Begusarai" 
                   target="_blank" 
                   class="btn btn-primary" 
                   style="display: inline-block; margin-top: 20px;">
                    📍 Google Maps पर देखें
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="footer-content">
            <h3>🏪 Kashyap Digital Service Point</h3>
            <p style="margin: 15px 0;">आपका विश्वसनीय डिजिटल साथी | Bhoja, Begusarai</p>
            
            <div class="social-links">
                <a href="tel:06243222300" class="social-btn">📞 Call Now</a>
                <a href="https://wa.me/916243222300" class="social-btn">💬 WhatsApp</a>
            </div>
            
            <p style="margin-top: 30px; opacity: 0.8; font-size: 0.9em;">
                © 2025 Kashyap Digital Service Point. All Rights Reserved.<br>
                Made with ❤️ by Claude AI
            </p>
        </div>
    </footer>

    <!-- Floating WhatsApp Button -->
    <a href="https://wa.me/916243222300" class="whatsapp-float" target="_blank" title="WhatsApp पर संपर्क करें">
        💬
    </a>

    <script>
        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth' });
                }
            });
        });

        // Service cards animation on scroll
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -100px 0px'
        };

        const observer = new IntersectionObserver(function(entries) {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.animation = 'fadeInUp 0.6s ease-out';
                }
            });
        }, observerOptions);

        document.querySelectorAll('.service-card').forEach(card => {
            observer.observe(card);
        });

        // Click tracking (for analytics - optional)
        document.querySelectorAll('a[href^="tel:"], a[href^="https://wa.me"]').forEach(link => {
            link.addEventListener('click', function() {
                console.log('Contact initiated:', this.href);
            });
        });
    </script>
</body>
</html>
