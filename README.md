<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="LUNIX - Premium brown themed clothing brand">
    <meta name="keywords" content="clothing, fashion, LUNIX, premium wear">
    <title>LUNIX - Premium Clothing</title>
    <!-- Save this file as index.html -->
    <link rel="icon" type="image/png" href="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/149e6b94-caac-42ee-820d-9f392280607c.png">
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Poppins:wght@300;400;500&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-brown: #5c4d3c;
            --secondary-brown: #7a6a57;
            --light-brown: #d2c7b8;
            --dark-brown: #3a3225;
            --accent-gold: #c2a578;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            color: white;
            background-color: var(--dark-brown);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        header {
            background-color: var(--primary-brown);
            padding: 20px 0;
            position: sticky;
            top: 0;
            z-index: 100;
            border-bottom: 1px solid var(--accent-gold);
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 2rem;
            color: var(--light-brown);
            text-decoration: none;
            letter-spacing: 2px;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 30px;
        }
        
        nav ul li a {
            color: var(--light-brown);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: var(--accent-gold);
        }
        
        .hero {
            height: 90vh;
            background-image: linear-gradient(rgba(58, 50, 37, 0.7), rgba(58, 50, 37, 0.7)), url('https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/3ba5c335-709f-4123-a03f-c90b084f2021.png');
            background-size: cover;
            background-position: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
            padding: 0 20px;
        }
        
        .hero h1 {
            font-family: 'Playfair Display', serif;
            font-size: 4rem;
            margin-bottom: 20px;
            color: var(--light-brown);
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin-bottom: 30px;
            color: var(--light-brown);
        }
        
        .btn {
            display: inline-block;
            background-color: var(--accent-gold);
            color: var(--dark-brown);
            padding: 12px 30px;
            text-decoration: none;
            font-weight: 500;
            border-radius: 25px;
            transition: all 0.3s;
        }
        
        .btn:hover {
            background-color: var(--light-brown);
            transform: translateY(-3px);
        }
        
        .section-title {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            text-align: center;
            margin: 60px 0 40px;
            color: var(--light-brown);
        }
        
        .collection {
            padding: 60px 0;
            background-color: var(--primary-brown);
        }
        
        .collection-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }
        
        .collection-item {
            background-color: var(--secondary-brown);
            border-radius: 8px;
            overflow: hidden;
            transition: transform 0.3s;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .collection-item:hover {
            transform: translateY(-10px);
        }
        
        .collection-item img {
            width: 100%;
            height: 300px;
            object-fit: cover;
        }
        
        .collection-info {
            padding: 20px;
        }
        
        .collection-info h3 {
            font-size: 1.3rem;
            margin-bottom: 10px;
            color: white;
        }
        
        .collection-info p {
            color: var(--light-brown);
            margin-bottom: 15px;
        }
        
        .collection-info .price {
            font-weight: 500;
            color: var(--accent-gold);
            font-size: 1.2rem;
        }
        
        .about {
            padding: 80px 0;
            background-color: var(--secondary-brown);
        }
        
        .about-content {
            display: flex;
            align-items: center;
            gap: 50px;
        }
        
        .about-text {
            flex: 1;
        }
        
        .about-text h2 {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            margin-bottom: 25px;
            color: var(--light-brown);
        }
        
        .about-text p {
            margin-bottom: 20px;
            color: white;
        }
        
        .about-image {
            flex: 1;
        }
        
        .about-image img {
            width: 100%;
            border-radius: 8px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }
        
        .testimonials {
            padding: 80px 0;
            background-color: var(--primary-brown);
        }
        
        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .testimonial-card {
            background-color: var(--secondary-brown);
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .testimonial-card p {
            font-style: italic;
            margin-bottom: 20px;
            color: white;
        }
        
        .testimonial-author {
            display: flex;
            align-items: center;
        }
        
        .testimonial-author img {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            margin-right: 15px;
            object-fit: cover;
        }
        
        .author-info h4 {
            color: var(--accent-gold);
            margin-bottom: 5px;
        }
        
        .author-info p {
            font-style: normal;
            font-size: 0.9rem;
            color: var(--light-brown);
        }
        
        footer {
            background-color: var(--dark-brown);
            padding: 50px 0 20px;
            text-align: center;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }
        
        .footer-column h3 {
            font-family: 'Playfair Display', serif;
            font-size: 1.5rem;
            margin-bottom: 20px;
            color: var(--accent-gold);
        }
        
        .footer-column ul {
            list-style: none;
        }
        
        .footer-column ul li {
            margin-bottom: 10px;
        }
        
        .footer-column ul li a {
            color: var(--light-brown);
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-column ul li a:hover {
            color: var(--accent-gold);
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 30px;
        }
        
        .social-links a {
            color: var(--light-brown);
            font-size: 1.5rem;
            transition: color 0.3s;
        }
        
        .social-links a:hover {
            color: var(--accent-gold);
        }
        
        .copyright {
            color: var(--light-brown);
            font-size: 0.9rem;
            padding-top: 20px;
            border-top: 1px solid var(--secondary-brown);
        }
        
        @media (max-width: 768px) {
            .header-container {
                flex-direction: column;
            }
            
            nav ul {
                margin-top: 20px;
            }
            
            nav ul li {
                margin-left: 15px;
                margin-right: 15px;
            }
            
            .hero h1 {
                font-size: 3rem;
            }
            
            .about-content {
                flex-direction: column;
            }
            
            .about-image {
                margin-top: 30px;
            }
        }
        
        @media (max-width: 480px) {
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .hero p {
                font-size: 1rem;
            }
            
            .section-title {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container header-container">
            <a href="#" class="logo">LUNIX</a>
            <nav>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#collection">Collection</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#testimonials">Testimonials</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>
    
    <section class="hero" id="home">
        <h1>Elevate Your Style</h1>
        <p>Discover timeless elegance with LUNIX's premium clothing collection. Crafted for comfort, designed for sophistication.</p>
        <a href="#collection" class="btn">Explore Collection</a>
    </section>
    
    <section class="collection" id="collection">
        <div class="container">
            <h2 class="section-title">Featured Collection</h2>
            <div class="collection-grid">
                <div class="collection-item">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/debe2e0e-ac79-45f5-bd55-77dd697bd164.png" alt="Brown leather jacket with modern minimalist design and premium stitching details">
                    <div class="collection-info">
                        <h3>Premium Jacket</h3>
                        <p>Crafted from finest Italian leather</p>
                        <p class="price">₹24,999</p>
                        <a href="#" class="btn">Add to Cart</a>
                    </div>
                </div>
                <div class="collection-item">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/3a907818-fbb1-4529-b8d6-6fc779195a24.png" alt="Warm brown cashmere sweater with elegant knit pattern and luxurious texture">
                    <div class="collection-info">
                        <h3>Cashmere Sweater</h3>
                        <p>100% Mongolian cashmere</p>
                        <p class="price">₹15,799</p>
                        <a href="#" class="btn">Add to Cart</a>
                    </div>
                </div>
                <div class="collection-item">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/685ac76c-4bb5-4850-be11-4938654d3776.png" alt="Classic brown wool dress pants with modern slim fit design">
                    <div class="collection-info">
                        <h3>Wool Pants</h3>
                        <p>Premium merino wool</p>
                        <p class="price">₹13,299</p>
                        <a href="#" class="btn">Add to Cart</a>
                    </div>
                </div>
                <div class="collection-item">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/718512b4-7447-4968-bd56-4603dc1e51e7.png" alt="Luxurious brown silk button-down shirt with subtle sheen">
                    <div class="collection-info">
                        <h3>Silk Shirt</h3>
                        <p>Handcrafted with organic silk</p>
                        <p class="price">₹12,499</p>
                        <a href="#" class="btn">Add to Cart</a>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <section class="about" id="about">
        <div class="container">
            <h2 class="section-title">Our Story</h2>
            <div class="about-content">
                <div class="about-text">
                    <h2>Crafted With Passion</h2>
                    <p>LUNIX was born from a vision to create clothing that transcends trends and seasons. Our founder, inspired by the timeless elegance of earth tones and natural textures, set out to design a collection that honors craftsmanship while embracing modern silhouettes.</p>
                    <p>Each piece in our collection is thoughtfully designed to complement the modern wardrobe, offering versatility and sophistication. We source only the finest materials from ethical producers around the globe.</p>
                    <p>At LUNIX, we believe that true luxury lies in impeccable attention to detail, sustainable practices, and garments that stand the test of time.</p>
                </div>
                <div class="about-image">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/0d3f5ee5-04b7-4305-b416-bd20dbdb1d7e.png" alt="Bright designer workshop with fabrics in earthy tones and craftsmen working on premium garments">
                </div>
            </div>
        </div>
    </section>
    
    <section class="testimonials" id="testimonials">
        <div class="container">
            <h2 class="section-title">What Our Clients Say</h2>
            <div class="testimonial-grid">
                <div class="testimonial-card">
                    <p>"The cashmere sweater is the softest I've ever owned. The quality is exceptional and it's become a staple in my wardrobe year after year."</p>
                    <div class="testimonial-author">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/6bfd7de8-23dc-4d3f-bf7b-3df71cc7efbf.png" alt="Portrait of satisfied customer Sarah Mitchell">
                        <div class="author-info">
                            <h4>Sarah Mitchell</h4>
                            <p>Loyal Customer</p>
                        </div>
                    </div>
                </div>
                <div class="testimonial-card">
                    <p>"As someone who values both style and sustainability, LUNIX delivers on both fronts. The craftsmanship is evident in every stitch."</p>
                    <div class="testimonial-author">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/f3a6ebc5-07f9-4c3b-9b4b-4d18d5a9e644.png" alt="Portrait of satisfied customer James Donovan">
                        <div class="author-info">
                            <h4>James Donovan</h4>
                            <p>Fashion Editor</p>
                        </div>
                    </div>
                </div>
                <div class="testimonial-card">
                    <p>"The wool pants fit perfectly and have maintained their shape beautifully over time. Worth every penny for the investment in quality."</p>
                    <div class="testimonial-author">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/77127228-bc0b-4330-8689-bc0711c0504b.png" alt="Portrait of satisfied customer Alice Freeman">
                        <div class="author-info">
                            <h4>Alice Freeman</h4>
                            <p>Frequent Buyer</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <footer id="contact">
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>LUNIX</h3>
                    <p>Owner: Aditiya Pandey<br>Helpline: 9876414241<br>Elevating wardrobes with timeless design since 2015.</p>
                </div>
                <div class="footer-column">
                    <h3>Shop</h3>
                    <ul>
                        <li><a href="#">New Arrivals</a></li>
                        <li><a href="#">Best Sellers</a></li>
                        <li><a href="#">Accessories</a></li>
                        <li><a href="#">Gift Cards</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Customer Care</h3>
                    <ul>
                        <li><a href="#">Contact Us</a></li>
                        <li><a href="#">FAQs</a></li>
                        <li><a href="#">Shipping & Returns</a></li>
                        <li><a href="#">Size Guide</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Connect</h3>
                    <ul>
                        <li><a href="#">Instagram</a></li>
                        <li><a href="#">Facebook</a></li>
                        <li><a href="#">Customer Chat</a></li>
                        <li><a href="#">WhatsApp</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="social-links">
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-facebook"></i></a>
                <a href="#"><i class="fab fa-pinterest"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
            </div>
            
            <p class="copyright">© 2023 LUNIX. All rights reserved.</p>
        </div>
    </footer>
    <!-- 
    Steps to open in Chrome:
    1. Right-click on saved HTML file
    2. "Open With" पर क्लिक करें
    3. Google Chrome select करें
    -->
    
    <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
    <script>
    <!-- 
    VS Code में: 
    1. Extensions में "Live Server" install करें
    2. HTML file पर Right-click करके "Open with Live Server" चुनें
    -->
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
        
        // Sticky header effect
        window.addEventListener('scroll', function() {
            const header = document.querySelector('header');
            header.classList.toggle('sticky', window.scrollY > 0);
        });
        
        // Product hover effect enhancement
        document.querySelectorAll('.collection-item').forEach(item => {
            item.addEventListener('mouseenter', function() {
                this.querySelector('img').style.transform = 'scale(1.05)';
            });
            
            item.addEventListener('mouseleave', function() {
                this.querySelector('img').style.transform = 'scale(1)';
            });
        });
    </script>
</body>
    <!-- 
