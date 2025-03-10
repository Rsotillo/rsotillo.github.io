<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="Amüre W. Anat" content="Author">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amüre W. Anat | Author</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/aos/2.3.4/aos.css">
    <style>
        :root {
            --primary: #2e4a6b;
            --secondary: #f4f0e8;
            --accent: #d9a566;
            --text: #333333;
            --light: #ffffff;
            --dark: #121212;
            --transition: all 0.4s cubic-bezier(0.165, 0.84, 0.44, 1);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Montserrat', -apple-system, BlinkMacSystemFont, sans-serif;
        }

        body {
            background-color: var(--secondary);
            color: var(--text);
            line-height: 1.8;
            overflow-x: hidden;
        }

        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            padding: 1.5rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            transition: var(--transition);
            backdrop-filter: blur(10px);
            background: rgba(244, 240, 232, 0.8);
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
        }

        header.scrolled {
            padding: 1rem 5%;
            background: rgba(244, 240, 232, 0.95);
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary);
            text-decoration: none;
            letter-spacing: 1px;
        }

        .nav-links {
            display: flex;
            gap: 2rem;
        }

        .nav-links a {
            color: var(--primary);
            text-decoration: none;
            font-weight: 700; /* Changed from 500 to 700 for bold */
            position: relative;
            padding: 0.5rem 0;
            transition: var(--transition);
            font-size: 1.2rem; /* Increased font size */
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--accent);
            transition: var(--transition);
        }

        .nav-links a:hover {
            color: var(--accent);
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .mobile-toggle {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            color: var(--primary);
            cursor: pointer;
        }

        .hero {
            height: 100vh;
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 0 5%;
            background: linear-gradient(to right, rgba(46, 74, 107, 0.05), rgba(46, 74, 107, 0.01));
            overflow: hidden;
            position: relative;
        }

        .hero-content {
            display: flex;
            align-items: center;
            justify-content: space-between;
            width: 100%;
            max-width: 1200px;
            gap: 4rem;
        }

        .hero-text {
            flex: 1;
            text-align: left;
        }

        .hero-title {
            font-size: 4.5rem;
            font-weight: 700;
            line-height: 1.1;
            margin-bottom: 1.5rem;
            color: var(--primary);
            opacity: 0;
            animation: fadeIn 1s ease forwards 0.5s;
        }

        .hero-subtitle {
            font-size: 1.5rem;
            margin-bottom: 2rem;
            color: var(--text);
            opacity: 0;
            animation: fadeIn 1s ease forwards 0.8s;
        }

        .hero-image {
            flex: 1;
            position: relative;
            opacity: 0;
            animation: fadeIn 1s ease forwards 1s;
        }

        .hero-image img {
            width: 100%;
            max-width: 500px;
            border-radius: 10px;
            box-shadow: 0 15px 50px rgba(0, 0, 0, 0.1);
        }

        /* Removed overlay and hover effects for hero-image */

        .section {
            padding: 120px 5%;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .section-inner {
            display: flex;
            align-items: center;
            justify-content: space-between;
            width: 100%;
            max-width: 1200px;
            gap: 5rem;
        }

        .section-title {
            font-size: 2.5rem;
            font-weight: 700;
            margin-bottom: 1.5rem;
            color: var(--primary);
            position: relative;
            display: inline-block;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 60px;
            height: 3px;
            background: var(--accent);
            transition: var(--transition);
        }

        .text-content:hover .section-title::after {
            width: 100px;
        }

        .text-content {
            flex: 1;
            text-align: left;
        }

        .main-text {
            font-size: 1.1rem;
            line-height: 1.8;
            color: var(--text);
        }

        .image-container {
            flex: 1;
            position: relative;
            overflow: hidden;
        }

        .image-container img {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 15px 50px rgba(0, 0, 0, 0.1);
        }

        /* Removed image hover effects */
        /* Removed overlay styles for image containers */

        .book-section {
            background-color: var(--primary);
            color: var(--light);
            position: relative;
            overflow: hidden;
        }

        .book-section::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="100" height="100" viewBox="0 0 100 100"><rect width="100" height="100" fill="none"/><path d="M0,0L100,100" stroke="rgba(255,255,255,0.05)" stroke-width="1"/></svg>');
            opacity: 0.2;
        }

        .book-section .section-title {
            color: var(--light);
        }

        .book-section .main-text {
            color: var(--secondary);
        }

        .book-section .section-title::after {
            background: var(--accent);
        }
        
        .book-title {
            font-size: 1.5rem;
            font-weight: 700;
            margin-bottom: 1rem;
            color: var(--accent);
        }

        .contact-section {
            background-color: var(--light);
            text-align: center;
            padding: 100px 5%;
        }

        .contact-section .section-title {
            display: inline-block;
        }

        .contact-section .section-title::after {
            left: 50%;
            transform: translateX(-50%);
        }

        .contact-info {
            margin: 3rem 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 1.5rem;
        }

        .contact-info p {
            font-size: 1.2rem;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .contact-info p i {
            color: var(--accent);
        }

        .social-links {
            display: flex;
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .social-link {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background-color: var(--primary);
            color: var(--light);
            text-decoration: none;
            font-size: 1.2rem;
            transition: var(--transition);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .social-link:hover {
            transform: translateY(-5px);
            background-color: var(--accent);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
        }

        footer {
            background-color: var(--dark);
            color: var(--secondary);
            text-align: center;
            padding: 2rem;
        }

        .back-to-top {
            position: fixed;
            bottom: 2rem;
            right: 2rem;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background-color: var(--primary);
            color: var(--light);
            display: flex;
            align-items: center;
            justify-content: center;
            text-decoration: none;
            font-size: 1.2rem;
            transition: var(--transition);
            opacity: 0;
            visibility: hidden;
            z-index: 999;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .back-to-top.visible {
            opacity: 1;
            visibility: visible;
        }

        .back-to-top:hover {
            background-color: var(--accent);
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @media (max-width: 992px) {
            .hero-title {
                font-size: 3.5rem;
            }
            
            .section-inner {
                flex-direction: column;
                gap: 3rem;
            }
            
            .section-inner.reverse {
                flex-direction: column-reverse;
            }
            
            .image-container, .text-content {
                width: 100%;
            }
        }

        @media (max-width: 768px) {
            .hero-content {
                flex-direction: column-reverse;
                text-align: center;
                gap: 2rem;
            }
            
            .hero-title {
                font-size: 2.8rem;
            }
            
            .hero-subtitle {
                font-size: 1.2rem;
            }
            
            .mobile-toggle {
                display: block;
            }
            
            .nav-links {
                position: fixed;
                top: 0;
                right: -100%;
                width: 250px;
                height: 100vh;
                background-color: var(--light);
                flex-direction: column;
                justify-content: center;
                align-items: center;
                padding: 2rem;
                transition: var(--transition);
                box-shadow: -5px 0 30px rgba(0, 0, 0, 0.1);
            }
            
            .nav-links.active {
                right: 0;
            }
            
            .section-title {
                font-size: 2rem;
            }
            
            .text-content {
                text-align: center;
            }
            
            .section-title::after {
                left: 50%;
                transform: translateX(-50%);
            }
        }
    </style>
</head>
<body>
    <header id="header">
        <a href="#" class="logo">Amüre W. Anat</a>
        <button class="mobile-toggle" id="mobileToggle">
            <i class="fas fa-bars"></i>
        </button>
        <nav class="nav-links" id="navLinks">
            <a href="#home">Home</a>
            <a href="#bio">Bio</a>
            <a href="#book">Projects</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section id="home" class="hero">
        <div class="hero-content">
            <div class="hero-text">
             <h1 class="hero-title">Dear,</h1>
                <div class="main-text">
                    <p>
                        Here we are. You and me on a digital layer. Face to face, in different times, in different places. <br><br>
                        Check my debut novel, read it through, pay attention, drop the book and forget you even read it. Because nothing is too serious, but the tyranny of the rich, and drudgery of the dull.
                    </p>
                </div>
            </div>
            <div class="hero-image">
                <img src="Screenshot 2025-03-06 at 16.52.09.jpeg" alt="Foto Reciente">
                <!-- Removed overlay div -->
            </div>
        </div>
    </section>

    <section id="bio" class="section">
        <div class="section-inner" data-aos="fade-up">
            <div class="image-container">
                <img src="Screenshot 2025-03-10 at 11.18.20.jpeg" alt="Bio Image">
                <!-- Removed overlay div -->
            </div>
            <div class="text-content">
                <h2 class="section-title">Bio</h2>
                <p class="main-text">
                    1996 - Forever and Never<br><br>
                    Born and exist. I love life even though I tried to end it. I've moved in different levels of consciousness many times, up, down, up, down, and always kept flowing to the next one. Life is black and white, grey and colorful. Bright and beautiful, dark and twisted.<br><br>
                    I was born in Venezuela, and lived most of my life in a tiny island of the Caribbean. Also lived in Argentina, America, and I'm currently living in Spain.
                </p>
            </div>
        </div>
    </section>

    <section id="book" class="section book-section">
        <div class="section-inner reverse" data-aos="fade-up">
            <div class="text-content">
                <h2 class="section-title">Projects</h2>
                <h3 class="book-title">Dear God, King David is Dead</h3>
                    It is a contemporary coming-of-age story about the highs of reinvention and the inevitable pull of self-destruction.

                    <br><br>

                    A boy escapes his past by reinventing himself in Miami's nightlife, but as friendships fade and love slips through his fingers, he realizes that no matter how far he runs, he can't escape himself.

                    <br><br>

                    Through a deeply introspective and emotionally charged narrative, it explores identity, loneliness, and the fleeting nature of joy, while subtly engaging with themes of anti-capitalism and distrust in authority. 

                    <br><br>

                    It's wild, fun and emotional.
            </div>
            <div class="image-container">
    <img src="an_english_cod_2014.136.5.jpg" alt="Dear God Image">
    <p style="font-size: 0.65rem; color: #999; margin-top: 5px; text-align: right;">William Merritt Chase (painter) American, 1849 - 1916</p>
</div>
<!-- This should be placed inside the existing book-section, after the Dear God project content -->
<div class="gallery-container" data-aos="fade-up" data-aos-delay="200">
    <h3 class="gallery-title">Paintings</h3>
    <div class="gallery-row">
        <div class="gallery-item">
            <div class="gallery-image-container">
                <img src="IMG_4944.jpeg" alt="Painting 1">
                <img src="IMG_4915.jpeg" alt="Painting 1">
                <div class="painting-info">
                    <p class="painting-title">Respect All</p>
                    <p class="painting-year">2021</p>
                </div>
            </div>
        </div>
        <div class="gallery-item">
            <div class="gallery-image-container">
                <img src="E12778F9-DE47-445B-ABC2-0CA8B8FD379A_1_105_c.jpeg" alt="Painting 2">
                <div class="painting-info">
                    <p class="painting-title">Sin Ti</p>
                    <p class="painting-year">2021</p>
                </div>
            </div>
        </div>
    </div>
    <div class="gallery-row">
        <div class="gallery-item">
            <div class="gallery-image-container">
                <img src="8043D5F1-3883-4325-B418-00878CFA2490_1_105_c.jpeg" alt="Painting 3">
                <div class="painting-info">
                    <p class="painting-title">Lonelier Everyday</p>
                    <p class="painting-year">2022</p>
                </div>
            </div>
        </div>
        <div class="gallery-item">
            <div class="gallery-image-container">
                <img src="E6733AE1-27BA-4BCD-AC43-984F11D68BD8_1_105_c.jpeg" alt="Painting 4">
                <div class="painting-info">
                    <p class="painting-title">Untitled</p>
                    <p class="painting-year">2022</p>
                </div>
            </div>
        </div>
    </div>
</div>

<style>
    /* Gallery Section Styles */
    .gallery-title {
        font-size: 1.5rem;
        font-weight: 700;
        margin: 3rem 0 2rem;
        color: var(--accent);
    }
    
    .gallery-container {
        width: 100%;
        margin-top: 4rem;
    }

    .gallery-row {
        display: flex;
        justify-content: space-between;
        gap: 2rem;
        margin-bottom: 2rem;
    }

    .gallery-item {
        flex: 1;
    }

    .gallery-image-container {
        width: 100%;
        height: 0;
        padding-bottom: 85%; /* Larger aspect ratio for bigger images */
        position: relative;
        overflow: hidden;
        border-radius: 10px;
        box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
        transition: var(--transition);
    }

    .gallery-image-container:hover {
        transform: translateY(-5px);
        box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
    }

    .gallery-image-container img {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        object-fit: cover;
    }

    .painting-info {
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
        padding: 15px;
        background: linear-gradient(to top, rgba(0,0,0,0.7), transparent);
    }

    .painting-title {
        font-size: 1.2rem;
        font-weight: 600;
        margin: 0 0 0.2rem;
        color: white;
    }

    .painting-year {
        font-size: 0.8rem;
        color: white;
        opacity: 0.8;
        margin: 0;
    }

    /* Mobile Responsive Adjustments */
    @media (max-width: 768px) {
        .gallery-row {
            flex-direction: column;
            gap: 2rem;
        }

        .gallery-image-container {
            padding-bottom: 100%; /* Square aspect ratio on mobile */
        }
        
        /* Make sure text is fully visible */
        .painting-info {
            padding: 12px;
        }
        
        .painting-title {
            font-size: 1.1rem;
        }
        
        .painting-year {
            font-size: 0.7rem;
        }
    }
</style>
        </div>
    </section>

    <section id="contact" class="contact-section">
        <h2 class="section-title" data-aos="fade-up">Contact Information</h2>
        <div class="contact-info" data-aos="fade-up" data-aos-delay="200">
            <p><i class="fas fa-phone"></i> +34 645-076-253</p>
            <p><i class="fas fa-envelope"></i> <a href="mailto:Aishtapamura@gmail.com" style="color: var(--primary); text-decoration: none;">Aishtapamura@gmail.com</a></p>
        </div>
        <div class="social-links" data-aos="fade-up" data-aos-delay="400">
            <a href="https://www.instagram.com/renesotillo/" target="_blank" class="social-link">
                <i class="fab fa-instagram"></i>
            </a>
            <a href="https://www.linkedin.com/in/amurewanat/" target="_blank" class="social-link">
                <i class="fab fa-linkedin-in"></i>
            </a>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 Amüre W. Anat. All rights reserved.</p>
    </footer>

    <a href="#" class="back-to-top" id="backToTop">
        <i class="fas fa-arrow-up"></i>
    </a>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/aos/2.3.4/aos.js"></script>
    <script>
        // Initialize AOS
        AOS.init({
            duration: 800,
            easing: 'ease-in-out',
            once: true,
            offset: 100
        });

        // Mobile Navigation Toggle
        const mobileToggle = document.getElementById('mobileToggle');
        const navLinks = document.getElementById('navLinks');
        
        mobileToggle.addEventListener('click', () => {
            navLinks.classList.toggle('active');
            mobileToggle.innerHTML = navLinks.classList.contains('active') 
                ? '<i class="fas fa-times"></i>' 
                : '<i class="fas fa-bars"></i>';
        });

        // Close mobile nav when clicking on links
        document.querySelectorAll('.nav-links a').forEach(link => {
            link.addEventListener('click', () => {
                navLinks.classList.remove('active');
                mobileToggle.innerHTML = '<i class="fas fa-bars"></i>';
            });
        });

        // Header scroll effect
        const header = document.getElementById('header');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 100) {
                header.classList.add('scrolled');
            } else {
                header.classList.remove('scrolled');
            }
        });

        // Back to top button
        const backToTop = document.getElementById('backToTop');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 500) {
                backToTop.classList.add('visible');
            } else {
                backToTop.classList.remove('visible');
            }
        });

        backToTop.addEventListener('click', (e) => {
            e.preventDefault();
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });

        // Smooth scrolling for all anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    const headerHeight = document.getElementById('header').offsetHeight;
                    const targetPosition = targetElement.getBoundingClientRect().top + window.pageYOffset - headerHeight;
                    
                    window.scrollTo({
                        top: targetPosition,
                        behavior: 'smooth'
                    });
                }
            });
        });
    </script>
</body>
</html>
