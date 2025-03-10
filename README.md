<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Author Portfolio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }

        body {
            background-color: #1a1a1a;
            color: #ffffff;
        }

        .header {
            padding: 20px 50px;
            position: fixed;
            width: 100%;
            top: 0;
            background: rgba(26, 26, 26, 0.9);
            z-index: 1000;
        }

        .nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 24px;
            color: #c5a47e;
            text-decoration: none;
            font-family: 'Times New Roman', serif;
        }

        .menu {
            display: flex;
            gap: 30px;
        }

        .menu a {
            color: #ffffff;
            text-decoration: none;
            text-transform: uppercase;
            font-size: 14px;
        }

        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            padding: 0 50px;
            background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)),
                        url('hero-bg.jpg');
            background-size: cover;
        }

        .hero-content {
            display: flex;
            justify-content: space-between;
            width: 100%;
            align-items: center;
        }

        .hero-text {
            width: 50%;
        }

        .hero-text h1 {
            font-size: 48px;
            color: #c5a47e;
            margin-bottom: 20px;
            font-family: 'Times New Roman', serif;
        }

        .hero-image {
            width: 40%;
            text-align: center;
        }

        .hero-image img {
            max-width: 400px;
            height: auto;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
        }

        .section {
            padding: 100px 50px;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
            color: #c5a47e;
            font-family: 'Times New Roman', serif;
        }

        .about-content {
            display: flex;
            gap: 50px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .contact-form {
            max-width: 600px;
            margin: 0 auto;
        }

        input, textarea {
            width: 100%;
            padding: 10px;
            margin-bottom: 20px;
            background: #333;
            border: 1px solid #444;
            color: white;
        }

        button {
            background: #c5a47e;
            color: white;
            padding: 15px 30px;
            border: none;
            cursor: pointer;
            text-transform: uppercase;
        }

        .social-links {
            text-align: center;
            margin-top: 50px;
        }

        .social-links a {
            color: #c5a47e;
            margin: 0 15px;
            font-size: 20px;
        }

    </style>
</head>
<body>
    <header class="header">
        <nav class="nav">
            <a href="#" class="logo">Author Name</a>
            <div class="menu">
                <a href="#about">About</a>
                <a href="#books">Books</a>
                <a href="#contact">Contact</a>
            </div>
        </nav>
    </header>

    <section class="hero">
        <div class="hero-content">
            <div class="hero-text">
                <h1>Bestselling Author</h1>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
            </div>
            <div class="hero-image">
                <img src="book-cover.jpg" alt="Book Cover">
            </div>
        </div>
    </section>

    <section id="about" class="section">
        <h2 class="section-title">About the Author</h2>
        <div class="about-content">
            <div class="about-text">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit...</p>
            </div>
        </div>
    </section>

    <section id="contact" class="section">
        <h2 class="section-title">Contact</h2>
        <form class="contact-form">
            <input type="text" placeholder="Name">
            <input type="email" placeholder="Email">
            <textarea rows="5" placeholder="Message"></textarea>
            <button type="submit">Send Message</button>
        </form>
        <div class="social-links">
            <a href="#">Facebook</a>
            <a href="#">Twitter</a>
            <a href="#">Instagram</a>
        </div>
    </section>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
