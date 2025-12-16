
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mindy Detailing | Professional Car Care in Queens, NY</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700&family=Open+Sans:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        :root {
            --primary: #1a365d;
            --secondary: #e6b325;
            --accent: #2d5aa0;
            --light: #f8f9fa;
            --dark: #212529;
            --gray: #6c757d;
            --success: #28a745;
        }
        
        body {
            font-family: 'Open Sans', sans-serif;
            line-height: 1.6;
            color: var(--dark);
            background-color: var(--light);
        }
        
        h1, h2, h3, h4, h5 {
            font-family: 'Montserrat', sans-serif;
            font-weight: 600;
            margin-bottom: 1rem;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header Styles */
        header {
            background-color: rgba(26, 54, 93, 0.95);
            position: fixed;
            width: 100%;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }
        
        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
        }
        
        .logo {
            color: white;
            font-size: 1.8rem;
            font-weight: 700;
            text-decoration: none;
            display: flex;
            align-items: center;
        }
        
        .logo i {
            color: var(--secondary);
            margin-right: 10px;
        }
        
        .nav-links {
            display: flex;
            list-style: none;
        }
        
        .nav-links li {
            margin-left: 30px;
        }
        
        .nav-links a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }
        
        .nav-links a:hover {
            color: var(--secondary);
        }
        
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
        }
        
        /* Hero Section */
        .hero {
            height: 100vh;
            background: linear-gradient(rgba(26, 54, 93, 0.8), rgba(26, 54, 93, 0.7)), url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQG1pJtoaM1-99koWi3WEvs_pqhbtARnmoRGO0fx5epww&s=10');
            background-size: cover;
            background-position: center;
            display: flex;
            align-items: center;
            color: white;
            text-align: center;
        }
        
        .hero-content {
            max-width: 800px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3);
        }
        
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
            opacity: 0.9;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--secondary);
            color: var(--primary);
            padding: 12px 30px;
            border-radius: 4px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s;
            border: none;
            cursor: pointer;
        }
        
        .btn:hover {
            background-color: white;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .btn-secondary {
            background-color: transparent;
            border: 2px solid white;
            color: white;
            margin-left: 15px;
        }
        
        .btn-secondary:hover {
            background-color: white;
            color: var(--primary);
        }
        
        /* Services Section */
        .section {
            padding: 80px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }
        
        .section-title h2 {
            font-size: 2.5rem;
            color: var(--primary);
            position: relative;
            display: inline-block;
            padding-bottom: 15px;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            width: 70px;
            height: 3px;
            background-color: var(--secondary);
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
            gap: 30px;
        }
        
        .service-card {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        
        .service-header {
            background-color: var(--primary);
            color: white;
            padding: 25px;
            text-align: center;
        }
        
        .service-price {
            font-size: 2rem;
            font-weight: 700;
            color: var(--secondary);
        }
        
        .service-price span {
            font-size: 1rem;
            font-weight: 400;
        }
        
        .service-body {
            padding: 25px;
        }
        
        .service-features h4 {
            color: var(--accent);
            margin-top: 20px;
            font-size: 1.1rem;
            border-bottom: 1px solid #eee;
            padding-bottom: 8px;
        }
        
        .service-features ul {
            list-style: none;
            margin-top: 10px;
        }
        
        .service-features li {
            padding: 8px 0;
            border-bottom: 1px dotted #eee;
            display: flex;
            align-items: center;
        }
        
        .service-features li i {
            color: var(--secondary);
            margin-right: 10px;
        }
        
        /* Gallery Section */
        .gallery-section {
            background-color: #f5f7fa;
        }
        
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }
        
        .gallery-item {
            position: relative;
            border-radius: 8px;
            overflow: hidden;
            height: 250px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }
        
        .gallery-item:hover img {
            transform: scale(1.05);
        }
        
        /* Before/After Section */
        .comparison-section {
            background-color: var(--primary);
            color: white;
        }
        
        .comparison-section .section-title h2 {
            color: white;
        }
        
        .comparison-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
            margin-top: 40px;
        }
        
        .comparison-item {
            text-align: center;
        }
        
        .comparison-img {
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
            height: 350px;
        }
        
        .comparison-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        .comparison-label {
            background-color: rgba(255, 255, 255, 0.1);
            padding: 10px;
            border-radius: 4px;
            margin-top: 15px;
            font-weight: 600;
            letter-spacing: 1px;
        }
        
        /* Booking Section */
        .booking-section {
            padding: 80px 0;
            background-color: white;
        }
        
        .booking-container {
            max-width: 800px;
            margin: 0 auto;
            background-color: #f8f9fa;
            border-radius: 10px;
            padding: 40px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
        }
        
        .booking-methods {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 30px;
            margin-top: 40px;
        }
        
        .booking-method {
            flex: 1;
            min-width: 250px;
            background-color: white;
            border-radius: 8px;
            padding: 30px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .booking-method i {
            font-size: 3rem;
            color: var(--primary);
            margin-bottom: 20px;
        }
        
        .booking-method h3 {
            color: var(--primary);
            margin-bottom: 15px;
        }
        
        .booking-note {
            margin-top: 30px;
            padding: 20px;
            background-color: rgba(230, 179, 37, 0.1);
            border-left: 4px solid var(--secondary);
            border-radius: 4px;
        }
        
        /* Contact Section */
        .contact-section {
            background-color: var(--primary);
            color: white;
        }
        
        .contact-info {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 40px;
            margin-top: 40px;
        }
        
        .contact-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
        }
        
        .contact-item i {
            font-size: 2.5rem;
            color: var(--secondary);
            margin-bottom: 15px;
        }
        
        /* Footer */
        footer {
            background-color: #0d1b36;
            color: #aaa;
            padding: 40px 0 20px;
            text-align: center;
        }
        
        .footer-content {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            margin-bottom: 30px;
        }
        
        .footer-column {
            flex: 1;
            min-width: 250px;
            margin-bottom: 30px;
        }
        
        .footer-column h3 {
            color: white;
            margin-bottom: 20px;
            font-size: 1.3rem;
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 20px;
        }
        
        .social-links a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            color: white;
            border-radius: 50%;
            text-decoration: none;
            transition: all 0.3s;
        }
        
        .social-links a:hover {
            background-color: var(--secondary);
            color: var(--primary);
        }
        
        .copyright {
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            padding-top: 20px;
            font-size: 0.9rem;
        }
        
        /* Responsive Styles */
        @media (max-width: 992px) {
            .hero h1 {
                font-size: 2.8rem;
            }
            
            .comparison-container {
                grid-template-columns: 1fr;
            }
        }
        
        @media (max-width: 768px) {
            .mobile-menu-btn {
                display: block;
            }
            
            .nav-links {
                position: fixed;
                top: 70px;
                left: 0;
                width: 100%;
                background-color: var(--primary);
                flex-direction: column;
                align-items: center;
                padding: 20px 0;
                transform: translateY(-100%);
                opacity: 0;
                transition: all 0.3s;
                box-shadow: 0 5px 10px rgba(0, 0, 0, 0.1);
            }
            
            .nav-links.active {
                transform: translateY(0);
                opacity: 1;
            }
            
            .nav-links li {
                margin: 15px 0;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .hero p {
                font-size: 1rem;
            }
            
            .section {
                padding: 60px 0;
            }
            
            .section-title h2 {
                font-size: 2rem;
            }
        }
        
        @media (max-width: 576px) {
            .hero h1 {
                font-size: 1.8rem;
            }
            
            .btn {
                padding: 10px 20px;
                font-size: 0.9rem;
            }
            
            .service-card {
                min-width: 100%;
            }
            
            .booking-container {
                padding: 30px 20px;
            }
        }
    </style>
</head>
<body>
    <!-- Header & Navigation -->
    <header>
        <div class="container nav-container">
            <a href="#" class="logo">
                <i class="fas fa-car"></i> Mindy Detailing
            </a>
            
            <button class="mobile-menu-btn" id="mobileMenuBtn">
                <i class="fas fa-bars"></i>
            </button>
            
            <ul class="nav-links" id="navLinks">
                <li><a href="#home">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#gallery">Gallery</a></li>
                <li><a href="#booking">Booking</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="hero-content">
            <h1>Professional Car Detailing in Queens, NY</h1>
            <p>We bring back the shine to your vehicle with premium detailing services, ceramic coatings, and expert installations. Experience the Mindy difference.</p>
            <div>
                <a href="#services" class="btn">View Services</a>
                <a href="#booking" class="btn btn-secondary">Book Now</a>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="section" id="services">
        <div class="container">
            <div class="section-title">
                <h2>Our Detailing Packages</h2>
                <p>Choose from our range of professional detailing services</p>
            </div>
            
            <div class="services-grid">
                <!-- Basic Package -->
                <div class="service-card">
                    <div class="service-header">
                        <h3>Mindy BASIC</h3>
                        <div class="service-price">$39.99</div>
                    </div>
                    <div class="service-body">
                        <div class="service-features">
                            <h4><i class="fas fa-spray-can"></i> Exterior</h4>
                            <ul>
                                <li><i class="fas fa-check"></i> Two-stage foam wash</li>
                                <li><i class="fas fa-check"></i> Gentle hand wash</li>
                                <li><i class="fas fa-check"></i> Finished with a 2-week wax</li>
                                <li><i class="fas fa-check"></i> Tire Shine</li>
                            </ul>
                            
                            <h4><i class="fas fa-vacuum"></i> Interior</h4>
                            <ul>
                                <li><i class="fas fa-check"></i> Wipe down vacuum</li>
                                <li><i class="fas fa-check"></i> Floor mats rinsed</li>
                            </ul>
                        </div>
                    </div>
                </div>
                
                <!-- Interior Plus Package -->
                <div class="service-card">
                    <div class="service-header">
                        <h3>Mindy Interior PLUS</h3>
                        <div class="service-price">$119.99<span>+*</span></div>
                    </div>
                    <div class="service-body">
                        <div class="service-features">
                            <h4><i class="fas fa-spray-can"></i> Exterior</h4>
                            <ul>
                                <li><i class="fas fa-check"></i> Two-stage foam wash</li>
                                <li><i class="fas fa-check"></i> Gentle hand wash</li>
                                <li><i class="fas fa-check"></i> Finished with a 2-week wax</li>
                                <li><i class="fas fa-check"></i> Tire Shine</li>
                            </ul>
                            
                            <h4><i class="fas fa-vacuum"></i> Interior</h4>
                            <ul>
                                <li><i class="fas fa-check"></i> Steam bath</li>
                                <li><i class="fas fa-check"></i> Plastic and vinyl protection</li>
                                <li><i class="fas fa-check"></i> Seat extraction</li>
                                <li><i class="fas fa-check"></i> Carpet Vacuumed</li>
                                <li><i class="fas fa-check"></i> Leather Conditioner</li>
                                <li><i class="fas fa-check"></i> Floor mats shampooed</li>
                            </ul>
                        </div>
                    </div>
                </div>
                
                <!-- Ceramic Deluxe Package -->
                <div class="service-card">
                    <div class="service-header">
                        <h3>Mindy Ceramic DELUXE</h3>
                        <div class="service-price">$219.99<span>+*</span></div>
                    </div>
                    <div class="service-body">
                        <div class="service-features">
                            <h4><i class="fas fa-spray-can"></i> Exterior</h4>
                            <ul>
                                <li><i class="fas fa-check"></i> Two-stage foam wash</li>
                                <li><i class="fas fa-check"></i> Iron remover</li>
                                <li><i class="fas fa-check"></i> Clay Bar</li>
                                <li><i class="fas fa-check"></i> Ceramic sealant (3-6 months protection)</li>
                                <li><i class="fas fa-check"></i> Tire Shine</li>
                            </ul>
                            
                            <h4><i class="fas fa-vacuum"></i> Interior</h4>
                            <ul>
                                <li><i class="fas fa-check"></i> Steam bath</li>
                                <li><i class="fas fa-check"></i> Plastic and vinyl protection</li>
                                <li><i class="fas fa-check"></i> Seat extraction</li>
                                <li><i class="fas fa-check"></i> Carpet Vacuumed</li>
                                <li><i class="fas fa-check"></i> Leather Conditioner</li>
                                <li><i class="fas fa-check"></i> Floor mats shampooed</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="booking-note">
                <p><strong>*Note:</strong> For an accurate quote please send pictures of your vehicle to (347)-776-3706</p>
            </div>
        </div>
    </section>

    <!-- Gallery Section -->
    <section class="section gallery-section" id="gallery">
        <div class="container">
            <div class="section-title">
                <h2>Our Work Gallery</h2>
                <p>See the transformation we deliver for every vehicle</p>
            </div>
            
            <div class="gallery-grid">
                <div class="gallery-item">
                    <img src="https://www.dropbox.com/scl/fi/17fqtayvetr97rfy3xloa/IMG_7378.jpeg?rlkey=5m3pm4tvsn1d84uj4v7ll88fn&st=fqanapjp&dl=1" alt="Car Detailing Work">
                </div>
                <div class="gallery-item">
                    <img src="https://www.dropbox.com/scl/fi/cabnrafwcend5tjfzyiuo/IMG_7377.jpeg?rlkey=m1ry0jzf1xobet11z2jm75pvk&st=aoiyzflu&dl=1" alt="Car Detailing Work">
                </div>
                <div class="gallery-item">
                    <img src="https://www.dropbox.com/scl/fi/nsf9we9t74y6ao59chnne/IMG_7376.jpeg?rlkey=r60cmj7pxx2by8uw95ojhl7ko&st=1yp9a52r&dl=1" alt="Car Detailing Work">
                </div>
                <div class="gallery-item">
                    <img src="https://www.dropbox.com/scl/fi/8qio8vl30m2ll9evr3lx1/IMG_7375.jpeg?rlkey=v4k1r2k24t0sdpazyz3kz25hd&st=137p6uk7&dl=1" alt="Car Detailing Work">
                </div>
                <div class="gallery-item">
                    <img src="https://www.dropbox.com/scl/fi/rx9jh5s9bmxbbpvv9ildr/IMG_7374.jpeg?rlkey=7a36rdwbqk4gpo1vcwnh45olf&st=ry0x4hnt&dl=1" alt="Car Detailing Work">
                </div>
            </div>
        </div>
    </section>

    <!-- Before/After Section -->
    <section class="section comparison-section">
        <div class="container">
            <div class="section-title">
                <h2>Before & After</h2>
                <p>See the dramatic transformation we achieve</p>
            </div>
            
            <div class="comparison-container">
                <div class="comparison-item">
                    <div class="comparison-img">
                        <img src="https://www.dropbox.com/scl/fi/pi1pnia6mcid371srnsv7/IMG_7379.jpeg?rlkey=oa48c9zku033c2wi526o6nnp7&st=czx6n7a6&dl=1" alt="Before Detailing">
                    </div>
                    <div class="comparison-label">BEFORE</div>
                </div>
                
                <div class="comparison-item">
                    <div class="comparison-img">
                        <img src="https://www.dropbox.com/scl/fi/epbjaycawpoyl0uvu8j1a/IMG_7380.jpeg?rlkey=1s9kku86hxpknho0mi3nsk0pk&st=i3lw0web&dl=1" alt="After Detailing">
                    </div>
                    <div class="comparison-label">AFTER</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Additional Services -->
    <section class="section">
        <div class="container">
            <div class="section-title">
                <h2>Additional Services</h2>
                <p>Beyond detailing, we offer premium automotive services</p>
            </div>
            
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-header">
                        <h3>Ceramic Coatings</h3>
                    </div>
                    <div class="service-body">
                        <p>Premium ceramic coatings that provide long-lasting protection against environmental contaminants, UV rays, and minor scratches.</p>
                        <ul class="service-features" style="margin-top: 20px;">
                            <li><i class="fas fa-check"></i> Professional-grade ceramic formulas</li>
                            <li><i class="fas fa-check"></i> Up to 5 years of protection</li>
                            <li><i class="fas fa-check"></i> Enhanced gloss and hydrophobic properties</li>
                        </ul>
                    </div>
                </div>
                
                <div class="service-card">
                    <div class="service-header">
                        <h3>OEM+ Ambient Lighting</h3>
                    </div>
                    <div class="service-body">
                        <p>Custom ambient lighting installations that enhance your vehicle's interior with factory-like quality and customization options.</p>
                        <ul class="service-features" style="margin-top: 20px;">
                            <li><i class="fas fa-check"></i> Professional installation</li>
                            <li><i class="fas fa-check"></i> Color customization</li>
                            <li><i class="fas fa-check"></i> Wireless control options</li>
                        </ul>
                    </div>
                </div>
                
                <div class="service-card">
                    <div class="service-header">
                        <h3>Dash Cam & Headlight Restoration</h3>
                    </div>
                    <div class="service-body">
                        <p>Professional dash cam installations and headlight restoration services to keep you safe and your vehicle looking its best.</p>
                        <ul class="service-features" style="margin-top: 20px;">
                            <li><i class="fas fa-check"></i> Dash cam installation</li>
                            <li><i class="fas fa-check"></i> Headlight restoration</li>
                            <li><i class="fas fa-check"></i> Professional wiring and setup</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Booking Section -->
    <section class="section booking-section" id="booking">
        <div class="container">
            <div class="section-title">
                <h2>Book Your Appointment</h2>
                <p>Schedule your detailing service today</p>
            </div>
            
            <div class="booking-container">
                <div class="booking-methods">
                    <div class="booking-method">
                        <i class="fas fa-qrcode"></i>
                        <h3>Scan to Book</h3>
                        <p>Use your phone's camera to scan the QR code and book your appointment directly.</p>
                        <div style="margin-top: 20px; background-color: #f1f1f1; padding: 15px; border-radius: 8px;">
                            <p><strong>Scan QR Code</strong></p>
                            <p style="font-size: 0.9rem; color: var(--gray);">Point your camera at the QR code from our flyer</p>
                        </div>
                    </div>
                    
                    <div class="booking-method">
                        <i class="fas fa-phone-alt"></i>
                        <h3>Call or Text</h3>
                        <p>Contact us directly to schedule your appointment or get a quote.</p>
                        <div style="margin-top: 20px; background-color: #f1f1f1; padding: 15px; border-radius: 8px;">
                            <p><strong>(347)-776-3706</strong></p>
                            <p style="font-size: 0.9rem; color: var(--gray);">Call or text for booking and quotes</p>
                        </div>
                    </div>
                </div>
                
                <div class="booking-note">
                    <p><strong>For an accurate quote:</strong> Please send pictures of your vehicle to the number above. We'll provide you with a personalized estimate based on your vehicle's condition and size.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="section contact-section" id="contact">
        <div class="container">
            <div class="section-title">
                <h2>Contact Us</h2>
                <p>Get in touch with Mindy Detailing</p>
            </div>
            
            <div class="contact-info">
                <div class="contact-item">
                    <i class="fas fa-map-marker-alt"></i>
                    <h3>Location</h3>
                    <p>Queens, New York</p>
                </div>
                
                <div class="contact-item">
                    <i class="fas fa-phone-alt"></i>
                    <h3>Phone</h3>
                    <p>(347)-776-3706</p>
                </div>
                
                <div class="contact-item">
                    <i class="fas fa-envelope"></i>
                    <h3>DM for Services</h3>
                    <p>Message us on Instagram for inquiries</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Mindy Detailing</h3>
                    <p>Professional auto detailing services in Queens, NY. Bringing back the shine to your vehicle with premium care and attention to detail.</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                    </div>
                </div>
                
                <div class="footer-column">
                    <h3>Services</h3>
                    <ul style="list-style: none;">
                        <li><a href="#services" style="color: #aaa; text-decoration: none;">Detailing Packages</a></li>
                        <li><a href="#services" style="color: #aaa; text-decoration: none;">Ceramic Coatings</a></li>
                        <li><a href="#services" style="color: #aaa; text-decoration: none;">Lighting Installation</a></li>
                        <li><a href="#services" style="color: #aaa; text-decoration: none;">Headlight Restoration</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Quick Links</h3>
                    <ul style="list-style: none;">
                        <li><a href="#home" style="color: #aaa; text-decoration: none;">Home</a></li>
                        <li><a href="#services" style="color: #aaa; text-decoration: none;">Services</a></li>
                        <li><a href="#gallery" style="color: #aaa; text-decoration: none;">Gallery</a></li>
                        <li><a href="#booking" style="color: #aaa; text-decoration: none;">Booking</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2023 Mindy Detailing. All rights reserved. | Queens, NY</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile Menu Toggle
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const navLinks = document.getElementById('navLinks');
        
        mobileMenuBtn.addEventListener('click', () => {
            navLinks.classList.toggle('active');
            mobileMenuBtn.innerHTML = navLinks.classList.contains('active') 
                ? '<i class="fas fa-times"></i>' 
                : '<i class="fas fa-bars"></i>';
        });
        
        // Close mobile menu when clicking a link
        document.querySelectorAll('.nav-links a').forEach(link => {
            link.addEventListener('click', () => {
                navLinks.classList.remove('active');
                mobileMenuBtn.innerHTML = '<i class="fas fa-bars"></i>';
            });
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if(targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if(targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 70,
                        behavior: 'smooth'
                    });
                }
            });
        });
        
        // Add active class to nav links on scroll
        window.addEventListener('scroll', () => {
            const sections = document.querySelectorAll('section');
            const navLinks = document.querySelectorAll('.nav-links a');
            
            let current = '';
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;
                if(pageYOffset >= sectionTop - 100) {
                    current = section.getAttribute('id');
                }
            });
            
            navLinks.forEach(link => {
                link.classList.remove('active');
                if(link.getAttribute('href') === `#${current}`) {
                    link.classList.add('active');
                }
            });
        });
    </script>
</body>
</html>
