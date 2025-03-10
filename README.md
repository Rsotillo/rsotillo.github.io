
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amüre W. Anat</title>
    <style>
        :root {
            --black: #000000;
            --steel-blue: #2e4a6b;
            --cream: #f4f0e8;
            --transition: all 0.3s ease-in-out;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Questrial', sans-serif;
        }

        body {
            background-color: var(--cream);
            color: var(--black);
            line-height: 1.6;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            align-items: center;
            padding: 4rem 2rem;
            gap: 40px;
            max-width: 1200px;
        }

        .section {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 40px;
            max-width: 1200px;
            padding: 2rem 0;
            opacity: 0;
            transform: translateY(20px);
            animation: fadeIn 0.6s ease forwards;
        }

        @keyframes fadeIn {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .section img {
            width: 45%;
            max-width: 500px;
            border-radius: 8px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            transition: var(--transition);
        }

        .section img:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(0,0,0,0.15);
        }

        .text-content {
            width: 45%;
            text-align: left;
            padding: 2rem;
        }

        .section-title {
            font-size: 2.5rem;
            margin-bottom: 1.5rem;
            color: var(--steel-blue);
            position: relative;
            display: inline-block;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 60%;
            height: 2px;
            background: var(--steel-blue);
        }

        .main-text {
            font-size: 1.1rem;
            line-height: 1.8;
            color: #444;
            max-width: 80ch;
        }

        .contact {
            margin: 4rem 0;
            text-align: center;
            padding: 2rem;
            background: rgba(255,255,255,0.9);
            border-radius: 12px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .contact h2 {
            font-size: 2rem;
            margin-bottom: 1.5rem;
            color: var(--steel-blue);
        }

        .contact a {
            display: inline-block;
            margin: 10px;
            color: var(--steel-blue);
            text-decoration: none;
            padding: 0.5rem 1rem;
            border-radius: 6px;
            transition: var(--transition);
        }

        .contact a:hover {
            background: rgba(46,74,107,0.1);
            transform: translateY(-2px);
        }

        @media (max-width: 768px) {
            .section {
                flex-direction: column;
                padding: 1rem;
            }

            .section img, .text-content {
                width: 100%;
                text-align: center;
            }

            .text-content {
                padding: 1rem;
            }

            .section-title {
                font-size: 2rem;
            }

            .contact {
                margin: 2rem 0;
                padding: 1rem;
            }
        }
    </style>
</head>
<body>
    <!-- Original Content Preserved Exactly -->
    <div class="container section">
        <div class="text-content">
            <div class="section-title">Dear,</div>
            <p class="main-text">
                Here we are. You and me on a digital layer. Face to face, in different times, in different places. <br><br>
                Check my debut novel, read it through, pay attention, drop the book and forget you even read it. Because nothing is too serious, but the tyranny of the rich, and drudgery of the dull.
            </p>
        </div>
        <img src="Screenshot 2025-03-06 at 16.52.09.jpeg" alt="Foto Reciente">
    </div>

    <div class="container section">
        <img src="Screenshot 2025-03-10 at 11.18.20.jpeg" alt="Bio Image">
        <div class="text-content">
            <div class="section-title">Bio</div>
            <p class="main-text">
                1996 - Forever and Never<br><br>
                Born and exist. I love life even though I tried to end it. I've moved in different levels of consciousness many times, up, down, up, down, and always kept flowing to the next one. Life is black and white, grey and colorful. Bright and beautiful, dark and twisted.<br><br>
                I was born in Venezuela, and lived most of my life in a tiny island of the Caribbean. Also lived in Argentina, America, and I'm currently living in Spain.
            </p>
        </div>
    </div>

    <div class="container section">
        <div class="text-content">
            <div class="section-title">Dear God, King David is Dead</div>
            <p class="main-text">
                It is a contemporary coming-of-age story about the highs of reinvention and the inevitable pull of self-destruction.

​<br><br>

A boy escapes his past by reinventing himself in Miami’s nightlife, but as friendships fade and love slips through his fingers, he realizes that no matter how far he runs, he can’t escape himself.

​<br><br>

Through a deeply introspective and emotionally charged narrative, it explores identity, loneliness, and the fleeting nature of joy, while subtly engaging with themes of anti-capitalism and distrust in authority. ​

​<br><br>

It's wild, fun and emotional.
            </p>
        </div>
        <img src="an_english_cod_2014.136.5.jpg" alt="Dear God Image">
    </div>

    <div class="contact">
        <h2>Contact Information</h2>
        <p>Phone: +34 645-076-253</p>
        <p>Email: <a href="mailto:Aishtapamura@gmail.com">Aishtapamura@gmail.com</a></p>
        <a href="https://www.instagram.com/renesotillo/" target="_blank">Instagram</a>
        <a href="https://www.linkedin.com/in/amurewanat/" target="_blank">LinkedIn</a>
    </div>

    <script>
        // Optional: Add smooth scroll behavior
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
