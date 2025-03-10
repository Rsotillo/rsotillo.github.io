<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amüre W. Anat - Author</title>
    <style>
        :root {
            --cream: #F4EEE0;
            --dusty-pink: #D8B4A0;
            --deep-pink: #C88EA7;
            --charcoal: #393646;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Georgia', serif;
        }

        body {
            background-color: var(--cream);
            color: var(--charcoal);
            line-height: 1.6;
        }

        .header {
            padding: 20px 50px;
            position: fixed;
            width: 100%;
            top: 0;
            background: rgba(244, 238, 224, 0.95);
            z-index: 1000;
            border-bottom: 1px solid var(--dusty-pink);
        }

        .logo {
            font-size: 28px;
            color: var(--deep-pink);
            text-decoration: none;
            font-family: 'Playfair Display', serif;
        }

        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            padding: 150px 50px 0;
            background: linear-gradient(rgba(244, 238, 224, 0.9), rgba(244, 238, 224, 0.9)),
                        url('floral-pattern.png');
        }

        .hero-text h1 {
            color: var(--deep-pink);
            font-size: 52px;
            margin-bottom: 25px;
        }

        .section-title {
            color: var(--deep-pink);
            border-bottom: 2px solid var(--dusty-pink);
            padding-bottom: 10px;
            margin-bottom: 40px;
        }

        button, .cta-button {
            background: var(--deep-pink);
            color: var(--cream);
            padding: 12px 35px;
            border-radius: 25px;
            transition: all 0.3s ease;
        }

        button:hover, .cta-button:hover {
            background: var(--dusty-pink);
            transform: translateY(-2px);
        }

        .book-card {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(200, 142, 167, 0.1);
        }
    </style>
</head>
<body>
    <header class="header">
        <nav class="nav">
            <a href="#" class="logo">Amüre W. Anat</a>
            <div class="menu">
                <a href="#about">About</a>
                <a href="#books">Novels</a>
                <a href="#contact">Contact</a>
            </div>
        </nav>
    </header>

    <section class="hero">
        <div class="hero-content">
            <div class="hero-text">
                <h1>Where Dark Romance Blossoms</h1>
                <p>Bestselling author of gothic love stories that walk the line between passion and peril</p>
                <a href="#books" class="cta-button">Explore Novels</a>
            </div>
        </div>
    </section>

    <section id="about" class="section">
        <h2 class="section-title">About Amüre</h2>
        <div class="about-content">
            <div class="book-card">
                <p>"A wordsmith of the shadowed heart, Amüre W. Anat crafts tales where love survives 
                even the darkest trials. Based in New Orleans, her writing draws inspiration from 
                historical architecture and the complex beauty of human relationships."</p>
            </div>
        </div>
    </section>

    <section id="books" class="section">
        <h2 class="section-title">Published Works</h2>
        <div class="book-grid">
            <!-- Add book cards with:
            - Title: "Thorns of the Dahlia"
            - Description: "A forbidden affair in 19th century Venice..."
            
            - Title: "Velvet Coffins"
            - Description: "Modern-day vampire court politics..."
            -->
        </div>
    </section>
</body>
</html>
